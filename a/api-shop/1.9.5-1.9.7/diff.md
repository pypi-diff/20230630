# Comparing `tmp/api-shop-1.9.5.tar.gz` & `tmp/api-shop-1.9.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\api-shop-1.9.5.tar", last modified: Thu Sep  5 13:35:18 2019, max compression
+gzip compressed data, was "dist\api-shop-1.9.7.tar", last modified: Tue Oct 22 08:23:10 2019, max compression
```

## Comparing `api-shop-1.9.5.tar` & `api-shop-1.9.7.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxrwxrwx   0        0        0        0 2019-09-05 13:35:17.000000 api-shop-1.9.5/
-drwxrwxrwx   0        0        0        0 2019-09-05 13:35:17.000000 api-shop-1.9.5/api_shop/
--rw-rw-rw-   0        0        0    26791 2019-09-04 13:29:38.000000 api-shop-1.9.5/api_shop/api_shop.py
--rw-rw-rw-   0        0        0     4221 2019-03-14 12:24:55.000000 api-shop-1.9.5/api_shop/autofill.py
--rw-rw-rw-   0        0        0      569 2019-09-03 14:53:34.000000 api-shop-1.9.5/api_shop/data_format.py
--rw-rw-rw-   0        0        0     2957 2019-09-03 14:53:34.000000 api-shop-1.9.5/api_shop/i18n.py
-drwxrwxrwx   0        0        0        0 2019-09-05 13:35:17.000000 api-shop-1.9.5/api_shop/static/
--rw-rw-rw-   0        0        0    26845 2019-09-05 13:31:00.000000 api-shop-1.9.5/api_shop/static/document.html
--rw-rw-rw-   0        0        0     1353 2019-03-09 14:26:15.000000 api-shop-1.9.5/api_shop/url_parse.py
--rw-rw-rw-   0        0        0       69 2019-09-05 13:33:58.000000 api-shop-1.9.5/api_shop/__init__.py
-drwxrwxrwx   0        0        0        0 2019-09-05 13:35:17.000000 api-shop-1.9.5/api_shop.egg-info/
--rw-rw-rw-   0        0        0        1 2019-09-05 13:35:16.000000 api-shop-1.9.5/api_shop.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0     2783 2019-09-05 13:35:16.000000 api-shop-1.9.5/api_shop.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      315 2019-09-05 13:35:17.000000 api-shop-1.9.5/api_shop.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        9 2019-09-05 13:35:16.000000 api-shop-1.9.5/api_shop.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       66 2019-01-30 12:30:29.000000 api-shop-1.9.5/MANIFEST.in
--rw-rw-rw-   0        0        0     2783 2019-09-05 13:35:17.000000 api-shop-1.9.5/PKG-INFO
--rw-rw-rw-   0        0        0     1573 2019-09-05 13:31:37.000000 api-shop-1.9.5/README.rst
--rw-rw-rw-   0        0        0       42 2019-09-05 13:35:17.000000 api-shop-1.9.5/setup.cfg
--rw-rw-rw-   0        0        0     1575 2019-09-03 14:53:34.000000 api-shop-1.9.5/setup.py
+drwxrwxrwx   0        0        0        0 2019-10-22 08:23:10.000000 api-shop-1.9.7/
+drwxrwxrwx   0        0        0        0 2019-10-22 08:23:10.000000 api-shop-1.9.7/api_shop/
+-rw-rw-rw-   0        0        0    27014 2019-10-22 08:19:41.000000 api-shop-1.9.7/api_shop/api_shop.py
+-rw-rw-rw-   0        0        0     4221 2019-03-14 03:04:33.000000 api-shop-1.9.7/api_shop/autofill.py
+-rw-rw-rw-   0        0        0      569 2019-05-07 09:15:36.000000 api-shop-1.9.7/api_shop/data_format.py
+-rw-rw-rw-   0        0        0     2957 2019-05-07 06:33:56.000000 api-shop-1.9.7/api_shop/i18n.py
+drwxrwxrwx   0        0        0        0 2019-10-22 08:23:10.000000 api-shop-1.9.7/api_shop/static/
+-rw-rw-rw-   0        0        0    26497 2019-10-22 08:01:57.000000 api-shop-1.9.7/api_shop/static/document.html
+-rw-rw-rw-   0        0        0     1353 2019-03-06 08:03:54.000000 api-shop-1.9.7/api_shop/url_parse.py
+-rw-rw-rw-   0        0        0       69 2019-10-22 08:20:04.000000 api-shop-1.9.7/api_shop/__init__.py
+drwxrwxrwx   0        0        0        0 2019-10-22 08:23:10.000000 api-shop-1.9.7/api_shop.egg-info/
+-rw-rw-rw-   0        0        0        1 2019-10-22 08:23:09.000000 api-shop-1.9.7/api_shop.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0     2804 2019-10-22 08:23:09.000000 api-shop-1.9.7/api_shop.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      315 2019-10-22 08:23:09.000000 api-shop-1.9.7/api_shop.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        9 2019-10-22 08:23:09.000000 api-shop-1.9.7/api_shop.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       66 2019-02-11 00:44:23.000000 api-shop-1.9.7/MANIFEST.in
+-rw-rw-rw-   0        0        0     2804 2019-10-22 08:23:10.000000 api-shop-1.9.7/PKG-INFO
+-rw-rw-rw-   0        0        0     1573 2019-09-06 00:41:29.000000 api-shop-1.9.7/README.rst
+-rw-rw-rw-   0        0        0       42 2019-10-22 08:23:10.000000 api-shop-1.9.7/setup.cfg
+-rw-rw-rw-   0        0        0     1575 2019-06-27 03:01:34.000000 api-shop-1.9.7/setup.py
```

### Comparing `api-shop-1.9.5/api_shop/api_shop.py` & `api-shop-1.9.7/api_shop/api_shop.py`

 * *Files 2% similar despite different names*

```diff
@@ -156,15 +156,19 @@
             
 
 api = ApiInit()
 
 
 
 class ApiDataClass(Namespace):
