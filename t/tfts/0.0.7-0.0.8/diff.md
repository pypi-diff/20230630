# Comparing `tmp/tfts-0.0.7.tar.gz` & `tmp/tfts-0.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tfts-0.0.7.tar", max compression
+gzip compressed data, was "tfts-0.0.8.tar", max compression
```

## Comparing `tfts-0.0.7.tar` & `tfts-0.0.8.tar`

### file list

```diff
@@ -1,39 +1,39 @@
--rwxr-xr-x   0        0        0     1093 2023-06-19 06:15:21.487797 tfts-0.0.7/LICENSE
--rw-r--r--   0        0        0    10206 2023-06-19 06:15:21.487797 tfts-0.0.7/README.md
--rw-r--r--   0        0        0     2346 2023-06-19 06:15:54.823986 tfts-0.0.7/pyproject.toml
--rw-r--r--   0        0        0      462 2023-06-19 06:15:54.827986 tfts-0.0.7/tfts/__init__.py
--rw-r--r--   0        0        0       20 2023-06-19 06:15:21.491797 tfts-0.0.7/tfts/datasets/__init__.py
--rw-r--r--   0        0        0     3822 2023-06-19 06:15:21.491797 tfts-0.0.7/tfts/datasets/get_data.py
--rw-r--r--   0        0        0       20 2023-06-19 06:15:21.491797 tfts-0.0.7/tfts/features/__init__.py
--rw-r--r--   0        0        0      109 2023-06-19 06:15:21.491797 tfts-0.0.7/tfts/features/ar_feature.py
--rw-r--r--   0        0        0       49 2023-06-19 06:15:21.491797 tfts-0.0.7/tfts/features/time_feature.py
--rw-r--r--   0        0        0       42 2023-06-19 06:15:21.491797 tfts-0.0.7/tfts/features/two_order_feature.py
--rw-r--r--   0        0        0       18 2023-06-19 06:15:21.491797 tfts-0.0.7/tfts/layers/__init__.py
--rw-r--r--   0        0        0     9988 2023-06-19 06:15:21.491797 tfts-0.0.7/tfts/layers/attention_layer.py
--rw-r--r--   0        0        0     5329 2023-06-19 06:15:21.491797 tfts-0.0.7/tfts/layers/autoformer_layer.py
--rw-r--r--   0        0        0     3245 2023-06-19 06:15:21.491797 tfts-0.0.7/tfts/layers/cnn_layer.py
--rw-r--r--   0        0        0     1716 2023-06-19 06:15:21.491797 tfts-0.0.7/tfts/layers/deepar_layer.py
--rw-r--r--   0        0        0     4003 2023-06-19 06:15:21.491797 tfts-0.0.7/tfts/layers/dense_layer.py
--rw-r--r--   0        0        0     8593 2023-06-19 06:15:21.491797 tfts-0.0.7/tfts/layers/embed_layer.py
--rw-r--r--   0        0        0     1408 2023-06-19 06:15:21.491797 tfts-0.0.7/tfts/layers/mask_layer.py
--rw-r--r--   0        0        0     6420 2023-06-19 06:15:21.491797 tfts-0.0.7/tfts/layers/nbeats_layer.py
--rw-r--r--   0        0        0     4081 2023-06-19 06:15:21.491797 tfts-0.0.7/tfts/layers/unet_layer.py
--rw-r--r--   0        0        0       18 2023-06-19 06:15:21.491797 tfts-0.0.7/tfts/models/__init__.py
--rw-r--r--   0        0        0     2064 2023-06-19 06:15:21.491797 tfts-0.0.7/tfts/models/auto_config.py
--rw-r--r--   0        0        0     4263 2023-06-19 06:15:21.491797 tfts-0.0.7/tfts/models/auto_model.py
--rw-r--r--   0        0        0     7507 2023-06-19 06:15:21.491797 tfts-0.0.7/tfts/models/autoformer.py
--rw-r--r--   0        0        0     5721 2023-06-19 06:15:21.491797 tfts-0.0.7/tfts/models/bert.py
--rw-r--r--   0        0        0     1560 2023-06-19 06:15:21.491797 tfts-0.0.7/tfts/models/deepar.py
--rw-r--r--   0        0        0    10357 2023-06-19 06:15:21.491797 tfts-0.0.7/tfts/models/informer.py
--rw-r--r--   0        0        0     2784 2023-06-19 06:15:21.495797 tfts-0.0.7/tfts/models/nbeats.py
--rw-r--r--   0        0        0      123 2023-06-19 06:15:21.495797 tfts-0.0.7/tfts/models/patchtst.py
--rw-r--r--   0        0        0     7429 2023-06-19 06:15:21.495797 tfts-0.0.7/tfts/models/rnn.py
--rw-r--r--   0        0        0    14814 2023-06-19 06:15:21.495797 tfts-0.0.7/tfts/models/seq2seq.py
--rw-r--r--   0        0        0     5513 2023-06-19 06:15:21.495797 tfts-0.0.7/tfts/models/tcn.py
--rw-r--r--   0        0        0      111 2023-06-19 06:15:21.495797 tfts-0.0.7/tfts/models/tide.py
--rw-r--r--   0        0        0    18138 2023-06-19 06:15:21.495797 tfts-0.0.7/tfts/models/transformer.py
--rw-r--r--   0        0        0     4905 2023-06-19 06:15:21.495797 tfts-0.0.7/tfts/models/unet.py
--rw-r--r--   0        0        0    12708 2023-06-19 06:15:21.495797 tfts-0.0.7/tfts/models/wavenet.py
--rw-r--r--   0        0        0    13386 2023-06-19 06:15:21.495797 tfts-0.0.7/tfts/trainer.py
--rw-r--r--   0        0        0      429 2023-06-19 06:15:21.495797 tfts-0.0.7/tfts/tuner.py
--rw-r--r--   0        0        0    11472 1970-01-01 00:00:00.000000 tfts-0.0.7/PKG-INFO
+-rwxr-xr-x   0        0        0     1093 2023-06-30 06:58:42.449126 tfts-0.0.8/LICENSE
+-rw-r--r--   0        0        0    10206 2023-06-30 06:58:42.449126 tfts-0.0.8/README.md
+-rw-r--r--   0        0        0     2346 2023-06-30 06:59:10.849201 tfts-0.0.8/pyproject.toml
+-rw-r--r--   0        0        0      462 2023-06-30 06:59:10.849201 tfts-0.0.8/tfts/__init__.py
+-rw-r--r--   0        0        0       20 2023-06-30 06:58:42.453126 tfts-0.0.8/tfts/datasets/__init__.py
+-rw-r--r--   0        0        0     3822 2023-06-30 06:58:42.453126 tfts-0.0.8/tfts/datasets/get_data.py
+-rw-r--r--   0        0        0       20 2023-06-30 06:58:42.453126 tfts-0.0.8/tfts/features/__init__.py
+-rw-r--r--   0        0        0      109 2023-06-30 06:58:42.453126 tfts-0.0.8/tfts/features/ar_feature.py
+-rw-r--r--   0        0        0       49 2023-06-30 06:58:42.453126 tfts-0.0.8/tfts/features/time_feature.py
+-rw-r--r--   0        0        0       42 2023-06-30 06:58:42.453126 tfts-0.0.8/tfts/features/two_order_feature.py
+-rw-r--r--   0        0        0       18 2023-06-30 06:58:42.453126 tfts-0.0.8/tfts/layers/__init__.py
+-rw-r--r--   0        0        0     9988 2023-06-30 06:58:42.453126 tfts-0.0.8/tfts/layers/attention_layer.py
+-rw-r--r--   0        0        0     5329 2023-06-30 06:58:42.453126 tfts-0.0.8/tfts/layers/autoformer_layer.py
+-rw-r--r--   0        0        0     3245 2023-06-30 06:58:42.453126 tfts-0.0.8/tfts/layers/cnn_layer.py
+-rw-r--r--   0        0        0     1716 2023-06-30 06:58:42.453126 tfts-0.0.8/tfts/layers/deepar_layer.py
+-rw-r--r--   0        0        0     4014 2023-06-30 06:58:42.453126 tfts-0.0.8/tfts/layers/dense_layer.py
+-rw-r--r--   0        0        0     8593 2023-06-30 06:58:42.453126 tfts-0.0.8/tfts/layers/embed_layer.py
+-rw-r--r--   0        0        0     1408 2023-06-30 06:58:42.453126 tfts-0.0.8/tfts/layers/mask_layer.py
+-rw-r--r--   0        0        0     6420 2023-06-30 06:58:42.453126 tfts-0.0.8/tfts/layers/nbeats_layer.py
+-rw-r--r--   0        0        0     4081 2023-06-30 06:58:42.453126 tfts-0.0.8/tfts/layers/unet_layer.py
+-rw-r--r--   0        0        0       18 2023-06-30 06:58:42.453126 tfts-0.0.8/tfts/models/__init__.py
+-rw-r--r--   0        0        0     2064 2023-06-30 06:58:42.453126 tfts-0.0.8/tfts/models/auto_config.py
+-rw-r--r--   0        0        0     4263 2023-06-30 06:58:42.453126 tfts-0.0.8/tfts/models/auto_model.py
+-rw-r--r--   0        0        0     7507 2023-06-30 06:58:42.453126 tfts-0.0.8/tfts/models/autoformer.py
+-rw-r--r--   0        0        0     5717 2023-06-30 06:58:42.453126 tfts-0.0.8/tfts/models/bert.py
+-rw-r--r--   0        0        0     1560 2023-06-30 06:58:42.453126 tfts-0.0.8/tfts/models/deepar.py
+-rw-r--r--   0        0        0    10357 2023-06-30 06:58:42.457126 tfts-0.0.8/tfts/models/informer.py
+-rw-r--r--   0        0        0     2784 2023-06-30 06:58:42.457126 tfts-0.0.8/tfts/models/nbeats.py
+-rw-r--r--   0        0        0      123 2023-06-30 06:58:42.457126 tfts-0.0.8/tfts/models/patchtst.py
+-rw-r--r--   0        0        0     7429 2023-06-30 06:58:42.457126 tfts-0.0.8/tfts/models/rnn.py
+-rw-r--r--   0        0        0    14814 2023-06-30 06:58:42.457126 tfts-0.0.8/tfts/models/seq2seq.py
+-rw-r--r--   0        0        0     5513 2023-06-30 06:58:42.457126 tfts-0.0.8/tfts/models/tcn.py
+-rw-r--r--   0        0        0      111 2023-06-30 06:58:42.457126 tfts-0.0.8/tfts/models/tide.py
+-rw-r--r--   0        0        0    18164 2023-06-30 06:58:42.457126 tfts-0.0.8/tfts/models/transformer.py
+-rw-r--r--   0        0        0     4905 2023-06-30 06:58:42.457126 tfts-0.0.8/tfts/models/unet.py
+-rw-r--r--   0        0        0    12708 2023-06-30 06:58:42.457126 tfts-0.0.8/tfts/models/wavenet.py
+-rw-r--r--   0        0        0    13386 2023-06-30 06:58:42.457126 tfts-0.0.8/tfts/trainer.py
+-rw-r--r--   0        0        0      429 2023-06-30 06:58:42.457126 tfts-0.0.8/tfts/tuner.py
+-rw-r--r--   0        0        0    11472 1970-01-01 00:00:00.000000 tfts-0.0.8/PKG-INFO
```

### Comparing `tfts-0.0.7/LICENSE` & `tfts-0.0.8/LICENSE`

 * *Files identical despite different names*

### Comparing `tfts-0.0.7/README.md` & `tfts-0.0.8/README.md`

 * *Files identical despite different names*

### Comparing `tfts-0.0.7/pyproject.toml` & `tfts-0.0.8/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -25,15 +25,15 @@
 [tool.nbqa.mutate]
 isort = 1
 black = 1
 
 [tool.poetry]
 name = "tfts"
 readme = "README.md"  # Markdown files are supported
