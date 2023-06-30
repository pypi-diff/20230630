# Comparing `tmp/tvm_valuetypes-0.0.8-py3-none-any.whl.zip` & `tmp/tvm_valuetypes-0.0.9-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,11 +1,11 @@
-Zip file size: 8895 bytes, number of entries: 9
+Zip file size: 9034 bytes, number of entries: 9
 -rw-rw-r--  2.0 unx      176 b- defN 22-Jan-11 16:39 tvm_valuetypes/__init__.py
--rw-rw-r--  2.0 unx    12781 b- defN 22-Apr-03 12:28 tvm_valuetypes/cell.py
--rw-rw-r--  2.0 unx     2979 b- defN 22-Jan-11 16:39 tvm_valuetypes/dict_utils.py
--rw-rw-r--  2.0 unx     2671 b- defN 22-Feb-15 17:43 tvm_valuetypes/stack_utils.py
--rw-rw-r--  2.0 unx     1181 b- defN 22-Apr-03 12:31 tvm_valuetypes-0.0.8.dist-info/LICENSE
--rw-rw-r--  2.0 unx     2177 b- defN 22-Apr-03 12:31 tvm_valuetypes-0.0.8.dist-info/METADATA
--rw-rw-r--  2.0 unx       92 b- defN 22-Apr-03 12:31 tvm_valuetypes-0.0.8.dist-info/WHEEL
--rw-rw-r--  2.0 unx       15 b- defN 22-Apr-03 12:31 tvm_valuetypes-0.0.8.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx      754 b- defN 22-Apr-03 12:31 tvm_valuetypes-0.0.8.dist-info/RECORD
-9 files, 22826 bytes uncompressed, 7591 bytes compressed:  66.7%
+-rw-rw-r--  2.0 unx    14628 b- defN 22-May-16 06:27 tvm_valuetypes/cell.py
+-rw-rw-r--  2.0 unx     3336 b- defN 22-May-16 06:25 tvm_valuetypes/dict_utils.py
+-rw-rw-r--  2.0 unx     3165 b- defN 22-May-16 06:25 tvm_valuetypes/stack_utils.py
+-rw-rw-r--  2.0 unx     1181 b- defN 22-May-16 06:29 tvm_valuetypes-0.0.9.dist-info/LICENSE
+-rw-rw-r--  2.0 unx     2177 b- defN 22-May-16 06:29 tvm_valuetypes-0.0.9.dist-info/METADATA
+-rw-rw-r--  2.0 unx       92 b- defN 22-May-16 06:29 tvm_valuetypes-0.0.9.dist-info/WHEEL
+-rw-rw-r--  2.0 unx       15 b- defN 22-May-16 06:29 tvm_valuetypes-0.0.9.dist-info/top_level.txt
+?rw-rw-r--  2.0 unx      754 b- defN 22-May-16 06:29 tvm_valuetypes-0.0.9.dist-info/RECORD
+9 files, 25524 bytes uncompressed, 7730 bytes compressed:  69.7%
```

## zipnote {}

```diff
@@ -6,23 +6,23 @@
 
 Filename: tvm_valuetypes/dict_utils.py
 Comment: 
 
 Filename: tvm_valuetypes/stack_utils.py
 Comment: 
 
-Filename: tvm_valuetypes-0.0.8.dist-info/LICENSE
+Filename: tvm_valuetypes-0.0.9.dist-info/LICENSE
 Comment: 
 
-Filename: tvm_valuetypes-0.0.8.dist-info/METADATA
+Filename: tvm_valuetypes-0.0.9.dist-info/METADATA
 Comment: 
 
-Filename: tvm_valuetypes-0.0.8.dist-info/WHEEL
+Filename: tvm_valuetypes-0.0.9.dist-info/WHEEL
 Comment: 
 
-Filename: tvm_valuetypes-0.0.8.dist-info/top_level.txt
+Filename: tvm_valuetypes-0.0.9.dist-info/top_level.txt
 Comment: 
 
-Filename: tvm_valuetypes-0.0.8.dist-info/RECORD
+Filename: tvm_valuetypes-0.0.9.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## tvm_valuetypes/cell.py