-    pass
+    '''api-data类'''
+    def __init__(self, data=None):
+        if data:
+            self.update(data)
+
     def dict(self):
         return self.__dict__
     
     def to_dict(self):
         return self.__dict__
 
     def get_json(self):
@@ -219,26 +223,24 @@
     api_class 是业务api类的对象（不是实例）
     method 是请求方法,str格式
     data 是附加数据，dict格式
     request=None 是当前request，业务代码如果不使用，可以不传递
     not200=True 是允许status_code不等于200的结果，为False的时候，遇到200以外程序中断并抛错
     返回值是 response
     '''
-    d_ = ApiDataClass()
-    if data:
-        d_.update(data)
+    d_ = ApiDataClass(data)
 
     fw = api.get('framework')
     fwname = fw.get('name')
 
     if request:
         if request.method != method:
             raise BaseException(_('request.method and method are not equal'))
     else:
-        request = ApiDataClass()
+        request = ApiDataClass(data)
         request.method = method
     
     
     tup = api_class(request,d_)
 
     if type(tup) == tuple:
         status_code = tup[1]
@@ -416,16 +418,14 @@
                 traceback.print_exc()
                 if auto_fill(thisconf, self.options) == True:
                     # 自动生成文件或者方法，成功后重试一次。
                     return self.__dynamic_import(thisconf)
                 else:
                     os._exit(0)
 
-            
-
     def __make_model(self, conf):
         # 将字符串里的function模块和函数加载进来，并写入到run_function字段方便调用。
         for i in range(len(conf)):
             # model = dynamic_import(conf[i]['class'])
             model = self.__dynamic_import(conf[i])
             if type(conf[i]['class'])!=str:
                 # 直接使用对象
@@ -463,15 +463,14 @@
 
         return conf
 
     def __not_find_url_function(self, request):
         # 如果找不到业务模块
         return return_response(_('no such interface'))
 
-
     def __find_api_function(self, url):
         # 查找api所指向的模块
         if (type(url) == tuple and len(url) > 0):
             key, value_dict = self.__find_url_rule(url[0])
             model = self.url_dict.get(key)
             if model:
                 return model,key,value_dict
@@ -502,15 +501,14 @@
             if url_:
                 # 有剩余url，表示该行不匹配
                 continue
             else:
                 return key, value_dict
         return None,None
 
-
     def __init_url_rules(self):
         # _converter_args_re = re.compile(r'''
         #     ((?P<name>\w+)\s*=\s*)?
         #     (?P<value>
         #         True|False|
         #         \d+.\d+|
         #         \d+.|