-version = "0.0.7"  # is being replaced automatically
+version = "0.0.8"  # is being replaced automatically
 
 authors = ["Longxing Tan"]
 classifiers = [
     "Intended Audience :: Developers",
     "Intended Audience :: Science/Research",
     "Programming Language :: Python :: 3",
     "Programming Language :: Python :: 3.7",
```

### Comparing `tfts-0.0.7/tfts/datasets/get_data.py` & `tfts-0.0.8/tfts/datasets/get_data.py`

 * *Files identical despite different names*

### Comparing `tfts-0.0.7/tfts/layers/attention_layer.py` & `tfts-0.0.8/tfts/layers/attention_layer.py`

 * *Files identical despite different names*

### Comparing `tfts-0.0.7/tfts/layers/autoformer_layer.py` & `tfts-0.0.8/tfts/layers/autoformer_layer.py`

 * *Files identical despite different names*

### Comparing `tfts-0.0.7/tfts/layers/cnn_layer.py` & `tfts-0.0.8/tfts/layers/cnn_layer.py`

 * *Files identical despite different names*

### Comparing `tfts-0.0.7/tfts/layers/deepar_layer.py` & `tfts-0.0.8/tfts/layers/deepar_layer.py`

 * *Files identical despite different names*

### Comparing `tfts-0.0.7/tfts/layers/dense_layer.py` & `tfts-0.0.8/tfts/layers/dense_layer.py`

 * *Files 0% similar despite different names*

```diff
@@ -84,15 +84,15 @@
     def build(self, input_shape):
         self.filter_dense_layer = Dense(self.filter_size, use_bias=True, activation="relu")
         self.output_dense_layer = Dense(self.hidden_size, use_bias=True)
         self.drop = Dropout(self.relu_dropout)
         super(FeedForwardNetwork, self).build(input_shape)
 
     def call(self, x):
-        """_summary_
+        """Feed Forward Network
 
         Parameters
         ----------
         x : _type_
             _description_
 
         Returns
```

### Comparing `tfts-0.0.7/tfts/layers/embed_layer.py` & `tfts-0.0.8/tfts/layers/embed_layer.py`

 * *Files identical despite different names*

### Comparing `tfts-0.0.7/tfts/layers/mask_layer.py` & `tfts-0.0.8/tfts/layers/mask_layer.py`

 * *Files identical despite different names*

### Comparing `tfts-0.0.7/tfts/layers/nbeats_layer.py` & `tfts-0.0.8/tfts/layers/nbeats_layer.py`

 * *Files identical despite different names*

### Comparing `tfts-0.0.7/tfts/layers/unet_layer.py` & `tfts-0.0.8/tfts/layers/unet_layer.py`

 * *Files identical despite different names*

### Comparing `tfts-0.0.7/tfts/models/auto_config.py` & `tfts-0.0.8/tfts/models/auto_config.py`

 * *Files identical despite different names*

### Comparing `tfts-0.0.7/tfts/models/auto_model.py` & `tfts-0.0.8/tfts/models/auto_model.py`

 * *Files identical despite different names*

### Comparing `tfts-0.0.7/tfts/models/autoformer.py` & `tfts-0.0.8/tfts/models/autoformer.py`

 * *Files identical despite different names*

### Comparing `tfts-0.0.7/tfts/models/bert.py` & `tfts-0.0.8/tfts/models/bert.py`

 * *Files 0% similar despite different names*

```diff
@@ -111,15 +111,15 @@
             encoder_feature = x = inputs
 
         encoder_feature = self.encoder_embedding(encoder_feature)
         # encoder_features = self.spatial_drop(encoder_features)
         # encoder_features_res = self.tcn(encoder_features)
         # encoder_features += encoder_features_res
 
-        memory = self.encoder(encoder_feature, src_mask=None)  # batch * train_sequence * (hidden * heads)
+        memory = self.encoder(encoder_feature, mask=None)  # batch * train_sequence * (hidden * heads)
         encoder_output = memory[:, -1]
 
         # encoder_output = self.bn1(encoder_output)
         encoder_output = self.drop1(encoder_output)
         encoder_output = self.dense1(encoder_output)
         # encoder_output = self.bn2(encoder_output)
         encoder_output = self.drop2(encoder_output)
```

### Comparing `tfts-0.0.7/tfts/models/deepar.py` & `tfts-0.0.8/tfts/models/deepar.py`

 * *Files identical despite different names*

### Comparing `tfts-0.0.7/tfts/models/informer.py` & `tfts-0.0.8/tfts/models/informer.py`

 * *Files identical despite different names*

### Comparing `tfts-0.0.7/tfts/models/nbeats.py` & `tfts-0.0.8/tfts/models/nbeats.py`

 * *Files identical despite different names*

### Comparing `tfts-0.0.7/tfts/models/rnn.py` & `tfts-0.0.8/tfts/models/rnn.py`

 * *Files identical despite different names*

### Comparing `tfts-0.0.7/tfts/models/seq2seq.py` & `tfts-0.0.8/tfts/models/seq2seq.py`

 * *Files identical despite different names*

### Comparing `tfts-0.0.7/tfts/models/tcn.py` & `tfts-0.0.8/tfts/models/tcn.py`

 * *Files identical despite different names*

### Comparing `tfts-0.0.7/tfts/models/transformer.py` & `tfts-0.0.8/tfts/models/transformer.py`

 * *Files 0% similar despite different names*

```diff
@@ -111,15 +111,15 @@
                     tf.reshape(tf.range(self.predict_sequence_length), (1, self.predict_sequence_length, 1)),
                     (tf.shape(encoder_feature)[0], 1, 1),
                 ),
                 tf.float32,
             )
 
         encoder_feature = self.encoder_embedding(encoder_feature)  # batch * seq * embedding_size