```diff
@@ -1,367 +1,443 @@
-from bitarray import bitarray
-from math import ceil
-from hashlib import sha256
-from crc32c import crc32 as crc32c
 import codecs
 import json
+from hashlib import sha256
+from math import ceil
+
+from bitarray import bitarray
+from crc32c import crc32 as crc32c
 
 reach_boc_magic_prefix = b'\xB5\xEE\x9C\x72'
 lean_boc_magic_prefix = b'\x68\xff\x65\xf3'
 lean_boc_magic_prefix_crc = b'\xac\xc3\xa7\x28'
 
 
 class CellData:
-  def __init__(self):
-    self.data = bitarray()
-  def put_bool(self, element):
-    if(len(self.data)>=1023):
-      raise Exception("Cell overflow")
-    self.data.append(element)
-  def put_arbitrary_uint(self, uint, bitsize):
-    if bitsize<=0 or (2**bitsize-1 < uint):
-      raise Exception("Not enough bits (%d) to encode integer (%d)"%(bitsize, uint))
-    for i in range(bitsize, 0, -1):
-      k = (2**(i-1))
-      if uint//k == 1:
-         self.put_bool(1)
-         uint -=k
-      else:
-         self.put_bool(0)
-  def put_uint8(self, uint):
-    self.put_arbitrary_uint(uint, 8)
-  def put_arbitrary_int(self, _int, bitsize):
-    if bitsize == 1:
-      if _int in [0,-1]:
-        self.put_bool(_int==-1)
-        return
-      else:
-        raise Exception("Not enough bits (%d) to encode integer (%d)"%(bitsize, uint))
-    if _int<0:
-      self.put_bool(1)
-      s = 2**(bitsize-1)
-      self.put_arbitrary_uint(s-_int, bitsize-1)
-    else:
-      self.put_bool(0)
-      self.put_arbitrary_uint(_int, bitsize-1)
-  def concatenate(self, another_cell_data):
-    if(self.length() + another_cell_data.length() > 1023):
-      raise Exception("Not enough bits to concantenate cells: %d + %d"%(self.length(), another_cell_data.length()))
-    self.data.extend(another_cell_data.data)
-  def top_up(self):
-    l= len(self.data)
-    additional_bits = ceil(l/8) - l//8
-    if(ceil(l/8)==128):
-      additional_bits-=1
-    for i in range(additional_bits):
-      if i==0:
-        self.put_bool(1)
-      else:
-        self.put_bool(0)
-  def copy(self):
-    cd = CellData()
-    cd.data = bitarray(self.data)
-    return cd
-  def length(self):
-    return len(self.data)
-  def top_upped_bytes(self):
-    t = self.copy()
-    t.top_up()
-    return t.data.tobytes()
-  def from_bytes(self, data, top_upped=False):
-    self.data = bitarray()
-    self.data.frombytes(data)
-    if top_upped:
-      x = self.data.pop()
-      while not x:
-        x = self.data.pop()
-  def __eq__(self, another_cell_data):
-    return (self.data.tobytes() == another_cell_data.data.tobytes()) and (self.length() == another_cell_data.length())
-
-  def __len__(self):
-    return self.length()
-
-  def __repr__(self):
-    if(self.length()%8):
-      x = self.copy()
-      x.top_up()
-      return "%s_"%(x.data.tobytes())
-    else:
-      return "%s"%(self.data.tobytes())
+    def __init__(self):
+        self.data = bitarray()
+
+    def put_bool(self, element):
+        if len(self.data) >= 1023:
+            raise Exception("Cell overflow")
+        self.data.append(element)
+
+    def put_arbitrary_uint(self, uint, bitsize):
+        if bitsize <= 0 or (2 ** bitsize - 1 < uint):
+            raise Exception(
+                "Not enough bits (%d) to encode integer (%d)" %
+                (bitsize, uint))
+        for i in range(bitsize, 0, -1):
+            k = (2 ** (i - 1))
+            if uint // k == 1:
+                self.put_bool(1)
+                uint -= k
+            else:
+                self.put_bool(0)
+
+    def put_uint8(self, uint):
+        self.put_arbitrary_uint(uint, 8)
+
+    def put_arbitrary_int(self, _int, bitsize):
+        if bitsize == 1:
+            if _int in [0, -1]:
+                self.put_bool(_int == -1)
+                return
+            else:
+                raise Exception(
+                    "Not enough bits (%d) to encode integer (%d)" %
+                    (bitsize, uint))
+        if _int < 0:
+            self.put_bool(1)
+            s = 2 ** (bitsize - 1)
+            self.put_arbitrary_uint(s - _int, bitsize - 1)
+        else:
+            self.put_bool(0)
+            self.put_arbitrary_uint(_int, bitsize - 1)
+
+    def concatenate(self, another_cell_data):
+        if self.length() + another_cell_data.length() > 1023:
+            raise Exception(
+                "Not enough bits to concantenate cells: %d + %d" %
+                (self.length(), another_cell_data.length()))
+        self.data.extend(another_cell_data.data)
+
+    def top_up(self):
+        l = len(self.data)
+        additional_bits = ceil(l / 8) - l // 8
+        if ceil(l / 8) == 128:
+            additional_bits -= 1
+        for i in range(additional_bits):
+            if i == 0:
+                self.put_bool(1)
+            else:
+                self.put_bool(0)
+
+    def copy(self):
+        cd = CellData()
+        cd.data = bitarray(self.data)
+        return cd
+
+    def length(self):
+        return len(self.data)
+
+    def top_upped_bytes(self):
+        t = self.copy()
+        t.top_up()
+        return t.data.tobytes()
+
+    def from_bytes(self, data, top_upped=False):
+        self.data = bitarray()
+        self.data.frombytes(data)
+        if top_upped:
+            x = self.data.pop()
+            while not x:
+                x = self.data.pop()
+
+    def __eq__(self, another_cell_data):
+        return (self.data.tobytes() == another_cell_data.data.tobytes()) and (
+            self.length() == another_cell_data.length())
+
+    def __len__(self):
+        return self.length()
+
+    def __repr__(self):
+        if self.length() % 8:
+            x = self.copy()
+            x.top_up()
+            return "%s_" % (x.data.tobytes())
+        else:
+            return "%s" % (self.data.tobytes())
 
 
 class Cell:
-  def __init__(self):
-    self.data = CellData()
-    self.refs = []
-  def level(self):
-    max_level = 0;
-    for k in self.refs:
-      if k.level() > max_level:
-        max_level = k.level()
-    return max_level;
-  def is_special(self):
-    return 0
-  def is_explicitly_stored_hashes(self):
-    return 0
-  def depth(self):
-    max_depth = 0;
-    if len(self.refs) > 0:
-      for k in self.refs:
-        if k.depth() > max_depth:
-          max_depth = k.depth()
-      max_depth = max_depth + 1
-    return max_depth
-  def encoded_depth(self):
-    return (self.depth()//256).to_bytes(1, "big")+(self.depth()%256).to_bytes(1, "big")
-  def concatenate(self, another_cell):
-    self.data.concatenate(another_cell.data);
-    self.refs = self.refs + another_cell.refs
-  def descripter1(self):    
-    return (len(self.refs) + self.is_special() * 8 + self.level() * 32).to_bytes(1, "big")
-  def descripter2(self):
-    return ((len(self.data) // 8) + ceil(len(self.data) / 8)).to_bytes(1, "big")
-  def data_with_descriptors(self): 
-    return self.descripter1() + self.descripter2() + self.data.top_upped_bytes()
-  def repr(self):
-    ret = self.data_with_descriptors()
-    for k in self.refs:
-      ret += k.encoded_depth()
-    for k in self.refs:
-      ret += k.hash()
-    return ret
-  def hash(self):
-    hasher = sha256()
-    hasher.update(self.repr())
-    return hasher.digest()
-  
-  def serialize_for_boc(self, cells_index, ref_size):
-    # This is not serialization of the cell as boc with this cell as root_cell
-    # it is serialization of the cell to be used in boc serialization
-    ret = self.data_with_descriptors();
-    if self.is_explicitly_stored_hashes(): 
-      raise NotImplementedError("Do not support explicitly stored hashes yet")
-    for k in self.refs:
-      ret += (cells_index[ k.hash()].to_bytes(ref_size, "big"))
-    return ret
-    
-  def serialize_for_boc_size(self, cells_index, ref_size):
-    return len(self.serialize_for_boc( cells_index, ref_size))
-
-  def build_indexes(self):
-    def tree_walk(cell, topological_order_array, index_hashmap):
-      cell_hash = cell.hash();
-      index_hashmap[cell_hash] = len(topological_order_array);
-      topological_order_array.append((cell_hash, cell));
-      for subcell in cell.refs:
-        topological_order_array, index_hashmap = tree_walk(subcell, topological_order_array, index_hashmap);
-      return topological_order_array, index_hashmap;
-    return tree_walk(self, [], {})
-    
-  def serialize_boc(self, has_idx=True, hash_crc32=True, has_cache_bits=False, flags=0 ):
-    # This is serialization of the cell to boc as root_cell
-    topological_order, index_hashmap = self.build_indexes()
-    cells_num = len(topological_order);
-    s = cells_num.bit_length() # Minimal number of bits to represent reference (unused?)
-    s_bytes = min(ceil(s/8), 1)
-    full_size = 0
-    cell_sizes = {}
-    for (_hash, subcell) in topological_order:
-      cell_sizes[_hash] = subcell.serialize_for_boc_size(index_hashmap, s_bytes)
-      full_size += cell_sizes[_hash]
-    
-    offset_bits = full_size.bit_length() # Minimal number of bits to encode offset
-    offset_bytes =  max(ceil(offset_bits/8), 1)
-    # has_idx 1bit, hash_crc32 1bit,  has_cache_bits 1bit, flags 2bit, s_bytes 3 bit
-    flag_byte = (has_idx*128 + hash_crc32*64 + has_cache_bits*32 + flags*8 + s_bytes).to_bytes(1,"big")
-    ret = reach_boc_magic_prefix + flag_byte
-    ret += offset_bytes.to_bytes(1,"big")
-    ret += cells_num.to_bytes(offset_bytes,"big")
-    ret += (1).to_bytes(1,"big") # only one root in this implementation
-    ret += b'\x00' # complete BOCs only
-    ret += full_size.to_bytes(offset_bytes, "big")
-    ret += b'\x00' # Root shoulh have index 0
-    if has_idx:
-      current_offset = 0
-      for (_hash, subcell) in topological_order:
-        current_offset += cell_sizes[_hash]
-        ret += (current_offset).to_bytes(offset_bytes, "big")
-    for (_hash, subcell) in topological_order: 
-      ret += subcell.serialize_for_boc(index_hashmap, s_bytes)
-    if(hash_crc32):
-      ret += crc32c(ret).to_bytes(4, "little")
-    return ret
-
-  def copy(self):
-    ret = Cell()
-    ret.data = self.data.copy()
-    ret.refs = self.refs.copy()
-    return ret
-    
-  def __repr__(self):
-    return "<Cell refs_num: %d, data: %s>"%(len(self.refs), repr(self.data))
-    
-  def serialize_to_object(self):
-    ret = {'data':{'b64':b'', 'len':0}, 'refs':[]}
-    for r in self.refs:
-      ret['refs'].append(r.serialize_to_object())
-    ret['data']['b64'] = codecs.decode(codecs.encode(self.data.data.tobytes(), 'base64'), 'utf8').replace('\n','')
-    ret['data']['len'] = len(self.data)
-    return ret
-    
-  def serialize_to_json(self):
-    return json.dumps(self.serialize_to_object())
-    
-  def __eq__(self, another_cell):
-    if not len(self.refs) == len(another_cell.refs):
-      return False
-    for i in range(len(self.refs)):
-      if not self.refs[i] == another_cell.refs[i]:
-        return False
-    return self.data == another_cell.data
-    
+    def __init__(self):
+        self.data = CellData()
+        self.refs = []
+
+    def level(self):
+        max_level = 0
+        for k in self.refs:
+            if k.level() > max_level:
+                max_level = k.level()
+        return max_level
+
+    def is_special(self):
+        return 0
+
+    def is_explicitly_stored_hashes(self):
+        return 0
+
+    def depth(self):
+        max_depth = 0
+        if len(self.refs) > 0:
+            for k in self.refs:
+                if k.depth() > max_depth:
+                    max_depth = k.depth()
+            max_depth = max_depth + 1
+        return max_depth
+
+    def encoded_depth(self):
+        return (self.depth() // 256).to_bytes(1, "big") + \
+            (self.depth() % 256).to_bytes(1, "big")
+
+    def concatenate(self, another_cell):
+        self.data.concatenate(another_cell.data)
+        self.refs = self.refs + another_cell.refs
+
+    def descripter1(self):
+        return (len(self.refs) + self.is_special() *
+                8 + self.level() * 32).to_bytes(1, "big")
+
+    def descripter2(self):
+        return ((len(self.data) // 8) +
+                ceil(len(self.data) / 8)).to_bytes(1, "big")
+
+    def data_with_descriptors(self):
+        return self.descripter1() + self.descripter2() + self.data.top_upped_bytes()
+
+    def repr(self):
+        ret = self.data_with_descriptors()
+        for k in self.refs:
+            ret += k.encoded_depth()
+        for k in self.refs:
+            ret += k.hash()
+        return ret
+
+    def hash(self):
+        hasher = sha256()
+        hasher.update(self.repr())
+        return hasher.digest()
+
+    def serialize_for_boc(self, cells_index, ref_size):
+        # This is not serialization of the cell as boc with this cell as root_cell
+        # it is serialization of the cell to be used in boc serialization
+        ret = self.data_with_descriptors()
+        if self.is_explicitly_stored_hashes():
+            raise NotImplementedError(
+                "Do not support explicitly stored hashes yet")
+        for k in self.refs:
+            ret += (cells_index[k.hash()].to_bytes(ref_size, "big"))
+        return ret
+
+    def serialize_for_boc_size(self, cells_index, ref_size):
+        return len(self.serialize_for_boc(cells_index, ref_size))
+
+    def build_indexes(self):
+        def tree_walk(cell, topological_order_array, index_hashmap):
+            cell_hash = cell.hash()
+            index_hashmap[cell_hash] = len(topological_order_array)
+            topological_order_array.append((cell_hash, cell))
+            for subcell in cell.refs:
+                topological_order_array, index_hashmap = tree_walk(
+                    subcell, topological_order_array, index_hashmap)
+            return topological_order_array, index_hashmap
+
+        return tree_walk(self, [], {})
+
+    def serialize_boc(
+            self,
+            has_idx=True,
+            hash_crc32=True,
+            has_cache_bits=False,
+            flags=0):
+        # This is serialization of the cell to boc as root_cell
+        topological_order, index_hashmap = self.build_indexes()
+        cells_num = len(topological_order)
+        s = cells_num.bit_length()  # Minimal number of bits to represent reference (unused?)
+        s_bytes = min(ceil(s / 8), 1)
+        full_size = 0
+        cell_sizes = {}
+        for (_hash, subcell) in topological_order:
+            cell_sizes[_hash] = subcell.serialize_for_boc_size(
+                index_hashmap, s_bytes)
+            full_size += cell_sizes[_hash]
+
+        offset_bits = full_size.bit_length()  # Minimal number of bits to encode offset
+        offset_bytes = max(ceil(offset_bits / 8), 1)
+        # has_idx 1bit, hash_crc32 1bit,  has_cache_bits 1bit, flags 2bit,
+        # s_bytes 3 bit
+        flag_byte = (
+            has_idx * 128 +
+            hash_crc32 * 64 +
+            has_cache_bits * 32 +
+            flags * 8 +
+            s_bytes).to_bytes( 1, "big")
+        ret = reach_boc_magic_prefix + flag_byte
+        ret += offset_bytes.to_bytes(1, "big")
+        ret += cells_num.to_bytes(offset_bytes, "big")
+        ret += (1).to_bytes(1, "big")  # only one root in this implementation
+        ret += b'\x00'  # complete BOCs only
+        ret += full_size.to_bytes(offset_bytes, "big")
+        ret += b'\x00'  # Root shoulh have index 0
+        if has_idx:
+            current_offset = 0
+            for (_hash, subcell) in topological_order:
+                current_offset += cell_sizes[_hash]
+                ret += current_offset.to_bytes(offset_bytes, "big")
+        for (_hash, subcell) in topological_order:
+            ret += subcell.serialize_for_boc(index_hashmap, s_bytes)
+        if hash_crc32:
+            ret += crc32c(ret).to_bytes(4, "little")
+        return ret
+
+    def copy(self):
+        ret = Cell()
+        ret.data = self.data.copy()
+        ret.refs = self.refs.copy()
+        return ret
+
+    def __repr__(self):
+        return "<Cell refs_num: %d, data: %s>" % (
+            len(self.refs), repr(self.data))
+
+    def serialize_to_object(self):
+        ret = {'data': {'b64': b'', 'len': 0}, 'refs': []}
+        for r in self.refs:
+            ret['refs'].append(r.serialize_to_object())
+        ret['data']['b64'] = codecs.decode(
+            codecs.encode(
+                self.data.data.tobytes(),
+                'base64'),
+            'utf8').replace(
+            '\n',
+            '')
+        ret['data']['len'] = len(self.data)
+        return ret
+
+    def serialize_to_json(self):
+        return json.dumps(self.serialize_to_object())
+
+    def __eq__(self, another_cell):
+        if not len(self.refs) == len(another_cell.refs):
+            return False
+        for i in range(len(self.refs)):
+            if not self.refs[i] == another_cell.refs[i]:
+                return False
+        return self.data == another_cell.data
 
 
+def test_boc_serialization():
+    c0 = Cell()
+    res = c0.serialize_boc(has_idx=False)
+    reference_serialization_0 = bytes.fromhex(
+        "B5EE9C724101010100020000004CACB9CD")
+    assert res == reference_serialization_0, "Wrong empty cell boc-serialization"
+
+    c1 = Cell()
+    c1.data.put_uint8(0)
+    res = c1.serialize_boc(has_idx=False)
+    reference_serialization_1 = bytes.fromhex(
+        "B5EE9C7241010101000300000200D367DC41")
+    assert res == reference_serialization_1, "Wrong <b 0 8 u, b> cell boc-serialization"
+
+    c1 = Cell()
+    c2 = Cell()
+    c1.data.put_uint8(0)
+    c2.data.put_uint8(73)
+    c1.refs.append(c2)
+    res = c1.serialize_boc(has_idx=False)
+    reference_serialization_2 = bytes.fromhex(
+        "B5EE9C72410102010007000102000100024995C5FE15")
+    assert res == reference_serialization_2, "Wrong '<b 0 8 u, <b 73 8 u, b> ref, b>' cell boc-serialization"
 
 
-def test_boc_serialization():
-  c0 = Cell()
-  res = c0.serialize_boc(has_idx=False);
-  reference_serialization_0 = bytes.fromhex("B5EE9C724101010100020000004CACB9CD");
-  assert res == reference_serialization_0 , "Wrong empty cell boc-serialization"
-
-  c1 = Cell()
-  c1.data.put_uint8(0)
-  res = c1.serialize_boc(has_idx=False);
-  reference_serialization_1 = bytes.fromhex("B5EE9C7241010101000300000200D367DC41");
-  assert res == reference_serialization_1 , "Wrong <b 0 8 u, b> cell boc-serialization"
-  
-  c1 = Cell();
-  c2 = Cell();
-  c1.data.put_uint8(0);
-  c2.data.put_uint8(73);  
-  c1.refs.append(c2);
-  res = c1.serialize_boc(has_idx=False);
-  reference_serialization_2 = bytes.fromhex("B5EE9C72410102010007000102000100024995C5FE15");
-  assert res == reference_serialization_2 , "Wrong '<b 0 8 u, <b 73 8 u, b> ref, b>' cell boc-serialization"
-  
-  
 def parse_flags(serialization):
-  header_byte, serialization = serialization[0], serialization[1:]
-  has_idx, hash_crc32, has_cache_bits = header_byte & 128, header_byte & 64, header_byte & 32
-  header_byte %= 32
-  flags, size_bytes = header_byte >> 3, header_byte % 8
-  return (has_idx, hash_crc32, has_cache_bits, flags, size_bytes), serialization
-  
-  
+    header_byte, serialization = serialization[0], serialization[1:]
+    has_idx, hash_crc32, has_cache_bits = header_byte & 128, header_byte & 64, header_byte & 32
+    header_byte %= 32
+    flags, size_bytes = header_byte >> 3, header_byte % 8
+    return (has_idx, hash_crc32, has_cache_bits,
+            flags, size_bytes), serialization
+
+
 def deserialize_cell_data(ser, index_size):
-  d1, d2, ser = ser[0], ser[1], ser[2:]
-  level, d1 = (d1 // 32), d1 % 32
-  h, d1  = (d1 // 16), d1 % 16
-  if h>0:
-    raise NotImplementedError("Cell with explicit hash references are not supported yet")
-  s, r  = (d1 // 8), d1 % 8
-  if s>0:
-    raise NotImplementedError("Exoctic cell ware not supported yet")
-  if r>4:
-    raise NotImplementedError("Cell with explicit hash references are not supported yet (r>4)")
-  if d2%2:
-    data_size = (d2+1)//2
-    not_full = True
-  else:
-    data_size = d2//2
-    not_full = False
-  cell_data, ser = ser[:data_size], ser[data_size:]
-  c = Cell()
-  c.data.from_bytes(cell_data, top_upped=not_full)
-  for i in range(r):
-    ref_index, ser = int.from_bytes(ser[:index_size], "big"), ser[index_size:]
-    c.refs.append(ref_index)
-  return c, ser
-  
+    d1, d2, ser = ser[0], ser[1], ser[2:]
+    level, d1 = (d1 // 32), d1 % 32
+    h, d1 = (d1 // 16), d1 % 16
+    if h > 0:
+        raise NotImplementedError(
+            "Cell with explicit hash references are not supported yet")
+    s, r = (d1 // 8), d1 % 8
+    if s > 0:
+        raise NotImplementedError("Exoctic cell ware not supported yet")
+    if r > 4:
+        raise NotImplementedError(
+            "Cell with explicit hash references are not supported yet (r>4)")
+    if d2 % 2:
+        data_size = (d2 + 1) // 2
+        not_full = True
+    else:
+        data_size = d2 // 2
+        not_full = False
+    cell_data, ser = ser[:data_size], ser[data_size:]
+    c = Cell()
+    c.data.from_bytes(cell_data, top_upped=not_full)
+    for i in range(r):
+        ref_index, ser = int.from_bytes(
+            ser[:index_size], "big"), ser[index_size:]
+        c.refs.append(ref_index)
+    return c, ser
+
+
 def substitute_indexes_with_cells(cells):
-  for cell in cells[::-1]:
-    for i,r in enumerate(cell.refs):
-      cell.refs[i] = cells[r]
-  return cells
-  
+    for cell in cells[::-1]:
+        for i, r in enumerate(cell.refs):
+            cell.refs[i] = cells[r]
+    return cells
+
 
 def deserialize_boc(boc):
-  bocs_prefixes = [reach_boc_magic_prefix, lean_boc_magic_prefix, lean_boc_magic_prefix_crc]
-  prefix, boc = boc[:4], boc[4:]
-  assert (prefix in bocs_prefixes), "Unknown boc prefix"
-  if prefix == reach_boc_magic_prefix:
-    (has_idx, hash_crc32, has_cache_bits, flags, size_bytes), boc = parse_flags(boc)
-    root_list = True
-  elif prefix == lean_boc_magic_prefix:
-    (has_idx, hash_crc32, has_cache_bits, flags, size_bytes), boc = (1, 0, 0, 0, boc[0]), boc[1:]
-    root_list = False
-  elif prefix == lean_boc_magic_prefix_crc:
-    (has_idx, hash_crc32, has_cache_bits, flags, size_bytes), boc = (1, 1, 0, 0, boc[0]), boc[1:]
-    root_list = False
-  off_bytes, boc = boc[0], boc[1:]
-  cells_num, boc = int.from_bytes(boc[0:size_bytes], "big"), boc[size_bytes:]
-  roots_num, boc = int.from_bytes(boc[0:size_bytes], "big"), boc[size_bytes:]
-  absent_num, boc = int.from_bytes(boc[0:size_bytes], "big"), boc[size_bytes:]
-  assert absent_num == 0
-  tot_cells_size, boc = int.from_bytes(boc[0:off_bytes], "big"), boc[off_bytes:]
-  if root_list:
-    if roots_num > 1:
-      raise NotImplementedError("Only 1 root supported for now (%d)"%roots_num)
-    roots_indexes = []
-    for i in range(roots_num):
-      ri, boc = int.from_bytes(boc[0:size_bytes], "big"), boc[size_bytes:]
-      roots_indexes.append(ri)
-  else:
-    roots_indexes = [0]
-  if has_idx:
-    offsets = []
+    bocs_prefixes = [
+        reach_boc_magic_prefix,
+        lean_boc_magic_prefix,
+        lean_boc_magic_prefix_crc]
+    prefix, boc = boc[:4], boc[4:]
+    assert (prefix in bocs_prefixes), "Unknown boc prefix"
+    if prefix == reach_boc_magic_prefix:
+        (has_idx, hash_crc32, has_cache_bits,
+         flags, size_bytes), boc = parse_flags(boc)
+        root_list = True
+    elif prefix == lean_boc_magic_prefix:
+        (has_idx, hash_crc32, has_cache_bits, flags,
+         size_bytes), boc = (1, 0, 0, 0, boc[0]), boc[1:]
+        root_list = False
+    elif prefix == lean_boc_magic_prefix_crc:
+        (has_idx, hash_crc32, has_cache_bits, flags,
+         size_bytes), boc = (1, 1, 0, 0, boc[0]), boc[1:]
+        root_list = False
+    off_bytes, boc = boc[0], boc[1:]
+    cells_num, boc = int.from_bytes(boc[0:size_bytes], "big"), boc[size_bytes:]
+    roots_num, boc = int.from_bytes(boc[0:size_bytes], "big"), boc[size_bytes:]
+    absent_num, boc = int.from_bytes(
+        boc[0:size_bytes], "big"), boc[size_bytes:]
+    assert absent_num == 0
+    tot_cells_size, boc = int.from_bytes(
+        boc[0:off_bytes], "big"), boc[off_bytes:]
+    if root_list:
+        if roots_num > 1:
+            raise NotImplementedError(
+                "Only 1 root supported for now (%d)" %
+                roots_num)
+        roots_indexes = []
+        for i in range(roots_num):
+            ri, boc = int.from_bytes(
+                boc[0:size_bytes], "big"), boc[size_bytes:]
+            roots_indexes.append(ri)
+    else:
+        roots_indexes = [0]
+    if has_idx:
+        offsets = []
+        for i in range(cells_num):
+            o, boc = int.from_bytes(boc[0:off_bytes], "big"), boc[off_bytes:]
+            offsets.append(o)
+    cells = []
     for i in range(cells_num):
-      o, boc = int.from_bytes(boc[0:off_bytes], "big"), boc[off_bytes:]
-      offset.append(o)
-  cells = []
-  for i in range(cells_num):
-    unfinished_cell, boc = deserialize_cell_data(boc, size_bytes)
-    cells.append(unfinished_cell)
-  cells = substitute_indexes_with_cells(cells)
-  # TODO hash_crc32?
-  return cells[0]
-  
+        unfinished_cell, boc = deserialize_cell_data(boc, size_bytes)
+        cells.append(unfinished_cell)
+    cells = substitute_indexes_with_cells(cells)
+    # TODO hash_crc32?
+    return cells[0]
+
+
 def deserialize_cell_from_object(data):
-  cell = Cell()
-  b64 = data['data']['b64']
-  cell.data.from_bytes( codecs.decode(codecs.encode(b64, 'utf8'), 'base64'))
-  cell.data.data = cell.data.data[:data['data']['len']]
-  for r in data['refs']:
-    cell.refs.append(deserialize_cell_from_object(r))
-  return cell
-  
+    cell = Cell()
+    b64 = data['data']['b64']
+    cell.data.from_bytes(codecs.decode(codecs.encode(b64, 'utf8'), 'base64'))
+    cell.data.data = cell.data.data[:data['data']['len']]
+    for r in data['refs']:
+        cell.refs.append(deserialize_cell_from_object(r))
+    return cell
+
+
 def deserialize_cell_from_json(json_data):
-  return deserialize_cell_from_object(json.loads(json_data))
-  
+    return deserialize_cell_from_object(json.loads(json_data))
+
+
 def test_boc_deserialization():
-  c1 = Cell();
-  c2 = Cell();
-  c3 = Cell();
-  c4 = Cell();
-  c1.data.put_arbitrary_uint(2**25, 26);
-  c2.data.put_arbitrary_uint(2**37, 38); 
-  c3.data.put_arbitrary_uint(2**41, 42); 
-  c4.data.put_arbitrary_uint(2**44-2, 44);  
-  c2.refs.append(c3);
-  c1.refs.append(c2);
-  c1.refs.append(c4);
-  serialized_c1 = c1.serialize_boc(has_idx=False);
-  
-  dc1 = deserialize_boc(serialized_c1)
-  assert dc1.data == c1.data
-  assert dc1.refs[0].data == c2.data
-  assert dc1.refs[1].data == c4.data
-  assert dc1.refs[0].refs[0].data == c3.data
-  
+    c1 = Cell()
+    c2 = Cell()
+    c3 = Cell()
+    c4 = Cell()
+    c1.data.put_arbitrary_uint(2 ** 25, 26)
+    c2.data.put_arbitrary_uint(2 ** 37, 38)
+    c3.data.put_arbitrary_uint(2 ** 41, 42)
+    c4.data.put_arbitrary_uint(2 ** 44 - 2, 44)
+    c2.refs.append(c3)
+    c1.refs.append(c2)
+    c1.refs.append(c4)
+    serialized_c1 = c1.serialize_boc(has_idx=False)
+
+    dc1 = deserialize_boc(serialized_c1)
+    assert dc1.data == c1.data
+    assert dc1.refs[0].data == c2.data
+    assert dc1.refs[1].data == c4.data
+    assert dc1.refs[0].refs[0].data == c3.data
+
 
 def Slice(Cell):
-  def __repr__(self):
-    return "<Slice refs_num: %d, data: %s>"%(len(self.refs), repr(self.data))
-  def __init__(self, cell):
-    self.data = cell.data.copy()
-    self.refs = cell.refs.copy()
+    def __repr__(self):
+        return "<Slice refs_num: %d, data: %s>" % (
+            len(self.refs), repr(self.data))
+
+    def __init__(self, cell):
+        self.data = cell.data.copy()
+        self.refs = cell.refs.copy()
```