@@ -545,15 +543,14 @@
                         })
                 index = index + 1
             self.rule_maps.append({
                 'line': this_rule,
                 'key':rule
             })
     
-
     def get_parameter(self, request):
         # 获取参数
         data = {}
         # 获取django的request数据
         if api.framework.name =='django':
             if request.GET:
                 data.update(request.GET.dict())
@@ -586,16 +583,15 @@
                 data.update(request.GET)
             if request.POST:
                 data.update(request.POST)
             if request.json:
                 data.update(request.json)
 
         return data
-
-        
+      
     def __verify(self, conf, name, value):
         # 校验数据并转换格式
         required_ = conf.get('required')
         type_ = conf.get('type')
         min_ = conf.get('min')
         max_ = conf.get('max')
         default_ = conf.get('default')
@@ -611,20 +607,25 @@
             else:
                 value = default_
 
          # 检查必要值
         if required_ == True and not value and value!=0:
             return _('parameter')+' {} '.format(name)+_('is required'), None
 
+        if value == '' and type_ != str:
+            # 如果是空字符串，但是要求类型不是字符串，就转换成None
+            value = None
+            
         # 检查空值，这个时候因为有些空值还处于字符串形态，比如'[]'，所以有可能会被跳过        
         if not value and value != 0:
             if required_:
                 return _('parameter')+' {} '.format(name)+_('can not be empty'), None,
             else:
                 return None, value
+        
             
         # 检查并转换类型
         if not_converting==False and type_ and type(value) != type_:
             try:
                 if type_ in [list, dict, set, tuple]:
                     # 容器类，json验证后转换
                     value = type_(json.loads(value))
@@ -716,15 +717,13 @@
 
     def render_documents(self,request,*url):
         '''渲染文档'''
         if self.document_version != time.ctime(os.stat(self.document_name).st_mtime):
             # 如果文档发生变化，读取文档。
             self.document = open(self.document_name, mode='r', encoding='utf-8').read()
         return api.framework.template(self.document)
-
-
  
     def get_api_data(self, request, *url):
         '''返回给文档页面数据'''
         return api.framework.json({'data': self.conf,'options':self.options})
```

### Comparing `api-shop-1.9.5/api_shop/autofill.py` & `api-shop-1.9.7/api_shop/autofill.py`

 * *Files identical despite different names*

### Comparing `api-shop-1.9.5/api_shop/data_format.py` & `api-shop-1.9.7/api_shop/data_format.py`

 * *Files identical despite different names*

### Comparing `api-shop-1.9.5/api_shop/i18n.py` & `api-shop-1.9.7/api_shop/i18n.py`

 * *Files identical despite different names*

### Comparing `api-shop-1.9.5/api_shop/static/document.html` & `api-shop-1.9.7/api_shop/static/document.html`

 * *Files 0% similar despite different names*

```diff
@@ -148,31 +148,33 @@
                             <i class="el-icon-document" style="font-size: 18px;color: #000;"></i>
                         </a>
                         <a href="https://github.com/pcloth/api-shop" target="_blank"
                             :title="_('Access code repository')"><span class="iconfont icon-github"></span></a>
                     </h4>
                     <h5>{{_('api count')}}: {{apiList.length}}</h5>
                     <div class="api-list">
-                        <div class="row-title" >
+                        <div class="row-title">
                             <el-autocomplete style="width: 100%" v-model="state" :fetch-suggestions="querySearch"
                                 :placeholder="_('research all')" :trigger-on-focus="false" @select="handleSelect">
                                 <template slot="prepend"><i class="el-icon-search"></i></template>
                             </el-autocomplete>
                         </div>
                         <div class="row-title">
                             <div class="col">