-        memory = self.encoder(encoder_feature, src_mask=None)
+        memory = self.encoder(encoder_feature, mask=None)
 
         # decoder_outputs = self.decoder(decoder_features, init_input=x[:, -1:], encoder_memory=memory, teacher=teacher)
 
         B, L, _ = tf.shape(decoder_feature)
         casual_mask = CausalMask(B * self.params["num_heads"], L).mask
         decoder_outputs = self.decoder(decoder_feature, memory, x_mask=casual_mask)
         decoder_outputs = self.project(decoder_outputs)
@@ -159,36 +159,36 @@
             attention_layer = SelfAttention(self.attention_hidden_sizes, self.num_heads, self.attention_dropout)
             feed_forward_layer = FeedForwardNetwork(self.ffn_hidden_sizes, self.ffn_filter_sizes, self.ffn_dropout)
             ln_layer1 = LayerNormalization(epsilon=1e-6, dtype="float32")
             ln_layer2 = LayerNormalization(epsilon=1e-6, dtype="float32")
             self.layers.append([attention_layer, ln_layer1, feed_forward_layer, ln_layer2])
         super(Encoder, self).build(input_shape)
 
-    def call(self, encoder_inputs, src_mask=None):
+    def call(self, inputs, mask=None):
         """Transformer encoder
 
         Parameters
         ----------
-        encoder_inputs : _type_
-            _description_
-        src_mask : _type_, optional
+        inputs : tf.Tensor
+            Transformer encoder inputs, with dimension of (batch, seq_len, features)
+        mask : tf.Tensor, optional
             _description_, by default None
 
         Returns
         -------
-        _type_
+        tf.Tensor
             _description_
         """