## tvm_valuetypes/dict_utils.py

```diff
@@ -1,101 +1,111 @@
 from bitarray import bitarray
 
 
 def read_arbitrary_uint(n, ser):
-  x=0
-  for i in range(n):
-    x <<= 1
-    r = ser.pop(0)
-    x += r
-  return x, ser
+    x = 0
+    for i in range(n):
+        x <<= 1
+        r = ser.pop(0)
+        x += r
+    return x, ser
+
 
 def deser_unary(ser):
-  """
-    unary_zero$0 = Unary ~0;
-    unary_succ$1 {n:#} x:(Unary ~n) = Unary ~(n + 1);
-  """
-  n=0
-  while True:
-    r = ser.pop(0)
-    if r:
-      n+=1
-    else:
-      return n, ser
+    """
+      unary_zero$0 = Unary ~0;
+      unary_succ$1 {n:#} x:(Unary ~n) = Unary ~(n + 1);
+    """
+    n = 0
+    while True:
+        r = ser.pop(0)
+        if r:
+            n += 1
+        else:
+            return n, ser
 
 
 def deser_hmlabel(ser, m):
-  """
-    hml_short$0 {m:#} {n:#} len:(Unary ~n) s:(n * Bit) = HmLabel ~n m;
-    hml_long$10 {m:#} n:(#<= m) s:(n * Bit) = HmLabel ~n m;
-    hml_same$11 {m:#} v:Bit n:(#<= m) = HmLabel ~n m;
-  """
-  _type = ''
-  k = ser.pop(0)
-  s = bitarray()
-  if k:
+    """
+      hml_short$0 {m:#} {n:#} len:(Unary ~n) s:(n * Bit) = HmLabel ~n m;
+      hml_long$10 {m:#} n:(#<= m) s:(n * Bit) = HmLabel ~n m;
+      hml_same$11 {m:#} v:Bit n:(#<= m) = HmLabel ~n m;
+    """
+    _type = ''
     k = ser.pop(0)
+    s = bitarray()
     if k:
-      _type = 'same'
+        k = ser.pop(0)
+        if k:
+            _type = 'same'
+        else:
+            _type = 'long'
+    else:
+        _type = 'short'
+    if _type == 'short':
+        _len, ser = deser_unary(ser)
+        s, ser = ser[:_len], ser[_len:]
+    elif _type == 'long':
+        _len, ser = read_arbitrary_uint(m.bit_length(), ser)
+        s, ser = ser[:_len], ser[_len:]
     else:
-      _type = 'long'
-  else:
-    _type = 'short'
-  if _type == 'short':
-    _len, ser = deser_unary(ser)
-    s, ser = ser[:_len], ser[_len:]
-  elif _type == 'long':
-    _len, ser = read_arbitrary_uint(m.bit_length(), ser)
-    s, ser = ser[:_len], ser[_len:]
-  else:
-    v, ser = ser[0:1], ser[1:]
-    _len, ser = read_arbitrary_uint(m.bit_length(), ser)
-    s = v * _len 
-  return _len, s, ser
+        v, ser = ser[0:1], ser[1:]
+        _len, ser = read_arbitrary_uint(m.bit_length(), ser)
+        s = v * _len
+    return _len, s, ser
 
-def deser_hashmapnode(cell, m, ret_dict, prefix, max_elements):
-  """
-    hmn_leaf#_ {X:Type} value:X = HashmapNode 0 X;
-    hmn_fork#_ {n:#} {X:Type} left:^(Hashmap n X) right:^(Hashmap n X) = HashmapNode (n + 1) X;
-  """
-  if len(ret_dict)>=max_elements:
-    return
-  if m == 0: #leaf
-    ret_dict[prefix.to01()] = cell
-  else: #fork
-    l_prefix, r_prefix = prefix.copy(), prefix.copy()
-    l_prefix.append(False)
-    r_prefix.append(True)
-    parse_hashmap(cell.refs[0].copy(), m-1, ret_dict, l_prefix, max_elements)
-    parse_hashmap(cell.refs[1].copy(), m-1, ret_dict, r_prefix, max_elements)
-
-def parse_hashmap(cell, bitlength, ret_dict, prefix, max_elements = 10000):
-  """
-    hm_edge#_ {n:#} {X:Type} {l:#} {m:#} label:(HmLabel ~l n)
-         {n = (~m) + l} node:(HashmapNode m X) = Hashmap n X;
-  """
-  _len, suffix, cell.data.data = deser_hmlabel(cell.data.data, bitlength)
-  prefix.extend(suffix)
-  m = bitlength - _len
-  deser_hashmapnode(cell.copy(), m, ret_dict, prefix.copy(), max_elements)
-    
 
+def deser_hashmapnode(cell, m, ret_dict, prefix, max_elements):
+    """
+      hmn_leaf#_ {X:Type} value:X = HashmapNode 0 X;
+      hmn_fork#_ {n:#} {X:Type} left:^(Hashmap n X) right:^(Hashmap n X) = HashmapNode (n + 1) X;
+    """
+    if len(ret_dict) >= max_elements:
+        return
+    if m == 0:  # leaf
+        ret_dict[prefix.to01()] = cell
+    else:  # fork
+        l_prefix, r_prefix = prefix.copy(), prefix.copy()
+        l_prefix.append(False)
+        r_prefix.append(True)
+        parse_hashmap(
+            cell.refs[0].copy(),
+            m - 1,
+            ret_dict,
+            l_prefix,
+            max_elements)
+        parse_hashmap(
+            cell.refs[1].copy(),
+            m - 1,
+            ret_dict,
+            r_prefix,
+            max_elements)
+
+
+def parse_hashmap(cell, bitlength, ret_dict, prefix, max_elements=10000):
+    """
+      hm_edge#_ {n:#} {X:Type} {l:#} {m:#} label:(HmLabel ~l n)
+           {n = (~m) + l} node:(HashmapNode m X) = Hashmap n X;
+    """
+    _len, suffix, cell.data.data = deser_hmlabel(cell.data.data, bitlength)
+    prefix.extend(suffix)
+    m = bitlength - _len
+    deser_hashmapnode(cell.copy(), m, ret_dict, prefix.copy(), max_elements)
 
 
 def test_parse_hashmap():
-  test_dict1 = "B5EE9C7241010A01002D00020120010202014803040003FC0202014805060003F5FE02014807080003DB24020120090900035FF800030020CB8CA892"
-  import codecs
-  test_dict1 = codecs.decode(test_dict1, 'hex')
-  from cell import deserialize_boc
-  dict1_cell = deserialize_boc(test_dict1)
-  parsed_dict = {}
-  parse_hashmap(dict1_cell, 8, parsed_dict)
-  print(parsed_dict)
-
-  test_dict1 = "B5EE9C7241010101000B000012A00000006400000001FC00C1D4"
-  test_dict1 = codecs.decode(test_dict1, 'hex')
-  dict1_cell = deserialize_boc(test_dict1)
-  parsed_dict = {}
-  parse_hashmap(dict1_cell, 32, parsed_dict)
-  print(parsed_dict)
-  #assert parsed_dict == {'00000000': bitarray('00000000'), '00000001': bitarray('00000000'), '00000011': bitarray('11111111'), '00001000': bitarray('01100100'), '00111111': bitarray('01111111'), '11111111': bitarray('00000000')} 
-
+    test_dict1 = "B5EE9C7241010A01002D00020120010202014803040003FC0202014805060003F5FE02014807080003DB24020120090900035FF800030020CB8CA892"
+    import codecs
+    test_dict1 = codecs.decode(test_dict1, 'hex')
+    from cell import deserialize_boc
+    dict1_cell = deserialize_boc(test_dict1)
+    parsed_dict = {}
+    parse_hashmap(dict1_cell, 8, parsed_dict)
+    print(parsed_dict)
+
+    test_dict1 = "B5EE9C7241010101000B000012A00000006400000001FC00C1D4"
+    test_dict1 = codecs.decode(test_dict1, 'hex')
+    dict1_cell = deserialize_boc(test_dict1)
+    parsed_dict = {}
+    parse_hashmap(dict1_cell, 32, parsed_dict)
+    # assert parsed_dict == {'00000000': bitarray('00000000'), '00000001': bitarray('00000000'), '00000011': bitarray('11111111'), '00001000': bitarray('01100100'), '00111111': bitarray('01111111'), '11111111': bitarray('00000000')}
+    print(parsed_dict)
```