-                                <el-select  style="width: 100%" v-model="seleledName" allow-create filterable placeholder="请选择">
+                                <el-select style="width: 100%" v-model="seleledName" allow-create filterable
+                                    placeholder="请选择">
                                     <el-option :label="_('Name')" value=""></el-option>
                                     <el-option v-for="item in name_type" :key="`name-type-${item.value}`"
                                         v-if="item.text" :label="item.text" :value="item.value">
                                     </el-option>
                                 </el-select>
                             </div>
                             <div class="col">
-                                <el-select  style="width: 100%" v-model="seleledUrl" allow-create filterable placeholder="请选择">
+                                <el-select style="width: 100%" v-model="seleledUrl" allow-create filterable
+                                    placeholder="请选择">
                                     <el-option :label="_('Url')" value=""></el-option>
                                     <el-option v-for="item in url_type" :key="`url-type-${item.value}`" v-if="item.text"
                                         :label="item.text" :value="item.value">
                                     </el-option>
                                 </el-select>
                             </div>
                         </div>
@@ -225,19 +227,19 @@
             'minimum': '最小值/长度',
             'maximum': '最大值/长度',
             'test value': '测试值',
             'description': '描述',
             'Mock Test': '模拟测试',
             'default': '默认值',
             'options': '可选项',