-        x = encoder_inputs
+        x = inputs
         for _, layer in enumerate(self.layers):
             attention_layer, ln_layer1, ffn_layer, ln_layer2 = layer
             enc = x
-            enc = attention_layer(enc, src_mask)
-            enc1 = ln_layer1(x + enc)  # residual connect
-            enc1 = ffn_layer(enc1)
+            enc = attention_layer(enc, mask)
+            enc = ln_layer1(x + enc)  # residual connect
+            enc1 = ffn_layer(enc)
             x = ln_layer2(enc + enc1)
         return x
 
     def get_config(self):
         config = {
             "n_encoder_layers": self.n_encoder_layers,
             "attention_hidden_sizes": self.attention_hidden_sizes,
@@ -347,16 +347,16 @@
 
         for _, layer in enumerate(self.layers):
             self_attention_layer, enc_dec_attention_layer, ffn_layer, ln_layer1, ln_layer2, ln_layer3 = layer
             dec = x
             dec = self_attention_layer(dec, mask=tgt_mask)
             dec1 = ln_layer1(x + dec)
             dec1 = enc_dec_attention_layer(dec1, encoder_memory, encoder_memory, mask=cross_mask)
-            dec2 = ln_layer2(dec + dec1)
-            dec2 = ffn_layer(dec2)
+            dec1 = ln_layer2(dec + dec1)
+            dec2 = ffn_layer(dec1)
             x = ln_layer3(dec1 + dec2)
         return x
 
     def get_config(self):
         config = {
             "n_decoder_layers": self.n_decoder_layers,
             "attention_hidden_sizes": self.attention_hidden_sizes,
```

### Comparing `tfts-0.0.7/tfts/models/unet.py` & `tfts-0.0.8/tfts/models/unet.py`

 * *Files identical despite different names*

### Comparing `tfts-0.0.7/tfts/models/wavenet.py` & `tfts-0.0.8/tfts/models/wavenet.py`

 * *Files identical despite different names*

### Comparing `tfts-0.0.7/tfts/trainer.py` & `tfts-0.0.8/tfts/trainer.py`

 * *Files identical despite different names*

### Comparing `tfts-0.0.7/PKG-INFO` & `tfts-0.0.8/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tfts
-Version: 0.0.7
+Version: 0.0.8
 Summary: Deep learning time series with TensorFlow
 Home-page: https://time-series-prediction.readthedocs.io
 Author: Longxing Tan
 Requires-Python: >=3.7.1,<3.11
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: MIT License
```