## tvm_valuetypes/stack_utils.py

```diff
@@ -1,63 +1,91 @@
 import codecs
 
 from .cell import deserialize_boc, Slice, deserialize_cell_from_json
 
+
 def render_tvm_element(element_type, element):
     if element_type in ["num", "number", "int"]:
-      element = str(int(str(element), 0))
-      return {'@type': 'tvm.stackEntryNumber', 'number': {'@type': 'tvm.numberDecimal', 'number': element}}
+        element = str(int(str(element), 0))
+        return {
+            '@type': 'tvm.stackEntryNumber',
+            'number': {
+                '@type': 'tvm.numberDecimal',
+                'number': element}}
     elif element_type == "cell":
-      element = deserialize_cell_from_json(element)
-      element_data = codecs.decode(codecs.encode(element.serialize_boc(has_idx=False), 'base64'), 'utf-8').replace('\n', '')
-      return {'@type': 'tvm.stackEntryCell', 'cell': {'@type': 'tvm.Cell', 'bytes': element_data}}
+        element = deserialize_cell_from_json(element)
+        element_data = codecs.decode(codecs.encode(element.serialize_boc(
+            has_idx=False), 'base64'), 'utf-8').replace('\n', '')
+        return {
+            '@type': 'tvm.stackEntryCell',
+            'cell': {
+                '@type': 'tvm.Cell',
+                'bytes': element_data}}
     elif element_type == "slice":
-      element = deserialize_cell_from_json(element)
-      element_data = codecs.decode(codecs.encode(element.serialize_boc(has_idx=False), 'base64'), 'utf-8').replace('\n', '')
-      return {'@type': 'tvm.stackEntrySlice', 'slice': {'@type': 'tvm.Slice', 'bytes': element_data}}
+        element = deserialize_cell_from_json(element)
+        element_data = codecs.decode(codecs.encode(element.serialize_boc(
+            has_idx=False), 'base64'), 'utf-8').replace('\n', '')
+        return {
+            '@type': 'tvm.stackEntrySlice',
+            'slice': {
+                '@type': 'tvm.Slice',
+                'bytes': element_data}}
     elif element_type == "tvm.Slice":
-      return {'@type': 'tvm.stackEntrySlice', 'slice': {'@type': 'tvm.Slice', 'bytes': element}}
+        return {
+            '@type': 'tvm.stackEntrySlice',
+            'slice': {
+                '@type': 'tvm.Slice',
+                'bytes': element}}
     elif element_type == "tvm.Cell":
-      return {'@type': 'tvm.stackEntryCell', 'cell': {'@type': 'tvm.Cell', 'bytes': element}}
+        return {
+            '@type': 'tvm.stackEntryCell',
+            'cell': {
+                '@type': 'tvm.Cell',
+                'bytes': element}}
     else:
-      raise NotImplemented()
+        raise NotImplemented()
+
 
 def render_tvm_stack(stack_data):
-  """
-    Elements like that are expected:
-    [["num", 300], ["cell", "0x"], ["dict", {...}]]
-    Currently only "num", "cell" and "slice" are supported.
-    To be implemented:
-      T: "list", "tuple", "num", "cell", "slice", "dict", "list"    
-  """
-  stack = []
-  for t in stack_data:
-    stack.append(render_tvm_element(*t))
-  return stack
+    """
+      Elements like that are expected:
+      [["num", 300], ["cell", "0x"], ["dict", {...}]]
+      Currently only "num", "cell" and "slice" are supported.
+      To be implemented:
+        T: "list", "tuple", "num", "cell", "slice", "dict", "list"
+    """
+    stack = []
+    for t in stack_data:
+        stack.append(render_tvm_element(*t))
+    return stack
+
 
 def serialize_tvm_element(t):
-  if not "@type" in t:
-    raise Exception("Not TVM stack element")
-  if t["@type"] == "tvm.stackEntryNumber":
-    return ["num", hex(int(t["number"]["number"]))]
-  elif t["@type"] == "tvm.stackEntrySlice":
-    data = codecs.encode(t["cell"]["bytes"],'utf8')
-    data = codecs.decode(data, 'base64')
-    s = Slice(deserialize_boc(data))
-    return ["cell", {'bytes':t["cell"]["bytes"], 'object':s.serialize_to_object()}]
-  elif t["@type"] == "tvm.stackEntryCell":
-    data = codecs.encode(t["cell"]["bytes"],'utf8')
-    data = codecs.decode(data, 'base64')
-    cell = deserialize_boc(data)
-    return ["cell", {'bytes':t["cell"]["bytes"], 'object':cell.serialize_to_object()}]
-  elif t["@type"] == "tvm.stackEntryTuple":
-    return ["tuple", t["tuple"]]
-  elif t["@type"] == "tvm.stackEntryList":
-    return ["list", t["list"]]
-  else:
-    raise Exception("Unknown type")
+    if "@type" not in t:
+        raise Exception("Not TVM stack element")
+    if t["@type"] == "tvm.stackEntryNumber":
+        return ["num", hex(int(t["number"]["number"]))]
+    elif t["@type"] == "tvm.stackEntrySlice":
+        data = codecs.encode(t["cell"]["bytes"], 'utf8')
+        data = codecs.decode(data, 'base64')
+        s = Slice(deserialize_boc(data))
+        return ["cell", {'bytes': t["cell"]["bytes"],
+                         'object': s.serialize_to_object()}]
+    elif t["@type"] == "tvm.stackEntryCell":
+        data = codecs.encode(t["cell"]["bytes"], 'utf8')
+        data = codecs.decode(data, 'base64')
+        cell = deserialize_boc(data)
+        return ["cell", {'bytes': t["cell"]["bytes"],
+                         'object': cell.serialize_to_object()}]
+    elif t["@type"] == "tvm.stackEntryTuple":
+        return ["tuple", t["tuple"]]
+    elif t["@type"] == "tvm.stackEntryList":
+        return ["list", t["list"]]
+    else:
+        raise Exception("Unknown type")
+
 
 def serialize_tvm_stack(tvm_stack):
-  stack = []
-  for t in tvm_stack:
-    stack.append(serialize_tvm_element(t))
-  return stack
+    stack = []
+    for t in tvm_stack:
+        stack.append(serialize_tvm_element(t))
+    return stack
```