-            'research all':'全文搜索',
-            'send mock request:':'发送模拟请求：',
-            'response':'response响应',
-            'Prompt message':'提示信息',
-            'Please press F12 to check the delivery status.':'请按下F12查看发送情况。'
+            'research all': '全文搜索',
+            'send mock request:': '发送模拟请求：',
+            'response': 'response响应',
+            'Prompt message': '提示信息',
+            'Please press F12 to check the delivery status.': '请按下F12查看发送情况。'
 
         },
         en: {
             'api count': 'api count',
             'View api-shop documentation': 'View api-shop documentation',
             'Name': 'Name',
             'Url': 'Url',
@@ -252,22 +254,22 @@
             'minimum': 'minimum',
             'maximum': 'maximum',
             'test value': 'test value',
             'description': 'description',
             'Mock Test': 'Mock Test',
             'default': 'default',
             'options': 'options',
-            'research all':'research all'
+            'research all': 'research all'
         }
     }
 
 
     const interface = {
         name: 'interface',
-            template: `<el-row><el-row v-if="currentApi">\
+        template: `<el-row><el-row v-if="currentApi">\
             <div class="flex-row">\
                 <div class="flex-row-title">{{_('Name')}} </div>\
                 <div class="flex-row-content">\
                     <el-input readonly v-model="currentApi.name">\
                     </el-input>\
                 </div>\
             </div>\
@@ -355,139 +357,140 @@
                                     </el-table-column>\
                                 </el-table>\
                             </div>\
                         </div>\
                 </el-tab-pane>\
             </el-tabs>\
         </el-row></el-row>`,
-            props: ['idx'],
+        props: ['idx'],
 
-            data() {
-                return {
-                    // test: '',
-                    currentApi: {},
-                    testData: {},
-                    ttt: 0,
+        data() {
+            return {
+                // test: '',
+                currentApi: {},
+                testData: {},
+                ttt: 0,
 
-                    // i18n:i18n
-                }
+                // i18n:i18n
+            }
+        },
+        watch: {
+            '$route'(to, from) {
+                this.readApi();
+            }
+        },
+        computed: {
+            // 计算属性的 getter
+            testString() {
+                return JSON.stringify(this.testData);
             },
-            watch: {
-                '$route'(to, from) {
-                    this.readApi();
-                }
+            apiList() {
+                return data.apiList;
             },
-            computed: {
-                // 计算属性的 getter
-                testString() {
-                    return JSON.stringify(this.testData);
-                },
-                apiList() {
-                    return data.apiList;
-                },
-
-                options() {
-                    return data.options;
-                },
-                baseUrl() {
-                    return data.baseUrl;
-                },
-                // name_type() {
-                //     return data.name_type;
-                // },
-                // url_type() {
-                //     return data.url_type;
-                // },
+
+            options() {
+                return data.options;
             },
-            mounted() {
-                this.readApi();
+            baseUrl() {
+                return data.baseUrl;
             },
-            methods: {
-                _(text) {
-                    let lang = data.options.lang ? data.options.lang : 'en'
-                    return i18n[lang][text] ? i18n[lang][text] : text;
-                },
-                readApi() {
-                    if (!data.apiList || data.apiList.length == 0) {
-                        setTimeout(this.readApi, 500);
-                    }
-                    this.testData = Mock.mock({
-                        "string|1-10": "★"
-                    });
-                    this.currentApi = data.apiList[this.idx];
-                    this.activeName = '0'
-                },
-                mockTest(method, key) {
-                    let api_url = ''
-                    if (typeof this.currentApi.url === 'string') {
-                        api_url = this.currentApi.url
+            // name_type() {
+            //     return data.name_type;
+            // },
+            // url_type() {
+            //     return data.url_type;
+            // },
+        },
+        mounted() {
+            this.readApi();
+        },
+        methods: {
+            _(text) {
+                let lang = data.options.lang ? data.options.lang : 'en'
+                return i18n[lang][text] ? i18n[lang][text] : text;
+            },
+            readApi() {
+                if (!data.apiList || data.apiList.length == 0) {
+                    setTimeout(this.readApi, 500);
+                }
+                this.testData = Mock.mock({
+                    "string|1-10": "★"
+                });
+                this.currentApi = data.apiList[this.idx];
+                this.activeName = '0'
+            },
+            mockTest(method, key) {
+                let api_url = ''
+                if (typeof this.currentApi.url === 'string') {
+                    api_url = this.currentApi.url
 
+                } else {
+                    api_url = this.currentApi.url[0]
+
+                }
+                let url = this.options.base_url + api_url;
+                this.$alert(this._('Please press F12 to check the delivery status.'), this._('Prompt message'))
+                let mapping = {
+                    str: '@string',
+                    int: '@integer',
+                    float: '@float',
+                    bool: '@boolean',
+                    list: '@range',
+                    set: '@range',
+                    "api_shop.data_format.datetime": '@datetime'
+                }
+                let mockConf = {}
+                for (let i in method) {
+
+                    if (method[i].value) {
+                        mockConf[method[i].name] = method[i].value;
+                    } else if (!method[i].required) {
+                        continue;
                     } else {
-                        api_url = this.currentApi.url[0]
+                        let min = method[i].min ? method[i].min : 1;
+                        let max = method[i].max ? method[i].max : 20;
+                        let length = getRandomInt(min, max);
+                        let val = mapping[method[i].type] ? mapping[method[i].type] : '@character'
+                        if (method[i].type == 'list' || method[i].type == 'set') val = `${val}(${length})`;
+                        if (method[i].type == 'str') val = `${val}("lower",${length})`;
+                        if (method[i].type == 'int' || method[i].type == 'float') val = `${val}(${min},${max})`;
+                        mockConf[method[i].name] = Mock.mock(val);
 
                     }
-                    let url = this.options.base_url + api_url;
-                    this.$alert(this._('Please press F12 to check the delivery status.'), this._('Prompt message'))
-                    let mapping = {
-                        str: '@string',
-                        int: '@integer',
-                        float: '@float',
-                        bool: '@boolean',
-                        list: '@range',
-                        set: '@range',
-                        "api_shop.data_format.datetime": '@datetime'
+
+                    if (mockConf[method[i].name] && url.indexOf(`<${method[i].name}>`) >= 0) {
+                        // console.log(method[i].name,mockConf[method[i].name])
+                        url = url.replace(`<${method[i].name}>`, mockConf[method[i].name])
+                        // console.log(url)
+                        mockConf[method[i].name] = undefined
                     }
-                    let mockConf = {}
-                    for (let i in method) {
 
-                        if (method[i].value) {
-                            mockConf[method[i].name] = method[i].value;
-                        } else if (!method[i].required) {
-                            continue;
-                        } else {
-                            let min = method[i].min ? method[i].min : 1;
-                            let max = method[i].max ? method[i].max : 20;
-                            let length = getRandomInt(min, max);
-                            let val = mapping[method[i].type] ? mapping[method[i].type] : '@character'
-                            if (method[i].type == 'list' || method[i].type == 'set') val = `${val}(${length})`;
-                            if (method[i].type == 'str') val = `${val}("lower",${length})`;
-                            if (method[i].type == 'int' || method[i].type == 'float') val = `${val}(${min},${max})`;
-                            mockConf[method[i].name] = Mock.mock(val);
-
-                        }
-
-                        if (mockConf[method[i].name] && url.indexOf(`<${method[i].name}>`) >= 0) {
-                            // console.log(method[i].name,mockConf[method[i].name])
-                            url = url.replace(`<${method[i].name}>`, mockConf[method[i].name])
-                            // console.log(url)
-                            mockConf[method[i].name] = undefined
-                        }
 
-                    }
-                    console.info(this._('send mock request:'),key, mockConf)
+                }
+                console.info(this._('send mock request:'), key, mockConf)
 
-                    if (key == 'GET' || key == 'DELETE') mockConf = {
-                        params: mockConf
-                    };
-
-                    axios[key.toLowerCase()](url, mockConf).then(res => {
-                        console.info(this._('response:'),res);
-                    }).catch(error => {
-                        console.error(error);
-                    })
+                if (key == 'GET' || key == 'DELETE') mockConf = {
+                    params: mockConf
+                };
+
+                axios[key.toLowerCase()](url, mockConf).then(res => {
+                    console.info(this._('response:'), res);
+                }).catch(error => {
+                    console.error(error);
+                })
 
-                },
             },
+        },
     }
 
     const routes = [{
         path: '/interface/:idx',
         component: interface,
         props: true
-    }, ]
+    },]
 
 
     const router = new VueRouter({
         routes
     })
 
     function getRandomInt(min, max) {
```

### Comparing `api-shop-1.9.5/api_shop/url_parse.py` & `api-shop-1.9.7/api_shop/url_parse.py`

 * *Files identical despite different names*

### Comparing `api-shop-1.9.5/api_shop.egg-info/PKG-INFO` & `api-shop-1.9.7/api_shop.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,16 +1,17 @@
-Metadata-Version: 1.1
+Metadata-Version: 1.2
 Name: api-shop
-Version: 1.9.5
+Version: 1.9.7
 Summary: RESTful api shop for django or flask or bottle
 Home-page: https://github.com/pcloth/api-shop
 Author: pcloth
 Author-email: pcloth@gmail.com
+Maintainer: pcloth
+Maintainer-email: pcloth@gmail.com
 License: BSD License
-Description-Content-Type: UNKNOWN
 Description: api-shop v1.9.5
         ===============
         
         `Online Documents <https://pcloth.github.io/api-shop/index.html>`_
         ------------------------------------------------------------------
         
         api-shop：一个易用的、快速的restful-api接口工具包，兼容：django / flask / bottle
```

### Comparing `api-shop-1.9.5/PKG-INFO` & `api-shop-1.9.7/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,16 +1,17 @@
-Metadata-Version: 1.1
+Metadata-Version: 1.2
 Name: api-shop
-Version: 1.9.5
+Version: 1.9.7
 Summary: RESTful api shop for django or flask or bottle
 Home-page: https://github.com/pcloth/api-shop
 Author: pcloth
 Author-email: pcloth@gmail.com
+Maintainer: pcloth
+Maintainer-email: pcloth@gmail.com
 License: BSD License
-Description-Content-Type: UNKNOWN
 Description: api-shop v1.9.5
         ===============
         
         `Online Documents <https://pcloth.github.io/api-shop/index.html>`_
         ------------------------------------------------------------------
         
         api-shop：一个易用的、快速的restful-api接口工具包，兼容：django / flask / bottle
```

### Comparing `api-shop-1.9.5/README.rst` & `api-shop-1.9.7/README.rst`

 * *Files identical despite different names*

### Comparing `api-shop-1.9.5/setup.py` & `api-shop-1.9.7/setup.py`

 * *Files identical despite different names*