## Comparing `tvm_valuetypes-0.0.8.dist-info/LICENSE` & `tvm_valuetypes-0.0.9.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `tvm_valuetypes-0.0.8.dist-info/METADATA` & `tvm_valuetypes-0.0.9.dist-info/METADATA`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tvm-valuetypes
-Version: 0.0.8
+Version: 0.0.9
 Summary: Collection of utils for handling Telegram Open Network Virtual Machine value types
 Home-page: https://github.com/EmelyanenkoK/tvm_valuetypes
 Author: Emelyanenko Kirill
 Author-email: emelyanenko.kirill@gmail.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
```

## Comparing `tvm_valuetypes-0.0.8.dist-info/RECORD` & `tvm_valuetypes-0.0.9.dist-info/RECORD`

 * *Files 12% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 tvm_valuetypes/__init__.py,sha256=9xchkNUoUptbq83KZGwqMhH5HUu9Nd6HThECVzrkqaA,176
-tvm_valuetypes/cell.py,sha256=meAFtH1K0zwkdjUGJajp-lSORoKrZKytmdBntVk8UrM,12781
-tvm_valuetypes/dict_utils.py,sha256=x9mTno_5bDBaAyttGhD8urlVXy68ql6wmUXJoN_QVJQ,2979
-tvm_valuetypes/stack_utils.py,sha256=XA2HrRMNZQO6hPOiI9Uv3qkgJyY83ap7OQi-a5ePBYU,2671
-tvm_valuetypes-0.0.8.dist-info/LICENSE,sha256=3Yd9_EbxYtaNzGurW_4WbYQ0mROfYQJNJt2c0c0JqOY,1181
-tvm_valuetypes-0.0.8.dist-info/METADATA,sha256=2bwbMpfD2h0S-1qpFk39cyCCWnAxEyRdorhVCE3Uzxk,2177
-tvm_valuetypes-0.0.8.dist-info/WHEEL,sha256=g4nMs7d-Xl9-xC9XovUrsDHGXt-FT0E17Yqo92DEfvY,92
-tvm_valuetypes-0.0.8.dist-info/top_level.txt,sha256=MXNRlqqlRA29VL_IwtG2xVEUoEnntKH8Ijb7yMo7rak,15
-tvm_valuetypes-0.0.8.dist-info/RECORD,,
+tvm_valuetypes/cell.py,sha256=Q3UnV0j3tC_dmH3KNZXJ_Vcs55ivYe4zlabRZYLf6vo,14628
+tvm_valuetypes/dict_utils.py,sha256=Vc7n4pUtbr2HU9uQfsEDKUHNP7Gh7Usg9MSzQ70KjQQ,3336
+tvm_valuetypes/stack_utils.py,sha256=L82OYmHh1EYDHcU_5dPq-UXCAB3k93aY5H_tmvn3aDU,3165
+tvm_valuetypes-0.0.9.dist-info/LICENSE,sha256=3Yd9_EbxYtaNzGurW_4WbYQ0mROfYQJNJt2c0c0JqOY,1181
+tvm_valuetypes-0.0.9.dist-info/METADATA,sha256=jSJIi9Q98KooBTjKtzPV2J0nA8mIJbLxmhPxCbZFIh4,2177
+tvm_valuetypes-0.0.9.dist-info/WHEEL,sha256=g4nMs7d-Xl9-xC9XovUrsDHGXt-FT0E17Yqo92DEfvY,92
+tvm_valuetypes-0.0.9.dist-info/top_level.txt,sha256=MXNRlqqlRA29VL_IwtG2xVEUoEnntKH8Ijb7yMo7rak,15
+tvm_valuetypes-0.0.9.dist-info/RECORD,,
```

