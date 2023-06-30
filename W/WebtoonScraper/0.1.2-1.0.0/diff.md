# Comparing `tmp/WebtoonScraper-0.1.2.tar.gz` & `tmp/WebtoonScraper-1.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "WebtoonScraper-0.1.2.tar", last modified: Sun Jun 25 12:35:24 2023, max compression
+gzip compressed data, was "WebtoonScraper-1.0.0.tar", last modified: Thu Jun 29 13:18:59 2023, max compression
```

## Comparing `WebtoonScraper-0.1.2.tar` & `WebtoonScraper-1.0.0.tar`

### file list

```diff
@@ -1,28 +1,29 @@
-drwxrwxrwx   0        0        0        0 2023-06-25 12:35:24.685039 WebtoonScraper-0.1.2/
--rw-rw-rw-   0        0        0     1089 2023-05-15 00:16:47.000000 WebtoonScraper-0.1.2/LICENSE
--rw-rw-rw-   0        0        0      140 2023-06-06 01:23:54.000000 WebtoonScraper-0.1.2/MANIFEST.in
--rw-rw-rw-   0        0        0    11009 2023-06-25 12:35:24.684032 WebtoonScraper-0.1.2/PKG-INFO
--rw-rw-rw-   0        0        0     9930 2023-06-22 08:36:45.000000 WebtoonScraper-0.1.2/README.md
-drwxrwxrwx   0        0        0        0 2023-06-25 12:35:24.666243 WebtoonScraper-0.1.2/WebtoonScraper/
--rw-rw-rw-   0        0        0      516 2023-06-06 00:42:00.000000 WebtoonScraper-0.1.2/WebtoonScraper/BestChallengeScraper.py
--rw-rw-rw-   0        0        0     6198 2023-06-21 11:41:23.000000 WebtoonScraper-0.1.2/WebtoonScraper/BufftoonScraper.py
--rw-rw-rw-   0        0        0     7405 2023-06-21 11:54:44.000000 WebtoonScraper-0.1.2/WebtoonScraper/NaverPostScraper.py
--rw-rw-rw-   0        0        0     3332 2023-06-07 11:43:11.000000 WebtoonScraper-0.1.2/WebtoonScraper/NaverWebtoonScraper.py
--rw-rw-rw-   0        0        0    16629 2023-06-25 12:32:48.000000 WebtoonScraper-0.1.2/WebtoonScraper/Scraper.py
--rw-rw-rw-   0        0        0     4715 2023-06-25 12:26:12.000000 WebtoonScraper-0.1.2/WebtoonScraper/TelescopeScraper.py
--rw-rw-rw-   0        0        0     4333 2023-06-22 08:34:53.000000 WebtoonScraper-0.1.2/WebtoonScraper/Webtoon.py
--rw-rw-rw-   0        0        0      501 2023-06-06 00:44:55.000000 WebtoonScraper-0.1.2/WebtoonScraper/WebtoonCanvasScraper.py
--rw-rw-rw-   0        0        0     4250 2023-06-17 07:29:55.000000 WebtoonScraper-0.1.2/WebtoonScraper/WebtoonOriginalsScraper.py
--rw-rw-rw-   0        0        0      630 2023-06-21 11:25:23.000000 WebtoonScraper-0.1.2/WebtoonScraper/__init__.py
--rw-rw-rw-   0        0        0     9473 2023-05-17 13:49:27.000000 WebtoonScraper-0.1.2/WebtoonScraper/foldermanagement.py
-drwxrwxrwx   0        0        0        0 2023-06-25 12:35:24.681869 WebtoonScraper-0.1.2/WebtoonScraper.egg-info/
--rw-rw-rw-   0        0        0    11009 2023-06-25 12:35:24.000000 WebtoonScraper-0.1.2/WebtoonScraper.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      653 2023-06-25 12:35:24.000000 WebtoonScraper-0.1.2/WebtoonScraper.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-25 12:35:24.000000 WebtoonScraper-0.1.2/WebtoonScraper.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        2 2023-05-17 14:16:38.000000 WebtoonScraper-0.1.2/WebtoonScraper.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0       48 2023-06-25 12:35:24.000000 WebtoonScraper-0.1.2/WebtoonScraper.egg-info/requires.txt
--rw-rw-rw-   0        0        0       15 2023-06-25 12:35:24.000000 WebtoonScraper-0.1.2/WebtoonScraper.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-06-25 12:35:24.685039 WebtoonScraper-0.1.2/setup.cfg
--rw-rw-rw-   0        0        0     1879 2023-06-25 12:34:38.000000 WebtoonScraper-0.1.2/setup.py
-drwxrwxrwx   0        0        0        0 2023-06-25 12:35:24.682883 WebtoonScraper-0.1.2/test/
--rw-rw-rw-   0        0        0      339 2023-06-25 12:33:54.000000 WebtoonScraper-0.1.2/test/test.py
+drwxrwxrwx   0        0        0        0 2023-06-29 13:18:59.498214 WebtoonScraper-1.0.0/
+-rw-rw-rw-   0        0        0     1089 2023-05-15 00:16:47.000000 WebtoonScraper-1.0.0/LICENSE
+-rw-rw-rw-   0        0        0      140 2023-06-06 01:23:54.000000 WebtoonScraper-1.0.0/MANIFEST.in
+-rw-rw-rw-   0        0        0    11936 2023-06-29 13:18:59.497207 WebtoonScraper-1.0.0/PKG-INFO
+-rw-rw-rw-   0        0        0    10517 2023-06-29 13:08:57.000000 WebtoonScraper-1.0.0/README.md
+drwxrwxrwx   0        0        0        0 2023-06-29 13:18:59.471313 WebtoonScraper-1.0.0/WebtoonScraper/
+-rw-rw-rw-   0        0        0      524 2023-06-27 18:35:30.000000 WebtoonScraper-1.0.0/WebtoonScraper/BestChallengeScraper.py
+-rw-rw-rw-   0        0        0     6181 2023-06-29 13:18:20.000000 WebtoonScraper-1.0.0/WebtoonScraper/BufftoonScraper.py
+-rw-rw-rw-   0        0        0    10194 2023-06-29 13:08:21.000000 WebtoonScraper-1.0.0/WebtoonScraper/FolderManager.py
+-rw-rw-rw-   0        0        0     4452 2023-06-28 15:30:07.000000 WebtoonScraper-1.0.0/WebtoonScraper/NaverGameScraper.py
+-rw-rw-rw-   0        0        0     7389 2023-06-26 11:53:01.000000 WebtoonScraper-1.0.0/WebtoonScraper/NaverPostScraper.py
+-rw-rw-rw-   0        0        0     3332 2023-06-07 11:43:11.000000 WebtoonScraper-1.0.0/WebtoonScraper/NaverWebtoonScraper.py
+-rw-rw-rw-   0        0        0    16339 2023-06-28 15:47:53.000000 WebtoonScraper-1.0.0/WebtoonScraper/Scraper.py
+-rw-rw-rw-   0        0        0     4715 2023-06-25 12:26:12.000000 WebtoonScraper-1.0.0/WebtoonScraper/TelescopeScraper.py
+-rw-rw-rw-   0        0        0     7786 2023-06-29 13:00:53.000000 WebtoonScraper-1.0.0/WebtoonScraper/Webtoon.py
+-rw-rw-rw-   0        0        0      501 2023-06-06 00:44:55.000000 WebtoonScraper-1.0.0/WebtoonScraper/WebtoonCanvasScraper.py
+-rw-rw-rw-   0        0        0     4252 2023-06-27 18:40:40.000000 WebtoonScraper-1.0.0/WebtoonScraper/WebtoonOriginalsScraper.py
+-rw-rw-rw-   0        0        0      679 2023-06-28 15:36:38.000000 WebtoonScraper-1.0.0/WebtoonScraper/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-29 13:18:59.495857 WebtoonScraper-1.0.0/WebtoonScraper.egg-info/
+-rw-rw-rw-   0        0        0    11936 2023-06-29 13:18:59.000000 WebtoonScraper-1.0.0/WebtoonScraper.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      685 2023-06-29 13:18:59.000000 WebtoonScraper-1.0.0/WebtoonScraper.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-29 13:18:59.000000 WebtoonScraper-1.0.0/WebtoonScraper.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        2 2023-05-17 14:16:38.000000 WebtoonScraper-1.0.0/WebtoonScraper.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0       48 2023-06-29 13:18:59.000000 WebtoonScraper-1.0.0/WebtoonScraper.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       15 2023-06-29 13:18:59.000000 WebtoonScraper-1.0.0/WebtoonScraper.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-06-29 13:18:59.498214 WebtoonScraper-1.0.0/setup.cfg
+-rw-rw-rw-   0        0        0     1462 2023-06-28 15:35:36.000000 WebtoonScraper-1.0.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-29 13:18:59.495857 WebtoonScraper-1.0.0/test/
+-rw-rw-rw-   0        0        0      339 2023-06-25 12:33:54.000000 WebtoonScraper-1.0.0/test/test.py
```

### Comparing `WebtoonScraper-0.1.2/LICENSE` & `WebtoonScraper-1.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `WebtoonScraper-0.1.2/PKG-INFO` & `WebtoonScraper-1.0.0/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: WebtoonScraper
-Version: 0.1.2
+Version: 1.0.0
 Summary: Scraping webtoons and some utils for it
 Home-page: https://github.com/ilotoki0804/WebtoonScraper
 Author: ilotoki0804
 Author-email: ilotoki0804@gmail.com
 License: MIT
 Keywords: Webtoon,Webtoon Scraper,Naver Webtoon,Webtoon Downloader,Download Webtoon
 Classifier: License :: OSI Approved :: MIT License
@@ -14,177 +14,204 @@
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 이 설명은 최신 버전이 아닐 수 있습니다. 만약 최신 버전을 확인하고 싶으시다면 [여기](https://github.com/ilotoki0804/WebtoonScraper)를 참고하세요.
 # WebtoonScraper
 
-웹툰을 다운로드하는 프로젝트입니다. 그 외에도 웹툰 모아서 보기 등 몇 가지 편의 기능을 지원합니다.
+웹툰을 다운로드하는 프로젝트입니다.
+
+네이버 웹툰, 베스트 도전만화, 웹툰 오리지널, 웹툰 캔버스, 만화경, 버프툰, 네이버 포스트, 네이버 게임을 지원합니다.
 
-네이버 웹툰, 베스트 도전만화, 웹툰 오리지널, 웹툰 캔버스, 만화경, 버프툰, 네이버 포스트를 지원합니다.
 # 시작하기
 
 1. 파이썬을 설치합니다.
-2. cmd 창을 열어 다음과 같은 명령어를 칩니다.
-
+2. cmd 창을 열어 pip 명령어를 실행합니다.
    ```
    pip install -U WebtoonScraper
    ```
 
-   또는
+# 네이버 웹툰, 베스트 도전만화, 웹툰 오리지널, 웹툰 캔버스, 만화경, 네이버 게임 다운로드하기
 
-   ```
-   pip3 install -U WebtoonScraper
-   ```
-
-# 네이버 웹툰, 베스트 도전만화, 웹툰 오리지널, 웹툰 캔버스, 만화경 다운로드하기
 버프툰과 네이버 포스트는 아래로 가서 확인하세요.
+
 1. 원하는 웹툰으로 가서 titleid 또는 title_no를 복사하세요.
-   ![img](https://raw.githubusercontent.com/ilotoki0804/WebtoonScraper/master/naver_webtoon.png)
-   국내의 경우 여기에서,
-   ![img](https://raw.githubusercontent.com/ilotoki0804/WebtoonScraper/master/webtoons_original.png)
-   해외의 경우는 여기에서,
-   ![img](https://raw.githubusercontent.com/ilotoki0804/WebtoonScraper/master/manhwakyung.png)
-   만화경의 경우는 여기에서 확인할 수 있습니다.
-2. 다음의 파이썬 코드를 웹툰이 다운로드되길 원하는 폴더 내에서 실행해 주세요. 웹툰은 정식 연재와 베스트 도전, Webtoons 오리지널과 캔버스, 만화경 모두 가능합니다.
+   ![img](https://raw.githubusercontent.com/ilotoki0804/WebtoonScraper/master/images/naver_webtoon.png)
+   네이버 웹툰과 베스트 도전의 경우 여기에서,
+   ![img](https://raw.githubusercontent.com/ilotoki0804/WebtoonScraper/master/images/webtoons_original.png)
+   웹툰 오리지널과 캔버스의 경우는 여기에서,
+   ![img](https://raw.githubusercontent.com/ilotoki0804/WebtoonScraper/master/images/manhwakyung.png)
+   만화경의 경우는 여기에서,
+   ![img](https://raw.githubusercontent.com/ilotoki0804/WebtoonScraper/master/images/naver_game.png)
+   네이버 게임 오리지널 시리즈의 경우는 여기에서 확인할 수 있습니다.
+2. 다음의 파이썬 코드를 웹툰이 다운로드되길 원하는 폴더 내에서 실행해 주세요. 웹툰은 정식 연재와 베스트 도전, Webtoons 오리지널과 캔버스, 만화경, 네이버 게임 모두 가능합니다.
 
    ```python
    from WebtoonScraper import Webtoon as wt
 
    # 네이버 웹툰
    wt.get_webtoon(76648, wt.N) # titleid를 여기에다 붙여넣으세요.
    # 베스트 도전만화
    wt.get_webtoon(763952, wt.B) # titleid를 여기에다 붙여넣으세요.
    # 웹툰 오리지널
    wt.get_webtoon(1435, wt.O) # titleid를 여기에다 붙여넣으세요.
    # 웹툰 캔버스
    wt.get_webtoon(304446, wt.C) # titleid를 여기에다 붙여넣으세요.
    # 만화경
    wt.get_webtoon(146, wt.M) # titleid를 여기에다 붙여넣으세요. Webtoon.T 태그도 사용 가능합니다.
+   # 네이버 게임 오리지널 시리즈
+   wt.get_webtoon(146, wt.G) # titleid를 여기에다 붙여넣으세요.
    ```
 
    이제 웹툰이 webtoons 폴더에 다운로드됩니다.
 
-   cf. 웹툰 태그를 생략하면 해당 웹툰이 어떤 사이트의 웹툰 id인지 자동으로 알아냅니다. 하지만 이 방식은 서로 다른 사이트에서 id가 겹치는 웹툰이 존재하면 오작동할 수 있으니 꼭 태그를 붙이는 것을 추천합니다.
+   cf. 웹툰 태그를 생략하면 해당 웹툰이 어떤 사이트의 웹툰 id인지 자동으로 알아냅니다. 만약 몇몇 태그가 겹친다면 태그에 맞는 수를 입력하는 창에 알맞은 수를 입력하면 됩니다.
 
    또 merge 태그를 이용하면 webtoon 폴더 내에 있는 모든 웹툰을 자동으로 5화씩 묶습니다.
 3. 만화 뷰어 앱을 통해 다운로드한 웹툰을 시청할 수 있습니다.
 
 ## 주의사항
 
 * 중간에 웹툰 다운로드가 멈춘 듯이 보여도 정상입니다. 그대로 가만히 있으면 다운로드가 다시 진행됩니다.
-* 만약 작동하지 않는다면 윈도우에서 Python 3.11.3을 설치하고 앞의 과정을 반복해 보세요.
+* 만약 작동하지 않는다면 윈도우에서 Python 3.11.4을 설치하고 앞의 과정을 반복해 보세요.
 
 # 버프툰 다운로드하기
-## 로그인하지 않은 상태에서 웹툰 다운로드하기(추천하지 않음)
+
+## 로그인하지 않은 상태에서 웹툰 다운로드하기
+
 로그인하지 않은 상태에서도 웹툰을 다운로드받을 수 있으나, 받을 수 있는 웹툰 수가 매우 적기에 추천하지 않습니다.
-1. 웹툰 페이지에 들어가 주소창의 맨 마지막 숫자를 복사합니다.
+
+1. 웹툰 페이지에 들어가 주소창의 맨 마지막 수를 복사합니다.
 2. 다음의 파이썬 코드를 웹툰이 다운로드되길 원하는 폴더 내에서 실행해 주세요.
    ```python
    from WebtoonScraper import Webtoon as wt
 
-   wt.get_webtoon(1007888, wt.BU) # 복사했던 숫자를 여기에다 붙여넣으세요.
+   wt.get_webtoon(1007888, wt.BU) # 복사했던 수를 여기에다 붙여넣으세요.
    ```
 3. 'Enter cookie of 1007888(시리즈 id) (Enter nothing to preceed without cookie)'라는 문구와 함께 입력란이 나오면 그냥 enter를 눌러줍니다.
 4. 로그인하지 않고 볼 수 있는 모든 에피소드가 다운로드됩니다.
+
 ## 로그인한 상태에서 웹툰 다운로드하기
-1. 웹툰 페이지에 들어가 주소창의 맨 마지막 숫자를 복사합니다.
-2. 로그인을 하고 f12를 누르고 네트워크 창을 연 뒤 아무 웹툰이나 들어갑니다.
-3. 아무 요청이나 클릭하고 나온 창에 '머리글' 탭을 엽니다.
+
+이 과정은 PC를 기준으로 설명합니다. 만약 모바일이라면 Kiwi Browser 등을 통해 다음의 과정을 수행할 수 있습니다.
+
+1. 웹툰 페이지에 들어가 주소창의 맨 마지막 수를 복사합니다. 이 예시에서는 1007888입니다.
+   ![img](https://raw.githubusercontent.com/ilotoki0804/WebtoonScraper/master/images/bufftoon1.png)
+2. 로그인을 하고 f12를 누르고 네트워크 창을 연 뒤 웹툰 페이지에 들어갑니다.
+   ![img](https://raw.githubusercontent.com/ilotoki0804/WebtoonScraper/master/images/bufftoon2.png)
+3. 새로고침을 한 뒤 '이름'에 있는 favicon.ico 요청을 클릭하고 나온 창에 '헤더' 탭을 엽니다.
+   ![img](https://raw.githubusercontent.com/ilotoki0804/WebtoonScraper/master/images/bufftoon3.png)
 4. 내려서 Cookie: 라고 되어 있는 모든 내용을 복사합니다.
+   ![img](https://raw.githubusercontent.com/ilotoki0804/WebtoonScraper/master/images/bufftoon4.png)
 5. 다음의 파이썬 코드를 웹툰이 다운로드되길 원하는 폴더 내에서 실행해 주세요.
+
    ```python
    from WebtoonScraper import Webtoon as wt
 
-   wt.get_webtoon(1007888, wt.BU) # 첫 번째로 복사했던 숫자를 여기에다 붙여넣으세요.
+   wt.get_webtoon(1007888, wt.BF) # 첫 번째로 복사했던 수를 여기에다 붙여넣으세요.
    ```
+
    혹은 다음과 같이 cookie를 코드 내에 포함할 수도 있습니다.
+
    ```python
    from WebtoonScraper import Webtoon as wt
    cookie = '두 번째로 복사했던 문자를 여기에다 붙여넣으세요.'
-   wt.get_webtoon(1007888, wt.BU, cookie=cookie) # 첫 번째로 복사했던 숫자를 여기에다 붙여넣으세요.
+   wt.get_webtoon(1007888, wt.BF, cookie=cookie) # 첫 번째로 복사했던 수를 여기에다 붙여넣으세요.
    ```
-6. 'Enter cookie of 1007888(시리즈 id) (Enter nothing to preceed without cookie)'라는 문구와 함께 입력란이 나오면 두 번째로 복사했던 일련의 문자열을 붙여넣기합니다.
-4. 로그인하면 볼 수 있는 모든 에피소드가 다운로드됩니다.
+
+   1. 'Enter cookie of 1007888(시리즈 id) (Enter nothing to proceed without cookie)'라는 문구와 함께 입력란이 나오면 두 번째로 복사했던 일련의 문자열을 붙여넣기합니다.
+6. 로그인하면 볼 수 있는 모든 에피소드가 다운로드됩니다.
 
 ## 주의사항
-* 버프툰은 titleid를 자동으로 알아내지 않습니다. 하지만 cookie를 입력하면 자동으로 버프툰으로 인식합니다.
+
+* get_webtoon에서 cookie를 입력하면 자동으로 버프툰으로 인식합니다.
 
 # 네이버 포스트 다운로드하기
 
 1. 웹툰이 있는 페이지로 가서 seriesNo와 memberNo를 복사하세요. 예시에서는 각각 597061과 19803452입니다.
-   ![img](https://raw.githubusercontent.com/ilotoki0804/WebtoonScraper/master/naver_post.png)
+   ![img](https://raw.githubusercontent.com/ilotoki0804/WebtoonScraper/master/images/naver_post.png)
 2. 다음의 파이썬 코드를 웹툰이 다운로드되길 원하는 폴더 내에서 실행해 주세요.
+
    ```python
    from WebtoonScraper import Webtoon as wt
 
    wt.get_webtoon(597061, wt.M) # 우선 seriesNo만 여기에 입력해주세요.
    ```
-   혹은 memberNo를 코드 내에 포함할 수 있습니다. 
+
+   혹은 memberNo를 코드 내에 포함할 수 있습니다.
+
    ```python
    from WebtoonScraper import Webtoon as wt
 
-   wt.get_webtoon(597061, wt.M, member_no='19803452')
+   wt.get_webtoon(597061, wt.M, member_no=19803452)
    ```
 3. 'Enter memberNo of 597061(해당 웹툰의 seriesNo)'라는 말과 함께 입력란이 나오면 거기에 아까 복사해 놓은 memberNo를 붙여넣습니다.
    만약 앞에서 이미 member_no를 사용했다면 이 단계는 건너뛰어집니다.
+
    ```
    Enter memberNo  of 597061: 19803452
    ...진행됨...
    ```
 4. 만화 뷰어 앱을 통해 다운로드한 웹툰을 시청할 수 있습니다.
+
 ## 주의사항
+
 * 가끔씩 이유 없는 오류가 발생할 수 있습니다. 그럴 때는 조금 시간이 지난 후에 다시 시도해 보세요.
-* 네이버 포스트는 titleid를 자동으로 알아내지 않습니다. 하지만 member_no를 입력하면 자동으로 포스트로 인식합니다.
+* 네이버 포스트는 titleid를 get_webtoon_platform으로 알아낼 수 없습니다.
+* member_no를 입력하면 자동으로 포스트로 인식됩니다.
+
 # 여러 회차 하나로 묶기
 
 1. 웹툰을 상기한 대로 다운로드받습니다.
 2. 다음과 같이 코드를 짭니다.
    ```python
-   from WebtoonScraper import *
+   from WebtoonScraper import FolderManager
 
-   folder = WebtoonFolderManagement('webtoon_merge')
-   folder.divide_all_webtoons(5)
+   fm = FolderManager()
+   fm.divide_all_webtoons(5)
    ```
 3. webtoons 폴더에 있는 **모든** 웹툰이 'webtoon_merge' 폴더에 5화씩 묶여져 다운로드됩니다.
 
 ## 주의사항
 
 * 시작 시 꼭 디렉토리를 선택해 주세요. 아니면 오류가 납니다.
 * 작업 중간에 폴더가 사라지고 이미지가 폴더 밖으로 나오는데, 이는 정상 과정입니다.
-* 너무 큰 숫자를 입력하면 웹툰 뷰어가 제대로 작동하지 않을 수 있음을 유의하세요.
+* 너무 큰 수를 입력하면 웹툰 뷰어가 제대로 작동하지 않을 수 있음을 유의하세요.
 
 # 묶인 회차 다시 원래대로 되돌리기
 
 1. 윗글의 기능으로 묶인 회차를 준비합니다.
 2. 다음과 같이 코드를 짭니다.
    ```python
-   from WebtoonScraper import *
+   from WebtoonScraper import FolderManager
 
-   folder = WebtoonFolderManagement('webtoon_merge')
-   folder.revert_to_original_state('webtoon/1초(725586)')
+   fm= FolderManager()
+   fm.restore_webtoons_in_directory('webtoon/1초(725586)')
    ```
 3. 'webtoon/1초(725586)' 폴더에 있던 모든 웹툰이 웹툰을 처음 다운로드했던 상태로 되돌아갑니다.
 
 # QNA
 
-## 회차가 띄엄띄엄 있거나 설정된 회차 번호가 작가가 설정한 회차 번호와 다릅니다./회차 묶기를 사용했는데 묶인 회차 수가 설정한 수보다 더 적습니다.
+## 회차 번호 관련
 
-### 생기는 이유
+### 문제와 이유
 
+회차가 띄엄띄엄 있거나 설정된 회차 번호가 작가가 설정한 회차 번호와 다르거나 회차 묶기를 사용했는데 묶인 회차 수가 설정한 수보다 더 적은 이유는 다음과 같습니다.
 이 프로젝트에서 웹툰의 회차 번호는 ID를 기준으로 합니다. 이는 작가가 정한 회차와는 다를 수 있습니다. 작가가 프롤로그부터 시작하는 경우(프로젝트의 회차 번호가 하나 빠름), 작가가 리메이크를 해서 전에 있던 작품을 제거해 ID가 연속적으로 있지 않는 경우(주로 베도에서 일어남/회차 번호가 띄엄띄엄하게 있음), 논란이나 작가 실수 등으로 회차가 삭제된 경우(한 회차를 건너띔) 등에서 ID가 불연속적이거나 작품과 일치하기 않는 경우가 생기게 됩니다.
 
 ### ID를 회차 번호로 그대로 사용하는 이유
 
 우선 작가가 설정한 회차 번호에 맞추는 것은 힘듭니다. 우선 번호가 어디에 있을지 알기 어렵고, 프롤로그가 있을지 없을지 알 수 없으며, 여러 화에 걸쳐 같은 에피소드를 진행하는 경우도 있고, 외전으로 본편의 회차에서 분리된 화를 운영하는 경우가 있어 화에 맞추어서 번호를 정하는 것을 어렵습니다.
 1부터 시작해서 끝까지 일정한 번호를 유지하는 것도 고려해볼 만하나 만약 그렇게 된다면 무결성 체크를 사용하기 어렵게 됩니다.
 따라서 작가가 설정한 회차를 그대로 사용하는 것도 어렵고, 만약 가능하다 할 지라도 무결성 체크를 포기하기 어렵기 때문에 현재는 ID를 회차 번호로 사용하고 있습니다.
 
 # Relese Note
 
+1.0.0: 네이버 게임 추가, FolderManager 리펙토링 및 개선, 정식 버전, docs 개선
+
 0.1.1: 네이버 포스트 추가, readme 작성, pbar 표시 내용 변경, 버그 수정
 
 0.1.0: 버프툰 추가, 빠진 부분 재추가
 
 0.0.19.3: merge 속성 추가, get_webtoon 함수로 변경
 
 0.0.19.1: pbar에 표시되는 내용 변경, 내부적 개선
```

### Comparing `WebtoonScraper-0.1.2/README.md` & `WebtoonScraper-1.0.0/README.md`

 * *Files 7% similar despite different names*

```diff
@@ -1,172 +1,199 @@
 # WebtoonScraper
 
-웹툰을 다운로드하는 프로젝트입니다. 그 외에도 웹툰 모아서 보기 등 몇 가지 편의 기능을 지원합니다.
+웹툰을 다운로드하는 프로젝트입니다.
+
+네이버 웹툰, 베스트 도전만화, 웹툰 오리지널, 웹툰 캔버스, 만화경, 버프툰, 네이버 포스트, 네이버 게임을 지원합니다.
 
-네이버 웹툰, 베스트 도전만화, 웹툰 오리지널, 웹툰 캔버스, 만화경, 버프툰, 네이버 포스트를 지원합니다.
 # 시작하기
 
 1. 파이썬을 설치합니다.
-2. cmd 창을 열어 다음과 같은 명령어를 칩니다.
-
+2. cmd 창을 열어 pip 명령어를 실행합니다.
    ```
    pip install -U WebtoonScraper
    ```
 
-   또는
+# 네이버 웹툰, 베스트 도전만화, 웹툰 오리지널, 웹툰 캔버스, 만화경, 네이버 게임 다운로드하기
 
-   ```
-   pip3 install -U WebtoonScraper
-   ```
-
-# 네이버 웹툰, 베스트 도전만화, 웹툰 오리지널, 웹툰 캔버스, 만화경 다운로드하기
 버프툰과 네이버 포스트는 아래로 가서 확인하세요.
+
 1. 원하는 웹툰으로 가서 titleid 또는 title_no를 복사하세요.
-   ![img](naver_webtoon.png)
-   국내의 경우 여기에서,
-   ![img](webtoons_original.png)
-   해외의 경우는 여기에서,
-   ![img](manhwakyung.png)
-   만화경의 경우는 여기에서 확인할 수 있습니다.
-2. 다음의 파이썬 코드를 웹툰이 다운로드되길 원하는 폴더 내에서 실행해 주세요. 웹툰은 정식 연재와 베스트 도전, Webtoons 오리지널과 캔버스, 만화경 모두 가능합니다.
+   ![img](images/naver_webtoon.png)
+   네이버 웹툰과 베스트 도전의 경우 여기에서,
+   ![img](images/webtoons_original.png)
+   웹툰 오리지널과 캔버스의 경우는 여기에서,
+   ![img](images/manhwakyung.png)
+   만화경의 경우는 여기에서,
+   ![img](images/naver_game.png)
+   네이버 게임 오리지널 시리즈의 경우는 여기에서 확인할 수 있습니다.
+2. 다음의 파이썬 코드를 웹툰이 다운로드되길 원하는 폴더 내에서 실행해 주세요. 웹툰은 정식 연재와 베스트 도전, Webtoons 오리지널과 캔버스, 만화경, 네이버 게임 모두 가능합니다.
 
    ```python
    from WebtoonScraper import Webtoon as wt
 
    # 네이버 웹툰
    wt.get_webtoon(76648, wt.N) # titleid를 여기에다 붙여넣으세요.
    # 베스트 도전만화
    wt.get_webtoon(763952, wt.B) # titleid를 여기에다 붙여넣으세요.
    # 웹툰 오리지널
    wt.get_webtoon(1435, wt.O) # titleid를 여기에다 붙여넣으세요.
    # 웹툰 캔버스
    wt.get_webtoon(304446, wt.C) # titleid를 여기에다 붙여넣으세요.
    # 만화경
    wt.get_webtoon(146, wt.M) # titleid를 여기에다 붙여넣으세요. Webtoon.T 태그도 사용 가능합니다.
+   # 네이버 게임 오리지널 시리즈
+   wt.get_webtoon(146, wt.G) # titleid를 여기에다 붙여넣으세요.
    ```
 
    이제 웹툰이 webtoons 폴더에 다운로드됩니다.
 
-   cf. 웹툰 태그를 생략하면 해당 웹툰이 어떤 사이트의 웹툰 id인지 자동으로 알아냅니다. 하지만 이 방식은 서로 다른 사이트에서 id가 겹치는 웹툰이 존재하면 오작동할 수 있으니 꼭 태그를 붙이는 것을 추천합니다.
+   cf. 웹툰 태그를 생략하면 해당 웹툰이 어떤 사이트의 웹툰 id인지 자동으로 알아냅니다. 만약 몇몇 태그가 겹친다면 태그에 맞는 수를 입력하는 창에 알맞은 수를 입력하면 됩니다.
 
    또 merge 태그를 이용하면 webtoon 폴더 내에 있는 모든 웹툰을 자동으로 5화씩 묶습니다.
 3. 만화 뷰어 앱을 통해 다운로드한 웹툰을 시청할 수 있습니다.
 
 ## 주의사항
 
 * 중간에 웹툰 다운로드가 멈춘 듯이 보여도 정상입니다. 그대로 가만히 있으면 다운로드가 다시 진행됩니다.
-* 만약 작동하지 않는다면 윈도우에서 Python 3.11.3을 설치하고 앞의 과정을 반복해 보세요.
+* 만약 작동하지 않는다면 윈도우에서 Python 3.11.4을 설치하고 앞의 과정을 반복해 보세요.
 
 # 버프툰 다운로드하기
-## 로그인하지 않은 상태에서 웹툰 다운로드하기(추천하지 않음)
+
+## 로그인하지 않은 상태에서 웹툰 다운로드하기
+
 로그인하지 않은 상태에서도 웹툰을 다운로드받을 수 있으나, 받을 수 있는 웹툰 수가 매우 적기에 추천하지 않습니다.
-1. 웹툰 페이지에 들어가 주소창의 맨 마지막 숫자를 복사합니다.
+
+1. 웹툰 페이지에 들어가 주소창의 맨 마지막 수를 복사합니다.
 2. 다음의 파이썬 코드를 웹툰이 다운로드되길 원하는 폴더 내에서 실행해 주세요.
    ```python
    from WebtoonScraper import Webtoon as wt
 
-   wt.get_webtoon(1007888, wt.BU) # 복사했던 숫자를 여기에다 붙여넣으세요.
+   wt.get_webtoon(1007888, wt.BU) # 복사했던 수를 여기에다 붙여넣으세요.
    ```
 3. 'Enter cookie of 1007888(시리즈 id) (Enter nothing to preceed without cookie)'라는 문구와 함께 입력란이 나오면 그냥 enter를 눌러줍니다.
 4. 로그인하지 않고 볼 수 있는 모든 에피소드가 다운로드됩니다.
+
 ## 로그인한 상태에서 웹툰 다운로드하기
-1. 웹툰 페이지에 들어가 주소창의 맨 마지막 숫자를 복사합니다.
-2. 로그인을 하고 f12를 누르고 네트워크 창을 연 뒤 아무 웹툰이나 들어갑니다.
-3. 아무 요청이나 클릭하고 나온 창에 '머리글' 탭을 엽니다.
+
+이 과정은 PC를 기준으로 설명합니다. 만약 모바일이라면 Kiwi Browser 등을 통해 다음의 과정을 수행할 수 있습니다.
+
+1. 웹툰 페이지에 들어가 주소창의 맨 마지막 수를 복사합니다. 이 예시에서는 1007888입니다.
+   ![img](images/bufftoon1.png)
+2. 로그인을 하고 f12를 누르고 네트워크 창을 연 뒤 웹툰 페이지에 들어갑니다.
+   ![img](images/bufftoon2.png)
+3. 새로고침을 한 뒤 '이름'에 있는 favicon.ico 요청을 클릭하고 나온 창에 '헤더' 탭을 엽니다.
+   ![img](images/bufftoon3.png)
 4. 내려서 Cookie: 라고 되어 있는 모든 내용을 복사합니다.
+   ![img](images/bufftoon4.png)
 5. 다음의 파이썬 코드를 웹툰이 다운로드되길 원하는 폴더 내에서 실행해 주세요.
+
    ```python
    from WebtoonScraper import Webtoon as wt
 
-   wt.get_webtoon(1007888, wt.BU) # 첫 번째로 복사했던 숫자를 여기에다 붙여넣으세요.
+   wt.get_webtoon(1007888, wt.BF) # 첫 번째로 복사했던 수를 여기에다 붙여넣으세요.
    ```
+
    혹은 다음과 같이 cookie를 코드 내에 포함할 수도 있습니다.
+
    ```python
    from WebtoonScraper import Webtoon as wt
    cookie = '두 번째로 복사했던 문자를 여기에다 붙여넣으세요.'
-   wt.get_webtoon(1007888, wt.BU, cookie=cookie) # 첫 번째로 복사했던 숫자를 여기에다 붙여넣으세요.
+   wt.get_webtoon(1007888, wt.BF, cookie=cookie) # 첫 번째로 복사했던 수를 여기에다 붙여넣으세요.
    ```
-6. 'Enter cookie of 1007888(시리즈 id) (Enter nothing to preceed without cookie)'라는 문구와 함께 입력란이 나오면 두 번째로 복사했던 일련의 문자열을 붙여넣기합니다.
-4. 로그인하면 볼 수 있는 모든 에피소드가 다운로드됩니다.
+
+   1. 'Enter cookie of 1007888(시리즈 id) (Enter nothing to proceed without cookie)'라는 문구와 함께 입력란이 나오면 두 번째로 복사했던 일련의 문자열을 붙여넣기합니다.
+6. 로그인하면 볼 수 있는 모든 에피소드가 다운로드됩니다.
 
 ## 주의사항
-* 버프툰은 titleid를 자동으로 알아내지 않습니다. 하지만 cookie를 입력하면 자동으로 버프툰으로 인식합니다.
+
+* get_webtoon에서 cookie를 입력하면 자동으로 버프툰으로 인식합니다.
 
 # 네이버 포스트 다운로드하기
 
 1. 웹툰이 있는 페이지로 가서 seriesNo와 memberNo를 복사하세요. 예시에서는 각각 597061과 19803452입니다.
-   ![img](naver_post.png)
+   ![img](images/naver_post.png)
 2. 다음의 파이썬 코드를 웹툰이 다운로드되길 원하는 폴더 내에서 실행해 주세요.
+
    ```python
    from WebtoonScraper import Webtoon as wt
 
    wt.get_webtoon(597061, wt.M) # 우선 seriesNo만 여기에 입력해주세요.
    ```
-   혹은 memberNo를 코드 내에 포함할 수 있습니다. 
+
+   혹은 memberNo를 코드 내에 포함할 수 있습니다.
+
    ```python
    from WebtoonScraper import Webtoon as wt
 
-   wt.get_webtoon(597061, wt.M, member_no='19803452')
+   wt.get_webtoon(597061, wt.M, member_no=19803452)
    ```
 3. 'Enter memberNo of 597061(해당 웹툰의 seriesNo)'라는 말과 함께 입력란이 나오면 거기에 아까 복사해 놓은 memberNo를 붙여넣습니다.
    만약 앞에서 이미 member_no를 사용했다면 이 단계는 건너뛰어집니다.
+
    ```
    Enter memberNo  of 597061: 19803452
    ...진행됨...
    ```
 4. 만화 뷰어 앱을 통해 다운로드한 웹툰을 시청할 수 있습니다.
+
 ## 주의사항
+
 * 가끔씩 이유 없는 오류가 발생할 수 있습니다. 그럴 때는 조금 시간이 지난 후에 다시 시도해 보세요.
-* 네이버 포스트는 titleid를 자동으로 알아내지 않습니다. 하지만 member_no를 입력하면 자동으로 포스트로 인식합니다.
+* 네이버 포스트는 titleid를 get_webtoon_platform으로 알아낼 수 없습니다.
+* member_no를 입력하면 자동으로 포스트로 인식됩니다.
+
 # 여러 회차 하나로 묶기
 
 1. 웹툰을 상기한 대로 다운로드받습니다.
 2. 다음과 같이 코드를 짭니다.
    ```python
-   from WebtoonScraper import *
+   from WebtoonScraper import FolderManager
 
-   folder = WebtoonFolderManagement('webtoon_merge')
-   folder.divide_all_webtoons(5)
+   fm = FolderManager()
+   fm.divide_all_webtoons(5)
    ```
 3. webtoons 폴더에 있는 **모든** 웹툰이 'webtoon_merge' 폴더에 5화씩 묶여져 다운로드됩니다.
 
 ## 주의사항
 
 * 시작 시 꼭 디렉토리를 선택해 주세요. 아니면 오류가 납니다.
 * 작업 중간에 폴더가 사라지고 이미지가 폴더 밖으로 나오는데, 이는 정상 과정입니다.
-* 너무 큰 숫자를 입력하면 웹툰 뷰어가 제대로 작동하지 않을 수 있음을 유의하세요.
+* 너무 큰 수를 입력하면 웹툰 뷰어가 제대로 작동하지 않을 수 있음을 유의하세요.
 
 # 묶인 회차 다시 원래대로 되돌리기
 
 1. 윗글의 기능으로 묶인 회차를 준비합니다.
 2. 다음과 같이 코드를 짭니다.
    ```python
-   from WebtoonScraper import *
+   from WebtoonScraper import FolderManager
 
-   folder = WebtoonFolderManagement('webtoon_merge')
-   folder.revert_to_original_state('webtoon/1초(725586)')
+   fm= FolderManager()
+   fm.restore_webtoons_in_directory('webtoon/1초(725586)')
    ```
 3. 'webtoon/1초(725586)' 폴더에 있던 모든 웹툰이 웹툰을 처음 다운로드했던 상태로 되돌아갑니다.
 
 # QNA
 
-## 회차가 띄엄띄엄 있거나 설정된 회차 번호가 작가가 설정한 회차 번호와 다릅니다./회차 묶기를 사용했는데 묶인 회차 수가 설정한 수보다 더 적습니다.
+## 회차 번호 관련
 
-### 생기는 이유
+### 문제와 이유
 
+회차가 띄엄띄엄 있거나 설정된 회차 번호가 작가가 설정한 회차 번호와 다르거나 회차 묶기를 사용했는데 묶인 회차 수가 설정한 수보다 더 적은 이유는 다음과 같습니다.
 이 프로젝트에서 웹툰의 회차 번호는 ID를 기준으로 합니다. 이는 작가가 정한 회차와는 다를 수 있습니다. 작가가 프롤로그부터 시작하는 경우(프로젝트의 회차 번호가 하나 빠름), 작가가 리메이크를 해서 전에 있던 작품을 제거해 ID가 연속적으로 있지 않는 경우(주로 베도에서 일어남/회차 번호가 띄엄띄엄하게 있음), 논란이나 작가 실수 등으로 회차가 삭제된 경우(한 회차를 건너띔) 등에서 ID가 불연속적이거나 작품과 일치하기 않는 경우가 생기게 됩니다.
 
 ### ID를 회차 번호로 그대로 사용하는 이유
 
 우선 작가가 설정한 회차 번호에 맞추는 것은 힘듭니다. 우선 번호가 어디에 있을지 알기 어렵고, 프롤로그가 있을지 없을지 알 수 없으며, 여러 화에 걸쳐 같은 에피소드를 진행하는 경우도 있고, 외전으로 본편의 회차에서 분리된 화를 운영하는 경우가 있어 화에 맞추어서 번호를 정하는 것을 어렵습니다.
 1부터 시작해서 끝까지 일정한 번호를 유지하는 것도 고려해볼 만하나 만약 그렇게 된다면 무결성 체크를 사용하기 어렵게 됩니다.
 따라서 작가가 설정한 회차를 그대로 사용하는 것도 어렵고, 만약 가능하다 할 지라도 무결성 체크를 포기하기 어렵기 때문에 현재는 ID를 회차 번호로 사용하고 있습니다.
 
 # Relese Note
 
+1.0.0: 네이버 게임 추가, FolderManager 리펙토링 및 개선, 정식 버전, docs 개선
+
 0.1.1: 네이버 포스트 추가, readme 작성, pbar 표시 내용 변경, 버그 수정
 
 0.1.0: 버프툰 추가, 빠진 부분 재추가
 
 0.0.19.3: merge 속성 추가, get_webtoon 함수로 변경
 
 0.0.19.1: pbar에 표시되는 내용 변경, 내부적 개선
```

### Comparing `WebtoonScraper-0.1.2/WebtoonScraper/BestChallengeScraper.py` & `WebtoonScraper-1.0.0/WebtoonScraper/BestChallengeScraper.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,14 @@
 '''Download Webtoons from Naver Webtoon Best Challenge.
 '''
 from WebtoonScraper.NaverWebtoonScraper import NaverWebtoonScraper
+
+
 class BestChallengeScraper(NaverWebtoonScraper):
     def __init__(self, pbar_independent=False, short_connection=False):
         super().__init__(pbar_independent, short_connection)
         self.BASE_URL = 'https://comic.naver.com/bestChallenge'
         self.EPISODE_IMAGES_URL_SELECTOR = '#comic_view_area > div > img'
 
+
 if __name__ == '__main__':
-    wt = BestChallengeScraper()
+    wt = BestChallengeScraper()
```

### Comparing `WebtoonScraper-0.1.2/WebtoonScraper/BufftoonScraper.py` & `WebtoonScraper-1.0.0/WebtoonScraper/BufftoonScraper.py`

 * *Files 2% similar despite different names*

```diff
@@ -23,30 +23,30 @@
         # print(raw_data)
         subtitles = {}
         episode_ids = {}
         for raw_episode in raw_data['result']['episodes']:
             if not get_payment and raw_episode['isPaymentEpisode']:
                 if self.PBAR_INDEPENDENT:
                     pass
-                print(f"Episode '{raw_episode['title']}' is not free of charge episode. It'll be not downloaded.")
+                print(f"Episode '{raw_episode['title']}' is not free of charge episode. It won't be downloaded.")
                 continue
             if not self.COOKIE and not raw_episode['isOpenFreeEpisode']:
                 if self.PBAR_INDEPENDENT:
                     pass
                 print(f"Episode '{raw_episode['title']}' is not opened for non-login users. It'll be not downloaded.")
                 continue
             episode_no = raw_episode['episodeOrder']
             raw_episode_id = raw_episode['listImgPath']
             # print(raw_episode_id)
             episode_id = int(re.search(rf'(?<=contents\/.\/{titleid}\/)(\d+)(?=\/)', raw_episode_id).group(0))
             episode_ids[episode_no] = episode_id
             subtitles[episode_no] = raw_episode['title']
         return subtitles, episode_ids
 
-    async def get_title(self, titleid, file_acceptable, limit: int=500):
+    async def get_title(self, titleid, file_acceptable):
         url = f'https://bufftoon.plaync.com/series/{titleid}'
         title = await self.get_internet(get_type='soup_select_one', url=url,
                                         selector='#content > div > div > div.series-info > div.cont > div.title')
         title = title.text.strip()
         if file_acceptable:
             title = self.get_acceptable_file_name(title)
         return title
```

### Comparing `WebtoonScraper-0.1.2/WebtoonScraper/NaverPostScraper.py` & `WebtoonScraper-1.0.0/WebtoonScraper/NaverPostScraper.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,23 +1,21 @@
 '''Download Webtoons from Naver Post.
 '''
-import re
 from pathlib import Path
-import time
 from itertools import count
 import asyncio
 from async_lru import alru_cache
 import demjson3
 from bs4 import BeautifulSoup
 # from WebtoonScraper.Scraper import Scraper
 from WebtoonScraper.Scraper import Scraper
 
 class NaverPostScraper(Scraper):
     '''Scrape webtoons from Naver Post.'''
-    def __init__(self, pbar_independent=False, short_connection=False, cookie=None):
+    def __init__(self, pbar_independent=False, short_connection=False):
         super().__init__(pbar_independent, short_connection)
         self.BASE_URL = 'https://post.naver.com'
         if not short_connection:
             self.IS_STABLE_CONNECTION = True
 
     def download_one_webtoon(self, titleid: int, member_no: int,  value_range: tuple|int|None=None) -> None:
         """async를 사용하지 않는 일반 상태일 경우 사용하는 함수이다. 사용법은 download_one_webtoon_async와 동일하다."""
@@ -37,15 +35,15 @@
             # n번째 리스트 불러옴
             url = f'https://post.naver.com/my/series/detail/more.nhn?memberNo={self.member_no}&seriesNo={titleid}&lastSortOrder=49&prevVolumeNo=&fromNo={i}&totalCount=68'
             # print(url)
             response = await self.get_internet('requests', url)
 
             # 네이버는 기본적으로 json이 망가져 있기에 json이 망가져 있어도 parse를 해주는 demres가 필요
             demres = demjson3.decode(response.text)['html']
-            soup = BeautifulSoup(demres, 'lxml')
+            soup = BeautifulSoup(demres, 'html.parser')
             
             # subtitle data만듦.
             for tag in soup.select('ul > li > a > div > span.ell'):
                 subtitle_sublist.append({'subtitle' : tag.text.strip()})
             for j, tag in enumerate(soup.select('ul > li > a > div > span.spot_post_like')):
                 # 버려지는 값은 member_no/그냥 member_no라고 해도 되지만 혹시 모를 corruption을 막기 위한 조치
                 episode_id, _ = map(int, tag['data-cid'].split('_'))
@@ -108,20 +106,20 @@
                 # 하지만 오류 이유는 불명, 가끔씩 생기는 문제.
                 print(f'episode {titleid} invalid. retrying...')
             else:
                 break
         else:
             raise ConnectionError('Unknown error occurred. Please try again later.')
         content = content.text
-        soup_content = BeautifulSoup(content, 'lxml')
+        soup_content = BeautifulSoup(content, 'html.parser')
         # import requests
         # res = requests.get(f'https://post.naver.com/viewer/postView.naver?volumeNo={episode_id}&memberNo={self.member_no}&navigationType=push')
         # soup = BeautifulSoup(res.text, 'html.parser')
         # content = soup.select_one('#__clipContent').text
-        # soup_content = BeautifulSoup(content, 'lxml')
+        # soup_content = BeautifulSoup(content, 'html.parser')
         episode_images_url = []
         # 문서 내에 있는 모든 이미지 링크를 불러옴
         for tag in soup_content.select('div.se_component_wrap.sect_dsc.__se_component_area > div > div > div > div > a > img'):
             episode_images_url.append(tag['data-src'])
         return [url for url in episode_images_url if not url.startswith('https://mail.naver.com/read/image/')]
     
 if __name__ == '__main__':
```

### Comparing `WebtoonScraper-0.1.2/WebtoonScraper/NaverWebtoonScraper.py` & `WebtoonScraper-1.0.0/WebtoonScraper/NaverWebtoonScraper.py`

 * *Files identical despite different names*

### Comparing `WebtoonScraper-0.1.2/WebtoonScraper/Scraper.py` & `WebtoonScraper-1.0.0/WebtoonScraper/Scraper.py`

 * *Files 4% similar despite different names*

```diff
@@ -3,22 +3,20 @@
 import re
 import os
 import asyncio
 import shutil
 import html
 from pathlib import Path
 from typing import Iterable, Literal
-# from abc import ABCMeta
-from abc import abstractmethod
+from abc import abstractmethod, ABCMeta
 
-from better_abc import ABCMeta, abstract_attribute
 import requests
 from bs4 import BeautifulSoup as bs
+from bs4.element import Tag
 from tqdm import tqdm
-from bs4.element import Tag as bsTag
 
 class Scraper(metaclass=ABCMeta):
     """Abstract class of all scrapers.
     
     init, get_internet, 전반적인 로직 등은 모두 이 페이지에서 관리하고, 구체적인 다운로드 방법은 각각의 scraper들에게 맡깁니다.
     따라서 썸네일을 받아오거나 한 회차의 이미지 URL을 불러오는 등의 역할은 각자 scraper들에 구현되어 있습니다.
     """
@@ -30,44 +28,35 @@
         
         Args:
             pbar_independent: 만약 True라면 tqdm을 이용해서 로그를 표시하고, False라면 print를 통해서 로그를 표시합니다.
             short_connection:
                 만약 True라면 timeout를 3초로 짧게 잡고 IS_STABLE_CONNECTION(거짓일 경우, 연결에 실패하면 재시도를 함.)을 False로 합니다.
                 False라면 기본 설정을 유지하고 timeout도 길게(120초) 유지합니다.
         """
-        # self.loop = asyncio.get_event_loop()
+        # BASE_URL and IS_STABLE_CONNECTION have to defined!
         self.HEADERS = {
             'User-Agent' : 'Mozilla/5.0 (Windows NT 10.0; Win64; x64) AppleWebKit/537.36 '
             '(KHTML, like Gecko) Chrome/113.0.0.0 Safari/537.36'
             }
-        self.set_folders()
+        # self.set_folders()
+        self.BASE_DIR = 'webtoon'
         self.TIMEOUT = 120
         self.PBAR_INDEPENDENT = pbar_independent
         if short_connection:
             self.TIMEOUT = 3
             self.IS_STABLE_CONNECTION = False
     
-    @abstract_attribute
-    def BASE_URL(self):
-        """Abstract 'attribute' for self.BASE_URL."""
-        pass
-    
-    @abstract_attribute
-    def IS_STABLE_CONNECTION(self):
-        """Abstract 'attribute' for self.IS_STABLE_CONNECTION."""
-        pass
-    
     # @profile
     async def get_internet(
             self, get_type: Literal['requests', 'soup', 'soup_select', 'soup_select_one'], 
             url: str, selector=None, 
             is_run_in_executor=False, 
             attempt: int=10, 
             headers=None
-            ) -> requests.Response|bs|list|bsTag|None:
+            ) -> requests.Response|bs|list|Tag|None:
         """Get response/beautifulsoup/beautifulsoup tag list/beautifulsoup tag from internet.
 
         Args:
             get_type:
                 인터넷에서 url로부터 받은 것으로부터 할 것이 무엇인지를 결정합니다.
 
                 'requests': reqests.get한 값을 그대로(.content나 .test, .json()이 붙지 않은 원본 그대로) 반환합니다.
@@ -193,18 +182,22 @@
                 if ord(chractor) in (0, 1, 2, 3, 4, 5, 6, 7, 8, 9, 10, 11, 12, 13, 14, 15, 16, 17, 18, 19, 20, 21,
                                      22, 23, 24, 25, 26, 27, 28, 29, 30, 31, 34, 42, 58, 60, 62, 63, 124):
                     strict_checked_string += ' '
                 else:
                     strict_checked_string += chractor
             return strict_checked_string
         return processed
-    
-    def set_folders(self, base_dir: str='webtoon') -> None:
-        """Set base folder."""
-        self.BASE_DIR = Path(base_dir)
+
+    @property
+    def BASE_DIR(self):
+        return self._BASE_DIR
+
+    @BASE_DIR.setter
+    def BASE_DIR(self, BASE_DIR):
+        self._BASE_DIR = Path(BASE_DIR)
 
 ################################## MAIN ACTION ##################################
 
     def download_one_webtoon(self, titleid: int, value_range: tuple|int|None=None) -> None:
         """async를 사용하지 않는 일반 상태일 경우 사용하는 함수이다. 사용법은 download_one_webtoon_async와 동일하다."""
         asyncio.run(self.download_one_webtoon_async(titleid, value_range))
         # self.loop.run_until_complete(self.download_one_webtoon_async(titleid, value_range))
@@ -222,14 +215,15 @@
                                 None일 경우: 웹툰의 모든 회차를 다운로드 받는다.
         :attempt(deprecated): episode_no_range가 None이어서 자동으로 웹툰을 다운로드 받을 경우 몇 번째 episode까지 다운로드 받을지 결정한다.
         """
         self.loop = asyncio.get_running_loop()
 
         title = await self.get_title(titleid, file_acceptable=True)
         webtoon_dir = self.BASE_DIR / f'{title}({titleid})'
+        self.webtoon_dir = webtoon_dir
 
         webtoon_dir.mkdir(parents=True, exist_ok=True)
 
         await self.save_webtoon_thumbnail(titleid, title, webtoon_dir)
 
         if not episode_no_range:
             titleids = await self.get_all_episode_no(titleid, attempt=50)
@@ -243,25 +237,22 @@
         for episode_no in self.pbar:
             await self.download_one_episode(episode_no, titleid, webtoon_dir)
         print(f'A webtoon {title} download ended.')
 
     @abstractmethod
     async def get_title(self, titleid: int, file_acceptable: bool) -> str:
         """웹툰의 title을 불러온다."""
-        pass
 
     @abstractmethod
     async def save_webtoon_thumbnail(self, titleid: int, title: str, thumbnail_dir: Path) -> None:
         """웹툰의 썸네일을 불러오고 thumbnail_dir에 저장한다."""
-        pass
     
     @abstractmethod
     async def get_all_episode_no(self, titleid: int, attempt: int) -> Iterable:
         """웹툰에서 전체 에피소드를 가져온다."""
-        pass
 
     # @profile
     def _check_validate_of_files(self, episode_dir: Path, episode_no: int, image_urls: list, subtitle: str) -> None|bool:
         """episode_dir를 생성하고 이미 있다면 해당 폴더 내 내용물이 적합한지 조사한다.
 
         None를 return한다면 회차를 다운로드해야 한다는 의미이다.
         True를 return하면 해당 회차가 이미 완전히 다운로드되어 있으며, 따라서 다운로드를 지속할 이유가 없음을 의미한다.
@@ -298,27 +289,26 @@
         self._set_pbar(f'downloading {subtitle}')
         get_image_coroutines = (self.download_single_image(episode_dir, element, i) for i, element in enumerate(episode_images_url))
         await asyncio.gather(*get_image_coroutines)
 
     @abstractmethod
     async def get_subtitle(self, titleid: int, episode_no: int, file_acceptable: bool) -> str:
         """부제목, 즉 회차의 제목을 불러온다."""
-        pass
 
     @abstractmethod
     async def get_episode_images_url(self, titleid: int, episode_no: int) -> list:
         """해당 회차를 구성하는 이미지들을 불러온다."""
-        pass
 
     # @profile
     async def download_single_image(self, episode_dir: Path, url: str, image_no: int) -> None:
         """Download image from url and returns to {episode_dir}/{file_name(translated to accactable name)}."""
         # print(url)
         image_extension = self.get_file_extension(url)
         file_name = f'{image_no:03d}.{image_extension}'
 
         # self._set_pbar(f'{episode_dir}|{file_name}')
         image_raw = await self.get_internet(get_type='requests', url=url, is_run_in_executor=True)
         image_raw = image_raw.content
 
         file_dir = episode_dir / file_name
-        file_dir.write_bytes(image_raw)
+        file_dir.write_bytes(image_raw)
+
```

### Comparing `WebtoonScraper-0.1.2/WebtoonScraper/TelescopeScraper.py` & `WebtoonScraper-1.0.0/WebtoonScraper/TelescopeScraper.py`

 * *Files identical despite different names*

### Comparing `WebtoonScraper-0.1.2/WebtoonScraper/WebtoonOriginalsScraper.py` & `WebtoonScraper-1.0.0/WebtoonScraper/WebtoonOriginalsScraper.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 '''Download Webtoons from Webtoon Originals.
 '''
+from bs4 import BeautifulSoup as bs
+
 from WebtoonScraper.Scraper import Scraper
 
-from bs4 import BeautifulSoup as bs
 class WebtoonOriginalsScraper(Scraper):
     '''Scrape webtoons from Webtoon Originals.'''
     def __init__(self, pbar_independent=False, short_connection=False):
         super().__init__(pbar_independent, short_connection)
         self.BASE_URL = 'https://www.webtoons.com/en/fantasy/watermelon'
         self.IS_STABLE_CONNECTION = False
         self.USER_AGENT = {
```

### Comparing `WebtoonScraper-0.1.2/WebtoonScraper/__init__.py` & `WebtoonScraper-1.0.0/WebtoonScraper/__init__.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 from WebtoonScraper.NaverWebtoonScraper import NaverWebtoonScraper
-from WebtoonScraper.foldermanagement import WebtoonFolderManagement
+from WebtoonScraper.FolderManager import FolderManager
 from WebtoonScraper.WebtoonOriginalsScraper import WebtoonOriginalsScraper
 from WebtoonScraper.BestChallengeScraper import BestChallengeScraper
 from WebtoonScraper.WebtoonCanvasScraper import WebtoonCanvasScraper
 from WebtoonScraper import Webtoon
 from WebtoonScraper.TelescopeScraper import TelescopeScraper
 from WebtoonScraper.BufftoonScraper import BufftoonScraper
 from WebtoonScraper.NaverPostScraper import NaverPostScraper
+from WebtoonScraper.NaverGameScraper import NaverGameScraper
 
 if __name__ == '__main__':
     print('Testing codes.')
```

### Comparing `WebtoonScraper-0.1.2/WebtoonScraper/foldermanagement.py` & `WebtoonScraper-1.0.0/WebtoonScraper/FolderManager.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,200 +1,228 @@
 # 회차 묶기
 import os
 import shutil
 import re
 from collections import defaultdict
+from pathlib import Path
+import logging
 
-class WebtoonFolderManagement:
-    def __init__(self, alt_dir):
-        self.BASE_DIR = r'webtoon'
-        self.alt_dir = alt_dir
-        self._make_directory(alt_dir)
-        self.TEMP_DIR = 'temp'
-        self._make_directory(self.TEMP_DIR)
-
-    def _make_directory(self, directory, alert=True):
-        try:
-            os.makedirs(directory)
-        except FileExistsError:
-            if alert:
-                print(f'Folder already exists. Overwrite the folder and continue. Folder name: {directory}')
 
-    def divide_all_webtoons(self, episode_bundle, asking_every_time=False):
-        webtoons = os.listdir(self.BASE_DIR)
-        for webtoon in webtoons:
-            alt_webtoon_dir = self.alt_dir + r'/' + webtoon
-            base_webtoon_dir = self.BASE_DIR + r'/' + webtoon
+class FolderManager:
+    def __init__(self):
+        
+        self.BASE_DIR = 'webtoon'
+        self.ALT_DIR = 'webtoon'
 
+    @property
+    def BASE_DIR(self):
+        return self._BASE_DIR
 
+    @BASE_DIR.setter
+    def BASE_DIR(self, BASE_DIR):
+        self._BASE_DIR = Path(BASE_DIR)
 
-            if asking_every_time:
-                try:
-                    episode_bundle = int(input(f'Please write down number for episode bundle. Recommend is 5. enter blank to skip.'))
-                    if not episode_bundle:
-                        continue
-                except ValueError:
-                    continue
-                self._make_directory(alt_webtoon_dir)
-                self._divide_webtoon(
-                    base_webtoon_dir, alt_webtoon_dir, 
-                    episode_bundle=episode_bundle
-                )
-            else:
-                self._make_directory(alt_webtoon_dir)
-                self._divide_webtoon(base_webtoon_dir, alt_webtoon_dir, episode_bundle=episode_bundle)
-            os.rmdir(base_webtoon_dir)
-            # break      
+    @property
+    def ALT_DIR(self):
+        return self._ALT_DIR
 
-    def _move_thumbnail(self, base_webtoon_dir, alt_webtoon_dir):
-        does_thumbnail_exist = False
-        for episode_or_thumbnail in os.listdir(base_webtoon_dir):
-            if re.match(r'.+[.](jpg|jpeg|png)$', episode_or_thumbnail, re.I):
-                does_thumbnail_exist = True
-                base_thumbnail_dir = f'{base_webtoon_dir}/{episode_or_thumbnail}'
-                alt_thumbnail_dir2 = f'{self.TEMP_DIR}/{episode_or_thumbnail}'
-                realt_thumbnail_dir = f'{alt_webtoon_dir}/{episode_or_thumbnail}'
-                shutil.move(base_thumbnail_dir, alt_thumbnail_dir2)
-                return does_thumbnail_exist, alt_thumbnail_dir2, realt_thumbnail_dir
-        return False, None, None
+    @ALT_DIR.setter
+    def ALT_DIR(self, ALT_DIR):
+        self._ALT_DIR = Path(ALT_DIR)
+
+    ############### MAIN FUNCTIONALITY ###############
 
-    def _divide_webtoon(self, base_webtoon_dir, alt_webtoon_dir, episode_bundle, merge_last_bundle=True):
-        self._make_directory(self.TEMP_DIR, alert=False)
+    def merge_webtoons_in_directory(self, merge_amount):
+        webtoons = os.listdir(self.BASE_DIR)
+        for webtoon in webtoons:
+            alt_webtoon_dir = self.ALT_DIR / webtoon
+            # base_dir와 alt_dir가 같은 경우를 대비해 이름을 달리함.
+            temp_alt_webtoon_dir = self.ALT_DIR / (webtoon + '(merged)') # why do I have to?
+            base_webtoon_dir = self.BASE_DIR / webtoon
+            self._merge_webtoon_episodes(base_webtoon_dir, temp_alt_webtoon_dir, merge_amount=merge_amount)
+            shutil.rmtree(base_webtoon_dir)
+            temp_alt_webtoon_dir.rename(alt_webtoon_dir)
+            # break
+
+    def merge_webtoon_episodes(self,
+                               webtoon_dir: Path,
+                               merge_amount,
+                               merge_last_bundle=True):
+        # base_dir와 alt_dir가 같은 경우를 대비해 이름을 달리함.
+        # temp_alt_webtoon_dir = Path(str(webtoon_dir.parents)) / (webtoon_dir.name + '(merged)') # why do I have to?
+        temp_alt_webtoon_dir = Path(str(webtoon_dir) + '(merged)')
+        self._merge_webtoon_episodes(webtoon_dir, temp_alt_webtoon_dir, merge_amount=merge_amount, merge_last_bundle=merge_last_bundle)
+        os.rmdir(webtoon_dir)
+        temp_alt_webtoon_dir.rename(webtoon_dir)
+
+    def _merge_webtoon_episodes(self, base_webtoon_dir: Path, alt_webtoon_dir: Path, merge_amount, merge_last_bundle=True):
+        # base_webtoon_dir와 alt_webtoon_dir가 같으면 안됨!
+        if base_webtoon_dir == alt_webtoon_dir:
+            raise NotImplementedError('base_webtoon_dir and alt_webtoon_dir cannot be same.')
         
-        # Thumbnail 옮기기
-        does_thumbnail_exist, alt_thumbnail_dir, realt_thumbnail_dir = self._move_thumbnail(base_webtoon_dir, alt_webtoon_dir)
-        # print(self._move_thumbnail(base_webtoon_dir, alt_webtoon_dir))
+        alt_webtoon_dir.mkdir(parents=True, exist_ok=True)
+
+        # Thumbnail 옮기기 > alt_dir로 옮기는 것으로 변경
+        self._move_thumbnail(base_webtoon_dir, alt_webtoon_dir)
         
+        # 에피소드를 분해해 base_webtoon_dir에 형식에 맞추어 넣음
         if not self._is_unified(base_webtoon_dir):
             self._unify_webtoon(base_webtoon_dir)
 
-        if episode_bundle == 1:
-            print('Episode bundle value is 1, so autometically revert directory state to original.')
-            self.revert_to_original_download_state(base_webtoon_dir)
+        # episode_bundle이 1인 경우 revert_to_original_download_state 수행
+        if merge_amount == 1:
+            print('Value of episode_bundle is 1, so autometically revert directory state to original.')
+            self.restore_webtoon(base_webtoon_dir)
         episodes = os.listdir(base_webtoon_dir)
-        if len(episodes) <= merge_last_bundle:
-            merge_last_bundle = len(episodes)
 
-        # 묶음으로 묶는 과정
-        episode_bundle_name_collection = defaultdict(list)
+        # merge_last_bundle을 고려하지 않고 컬랙션을 제작함
+        merged_images: list[list[str]] = defaultdict(list)
         for episode in episodes:
             episode_no = int(episode.split('.')[0])
-            episode_bundle_name_collection[(episode_no - 1)//episode_bundle].append(episode)
-        if merge_last_bundle and len(episode_bundle_name_collection):
-            episode_last_bundle = max(episode_bundle_name_collection.keys())
-            last_bundle_value = episode_bundle_name_collection[episode_last_bundle]
-            episode_ids = set()
-            for image in last_bundle_value:
-                episode_ids.add(image.split('.')[0])
-            last_bundle_length = len(episode_ids)
-            if last_bundle_length < episode_bundle:
-                episode_list = list(episode_bundle_name_collection.keys())
-                before_last_bundle = episode_list[episode_list.index(episode_last_bundle) - 1]
-                # episode_bundle_name_collection[episode_last_bundle - 1].extend(last_bundle_value)
-                episode_bundle_name_collection[before_last_bundle].extend(last_bundle_value)
-                del episode_bundle_name_collection[episode_last_bundle]
-        
-        # 폴더에 넣는 과정
-        temp_dir = fr'{self.TEMP_DIR}/temp'
-        base_dir = fr'{base_webtoon_dir}'
-        episode_bundle_name_collection = episode_bundle_name_collection.values()
-        for episode_name_list in episode_bundle_name_collection:
-            self._make_directory(temp_dir, alert=False)
-            for image_name in episode_name_list:
-                image_dir = fr'{base_dir}/{image_name}'
-                shutil.move(image_dir, temp_dir)
-            dir_name = self._make_dir_name(temp_dir)
-            alt_dir = fr'{alt_webtoon_dir}/{dir_name}'
-            self._make_directory(alt_dir)
-            self._move_dir(temp_dir, alt_dir)
-
-        # Thumbnail 다시 옮기기
-        if does_thumbnail_exist:
-            shutil.move(alt_thumbnail_dir, realt_thumbnail_dir)
+            merged_images[(episode_no - 1)//merge_amount].append(episode)
+
+        # merge_last_bundle을 적용함
+        merged_images = sorted(merged_images.items())
+        _, last_images = merged_images[-1]
+        if merge_last_bundle and len(self._find_episode_id(last_images)) != merge_amount:
+            merged_second_last_list = merged_images[-2][1]
+            merged_second_last_list += merged_images.pop()[1]
 
-        shutil.rmtree(self.TEMP_DIR)
+        # 폴더에 넣는 과정
+        for _, images in merged_images:
+            alt_dir_name = self._make_dir_name(images)
+            images_dir = alt_webtoon_dir / alt_dir_name
+            images_dir.mkdir(parents=True, exist_ok=True)
+            for image in images:
+                image_dir = base_webtoon_dir / image
+                shutil.move(image_dir, images_dir)
 
-    def _move_dir(self, base_episode_dir, alt_webtoon_dir, ignore_folders=False, rename=False, episode_name=None):
+    def _move_thumbnail(self, base_webtoon_dir, alt_webtoon_dir):
+        if self._is_unified(base_webtoon_dir):
+            logging.debug('Webtoon look unified already, so _move_thumbnail is skipped.')
+            return
+        for episode_or_thumbnail in os.listdir(base_webtoon_dir):
+            if re.match(r'.+[.](jpg|jpeg|png)$', episode_or_thumbnail, re.I):
+                base_thumbnail_dir = base_webtoon_dir / episode_or_thumbnail
+                alt_thumbnail_dir = alt_webtoon_dir / episode_or_thumbnail
+                shutil.move(base_thumbnail_dir, alt_thumbnail_dir)
+                return
+            
+    ############### SUB FUNCTIONALITY ###############
+
+    def _make_dir_name(self, images):
+        episode_id = self._find_episode_id(images)
+        # episode_id = set(int(image.split('.')[0]) for image in images)
+        return f'{min(episode_id):04d}~{max(episode_id):04d}'
+    
+    @staticmethod
+    def _find_episode_id(images):
+        return {int(image.split('.')[0]) for image in images}
+    
+    def _move_images(self, base_episode_dir: Path, alt_webtoon_dir: Path,
+                     episode_name: str|None=None, ignore_folders: bool=False, rename: bool=False):
+        """이미지가 들어있는 폴더를 받아서 rename하거나 하지 않고 alt_webtoon_dir로 보내는 함수
+
+        Args:
+            base_episode_dir (Path): 이미지가 들어있는 폴더
+            alt_webtoon_dir (Path): 이미지를 보낼 폴더
+            episode_name (str): 만약 rename을 할 경우, 이름을 정하기 위한 에피소드 이름.
+            ignore_folders (bool, optional): 폴더를 무시할 지 여부. Defaults to False.
+            rename (bool, optional): 이름을 바꿀 것인지 여부. Defaults to False.
+        """
         images = os.listdir(base_episode_dir)
         if ignore_folders:
-            images = (image for image in images if not re.match(r'^([.])*((?![.]).)+$', image)) # 디렉토리(확장자가 없는 경우, 맨 앞줄 '.'은 상관없음.)이면 제거
+            # 디렉토리(확장자가 없는 경우, 맨 앞줄 '.'은 상관없음.)이면 제거
+            images = (image for image in images if not re.match(r'^([.])*((?![.]).)+$', image))
         for image in images:
-            base_image_name = rf'{base_episode_dir}/{image}'
+            base_image_name = base_episode_dir / image
             # os.rename(base_image_name, alt_image_name)
             if rename:
-                alt_image_name = rf'{alt_webtoon_dir}/{self._rename_image(image, episode_name)}'
+                alt_image_name = alt_webtoon_dir / self._rename_image(image, episode_name)
             else:
-                alt_image_name = rf'{alt_webtoon_dir}/{image}'
+                alt_image_name = alt_webtoon_dir / image
             shutil.move(base_image_name, alt_image_name)
 
-    def _rename_image(self, image_name, episode_name):
-        episode_split = re.search(r'^(\d+)[.] (.+)', episode_name)
-        image_no, image_extension = image_name.split('.')[0], image_name.split('.')[-1]
-        return f'{episode_split.group(1)}.{image_no}. {episode_split.group(2)}.{image_extension}'
-    
-    def _make_dir_name(self, base_webtoon_dir):
-        episode_id = set([int(image.split('.')[0]) for image in os.listdir(base_webtoon_dir)])
-        return f'{min(episode_id):04d}~{max(episode_id):04d}'
-
-    def dividify_all_webtoon(self):
-        webtoons = os.listdir(self.BASE_DIR)
-        for webtoon in webtoons:
-            print(webtoon)
-
-            # 디렉토리 설정
-            base_webtoon_dir = rf'{self.BASE_DIR}/{webtoon}'
-            webtoon_episode_name = self._make_dir_name(base_webtoon_dir)
-            alt_webtoon_dir = rf'{self.BASE_DIR}/{webtoon}/{webtoon_episode_name}'
-
-            # 디렉토리 제작
-            self._make_directory(alt_webtoon_dir)
-            # self._make_directory(self.TEMP_FOLDER)
-
-            # 옮길 웹툰 선정
-            self._move_dir(base_webtoon_dir, alt_webtoon_dir, ignore_folders=True)
-
-            break
-
     def _unify_webtoon(self, directory):
         episodes = os.listdir(directory)
-        directory = directory[:-1] if directory[-1] == '/' or directory[-1] == '\\' else directory
-        # child_dir = re.match(r'(.+)(?=\\|\/)(?=.+?$)', directory).group() # A/B/C가 주어지만 A/B를 호출하는 regex
         for episode in episodes:
-            base_episode_dir = rf'{directory}/{episode}'
-            self._move_dir(base_episode_dir, directory, rename=True, episode_name=episode)
+            base_episode_dir = directory / episode
+            self._move_images(base_episode_dir, directory, episode, rename=True)
             os.rmdir(base_episode_dir)
+
+    def _rename_image(self, image_name, episode_name):
+        episode_split = re.search(r'^(\d+)[.] (.+)', episode_name)
+        image_no, image_extension = image_name.split('.')[0], image_name.split('.')[-1]
+        return f'{episode_split[1]}.{image_no}. {episode_split[2]}.{image_extension}'
     
     def _is_unified(self, directory):
         episodes_or_images = os.listdir(directory)
         number_of_images = 0
         for episode_or_image in episodes_or_images:
-            number_of_images += 1 if re.match(r'.+[.](jpg|jpeg|png)$', episode_or_image, re.I) else 0
+            number_of_images += 1 if re.match(r'.+[.](jpg|jpeg|png)$',
+                                              episode_or_image, re.I) else 0
         if number_of_images == 1 or number_of_images == 0:
             return False
         else:
             return True
+    
+    ############### RESTORE FUNCTIONALITY ###############
+
+    def restore_webtoons_in_directory(self):
+        webtoons = os.listdir(self.BASE_DIR)
+        for webtoon in webtoons:
+            webtoon_dir = self.BASE_DIR / webtoon
+            self.restore_webtoon(webtoon_dir)
 
-    def revert_to_original_state(self, directory):
+    def restore_webtoon(self, directory: Path):
         # Thumbnail 옮기기
-        does_thumbnail_exist, alt_thumbnail_dir, realt_thumbnail_dir = self._move_thumbnail(directory, directory)
+        temp_thumbnail_path = directory / 'thumbnail-TEMP'
+        temp_thumbnail_path.mkdir(parents=True)
+        self._move_thumbnail(directory, temp_thumbnail_path)
 
         if not self._is_unified(directory):
-            self._unify_webtoon(directory)
-        
+            # self._unify_webtoon(directory)
+            directories = os.listdir(directory)
+            directories = (directory_ for directory_ in directories
+                           if not directory_ == 'thumbnail-TEMP')
+
+            for directory_ in directories:
+                directory_ = directory / directory_
+                self._move_images(directory_, directory)
+                directory_.rmdir()
+
         images = os.listdir(directory)
+        images = (image for image in images if image != 'thumbnail-TEMP')
+
         for image in images:
-            image_nos = image.split('.')
-            episode_no = image_nos[0]
-            image_no = image_nos[1]
-            episode_name = '.'.join(image_nos[2:-1])
-            image_extension = image_nos[-1]
-            episode_dir = f'{directory}/{episode_no}.{episode_name}'
+            image_info = re.match(r'(\d+)\.(\d+)\. (.+?)\.(\w.+)', image)
+            episode_no, image_no = image_info.group(1), image_info.group(2)
+            episode_name, image_extension = image_info.group(3), image_info.group(4)
+
+            episode_dir = directory / f'{episode_no}. {episode_name}'
             alt_image_name = f'{image_no}.{image_extension}'
-            self._make_directory(episode_dir, alert=False)
-            base_image_dir = f'{directory}/{image}'
-            alt_image_dir = f'{episode_dir}/{alt_image_name}'
-            shutil.move(base_image_dir, alt_image_dir)
-        
-        # Thumbnail 다시 옮기기
-        if does_thumbnail_exist:
-            shutil.move(alt_thumbnail_dir, realt_thumbnail_dir)
-            os.removedirs(self.TEMP_DIR)
+            episode_dir.mkdir(parents=True, exist_ok=True)
+            base_image_path = directory / image
+            alt_image_path = episode_dir / alt_image_name
+            shutil.move(base_image_path, alt_image_path)
+
+        self._move_thumbnail(temp_thumbnail_path, directory)
+        temp_thumbnail_path.rmdir()
+
+if __name__ == "__main__":
+    print(os.curdir)
+    fm = FolderManager()
+    # fm.BASE_DIR = './(699830)'
+    # fm.BASE_DIR = 'webtoon/(699830)'
+    # fm.BASE_DIR = 'webtoon'
+    # fm.ALT_DIR = './going_on'
+    # fm.ALT_DIR = 'webtoon/going_on'
+    # fm.ALT_DIR = 'webtoon'
+    # print(fm.BASE_DIR, repr(fm.ALT_DIR))
+    # print(fm._BASE_DIR, repr(fm._ALT_DIR))
+    # fm.merge_webtoon_episodes(fm.ALT_DIR, fm.BASE_DIR, 5)
+    # fm.merge_webtoon_episodes(fm.BASE_DIR, fm.ALT_DIR, 5)
+    # fm.restore_webtoon(fm.ALT_DIR)
+
+    # fm.merge_webtoons_in_directory(10)
+    # fm.restore_webtoons_in_directory()
+    # fm.merge_webtoon_episodes(Path('webtoon/(699830)'), 5)
```

### Comparing `WebtoonScraper-0.1.2/WebtoonScraper.egg-info/PKG-INFO` & `WebtoonScraper-1.0.0/WebtoonScraper.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: WebtoonScraper
-Version: 0.1.2
+Version: 1.0.0
 Summary: Scraping webtoons and some utils for it
 Home-page: https://github.com/ilotoki0804/WebtoonScraper
 Author: ilotoki0804
 Author-email: ilotoki0804@gmail.com
 License: MIT
 Keywords: Webtoon,Webtoon Scraper,Naver Webtoon,Webtoon Downloader,Download Webtoon
 Classifier: License :: OSI Approved :: MIT License
@@ -14,177 +14,204 @@
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 이 설명은 최신 버전이 아닐 수 있습니다. 만약 최신 버전을 확인하고 싶으시다면 [여기](https://github.com/ilotoki0804/WebtoonScraper)를 참고하세요.
 # WebtoonScraper
 
-웹툰을 다운로드하는 프로젝트입니다. 그 외에도 웹툰 모아서 보기 등 몇 가지 편의 기능을 지원합니다.
+웹툰을 다운로드하는 프로젝트입니다.
+
+네이버 웹툰, 베스트 도전만화, 웹툰 오리지널, 웹툰 캔버스, 만화경, 버프툰, 네이버 포스트, 네이버 게임을 지원합니다.
 
-네이버 웹툰, 베스트 도전만화, 웹툰 오리지널, 웹툰 캔버스, 만화경, 버프툰, 네이버 포스트를 지원합니다.
 # 시작하기
 
 1. 파이썬을 설치합니다.
-2. cmd 창을 열어 다음과 같은 명령어를 칩니다.
-
+2. cmd 창을 열어 pip 명령어를 실행합니다.
    ```
    pip install -U WebtoonScraper
    ```
 
-   또는
+# 네이버 웹툰, 베스트 도전만화, 웹툰 오리지널, 웹툰 캔버스, 만화경, 네이버 게임 다운로드하기
 
-   ```
-   pip3 install -U WebtoonScraper
-   ```
-
-# 네이버 웹툰, 베스트 도전만화, 웹툰 오리지널, 웹툰 캔버스, 만화경 다운로드하기
 버프툰과 네이버 포스트는 아래로 가서 확인하세요.
+
 1. 원하는 웹툰으로 가서 titleid 또는 title_no를 복사하세요.
-   ![img](https://raw.githubusercontent.com/ilotoki0804/WebtoonScraper/master/naver_webtoon.png)
-   국내의 경우 여기에서,
-   ![img](https://raw.githubusercontent.com/ilotoki0804/WebtoonScraper/master/webtoons_original.png)
-   해외의 경우는 여기에서,
-   ![img](https://raw.githubusercontent.com/ilotoki0804/WebtoonScraper/master/manhwakyung.png)
-   만화경의 경우는 여기에서 확인할 수 있습니다.
-2. 다음의 파이썬 코드를 웹툰이 다운로드되길 원하는 폴더 내에서 실행해 주세요. 웹툰은 정식 연재와 베스트 도전, Webtoons 오리지널과 캔버스, 만화경 모두 가능합니다.
+   ![img](https://raw.githubusercontent.com/ilotoki0804/WebtoonScraper/master/images/naver_webtoon.png)
+   네이버 웹툰과 베스트 도전의 경우 여기에서,
+   ![img](https://raw.githubusercontent.com/ilotoki0804/WebtoonScraper/master/images/webtoons_original.png)
+   웹툰 오리지널과 캔버스의 경우는 여기에서,
+   ![img](https://raw.githubusercontent.com/ilotoki0804/WebtoonScraper/master/images/manhwakyung.png)
+   만화경의 경우는 여기에서,
+   ![img](https://raw.githubusercontent.com/ilotoki0804/WebtoonScraper/master/images/naver_game.png)
+   네이버 게임 오리지널 시리즈의 경우는 여기에서 확인할 수 있습니다.
+2. 다음의 파이썬 코드를 웹툰이 다운로드되길 원하는 폴더 내에서 실행해 주세요. 웹툰은 정식 연재와 베스트 도전, Webtoons 오리지널과 캔버스, 만화경, 네이버 게임 모두 가능합니다.
 
    ```python
    from WebtoonScraper import Webtoon as wt
 
    # 네이버 웹툰
    wt.get_webtoon(76648, wt.N) # titleid를 여기에다 붙여넣으세요.
    # 베스트 도전만화
    wt.get_webtoon(763952, wt.B) # titleid를 여기에다 붙여넣으세요.
    # 웹툰 오리지널
    wt.get_webtoon(1435, wt.O) # titleid를 여기에다 붙여넣으세요.
    # 웹툰 캔버스
    wt.get_webtoon(304446, wt.C) # titleid를 여기에다 붙여넣으세요.
    # 만화경
    wt.get_webtoon(146, wt.M) # titleid를 여기에다 붙여넣으세요. Webtoon.T 태그도 사용 가능합니다.
+   # 네이버 게임 오리지널 시리즈
+   wt.get_webtoon(146, wt.G) # titleid를 여기에다 붙여넣으세요.
    ```
 
    이제 웹툰이 webtoons 폴더에 다운로드됩니다.
 
-   cf. 웹툰 태그를 생략하면 해당 웹툰이 어떤 사이트의 웹툰 id인지 자동으로 알아냅니다. 하지만 이 방식은 서로 다른 사이트에서 id가 겹치는 웹툰이 존재하면 오작동할 수 있으니 꼭 태그를 붙이는 것을 추천합니다.
+   cf. 웹툰 태그를 생략하면 해당 웹툰이 어떤 사이트의 웹툰 id인지 자동으로 알아냅니다. 만약 몇몇 태그가 겹친다면 태그에 맞는 수를 입력하는 창에 알맞은 수를 입력하면 됩니다.
 
    또 merge 태그를 이용하면 webtoon 폴더 내에 있는 모든 웹툰을 자동으로 5화씩 묶습니다.
 3. 만화 뷰어 앱을 통해 다운로드한 웹툰을 시청할 수 있습니다.
 
 ## 주의사항
 
 * 중간에 웹툰 다운로드가 멈춘 듯이 보여도 정상입니다. 그대로 가만히 있으면 다운로드가 다시 진행됩니다.
-* 만약 작동하지 않는다면 윈도우에서 Python 3.11.3을 설치하고 앞의 과정을 반복해 보세요.
+* 만약 작동하지 않는다면 윈도우에서 Python 3.11.4을 설치하고 앞의 과정을 반복해 보세요.
 
 # 버프툰 다운로드하기
-## 로그인하지 않은 상태에서 웹툰 다운로드하기(추천하지 않음)
+
+## 로그인하지 않은 상태에서 웹툰 다운로드하기
+
 로그인하지 않은 상태에서도 웹툰을 다운로드받을 수 있으나, 받을 수 있는 웹툰 수가 매우 적기에 추천하지 않습니다.
-1. 웹툰 페이지에 들어가 주소창의 맨 마지막 숫자를 복사합니다.
+
+1. 웹툰 페이지에 들어가 주소창의 맨 마지막 수를 복사합니다.
 2. 다음의 파이썬 코드를 웹툰이 다운로드되길 원하는 폴더 내에서 실행해 주세요.
    ```python
    from WebtoonScraper import Webtoon as wt
 
-   wt.get_webtoon(1007888, wt.BU) # 복사했던 숫자를 여기에다 붙여넣으세요.
+   wt.get_webtoon(1007888, wt.BU) # 복사했던 수를 여기에다 붙여넣으세요.
    ```
 3. 'Enter cookie of 1007888(시리즈 id) (Enter nothing to preceed without cookie)'라는 문구와 함께 입력란이 나오면 그냥 enter를 눌러줍니다.
 4. 로그인하지 않고 볼 수 있는 모든 에피소드가 다운로드됩니다.
+
 ## 로그인한 상태에서 웹툰 다운로드하기
-1. 웹툰 페이지에 들어가 주소창의 맨 마지막 숫자를 복사합니다.
-2. 로그인을 하고 f12를 누르고 네트워크 창을 연 뒤 아무 웹툰이나 들어갑니다.
-3. 아무 요청이나 클릭하고 나온 창에 '머리글' 탭을 엽니다.
+
+이 과정은 PC를 기준으로 설명합니다. 만약 모바일이라면 Kiwi Browser 등을 통해 다음의 과정을 수행할 수 있습니다.
+
+1. 웹툰 페이지에 들어가 주소창의 맨 마지막 수를 복사합니다. 이 예시에서는 1007888입니다.
+   ![img](https://raw.githubusercontent.com/ilotoki0804/WebtoonScraper/master/images/bufftoon1.png)
+2. 로그인을 하고 f12를 누르고 네트워크 창을 연 뒤 웹툰 페이지에 들어갑니다.
+   ![img](https://raw.githubusercontent.com/ilotoki0804/WebtoonScraper/master/images/bufftoon2.png)
+3. 새로고침을 한 뒤 '이름'에 있는 favicon.ico 요청을 클릭하고 나온 창에 '헤더' 탭을 엽니다.
+   ![img](https://raw.githubusercontent.com/ilotoki0804/WebtoonScraper/master/images/bufftoon3.png)
 4. 내려서 Cookie: 라고 되어 있는 모든 내용을 복사합니다.
+   ![img](https://raw.githubusercontent.com/ilotoki0804/WebtoonScraper/master/images/bufftoon4.png)
 5. 다음의 파이썬 코드를 웹툰이 다운로드되길 원하는 폴더 내에서 실행해 주세요.
+
    ```python
    from WebtoonScraper import Webtoon as wt
 
-   wt.get_webtoon(1007888, wt.BU) # 첫 번째로 복사했던 숫자를 여기에다 붙여넣으세요.
+   wt.get_webtoon(1007888, wt.BF) # 첫 번째로 복사했던 수를 여기에다 붙여넣으세요.
    ```
+
    혹은 다음과 같이 cookie를 코드 내에 포함할 수도 있습니다.
+
    ```python
    from WebtoonScraper import Webtoon as wt
    cookie = '두 번째로 복사했던 문자를 여기에다 붙여넣으세요.'
-   wt.get_webtoon(1007888, wt.BU, cookie=cookie) # 첫 번째로 복사했던 숫자를 여기에다 붙여넣으세요.
+   wt.get_webtoon(1007888, wt.BF, cookie=cookie) # 첫 번째로 복사했던 수를 여기에다 붙여넣으세요.
    ```
-6. 'Enter cookie of 1007888(시리즈 id) (Enter nothing to preceed without cookie)'라는 문구와 함께 입력란이 나오면 두 번째로 복사했던 일련의 문자열을 붙여넣기합니다.
-4. 로그인하면 볼 수 있는 모든 에피소드가 다운로드됩니다.
+
+   1. 'Enter cookie of 1007888(시리즈 id) (Enter nothing to proceed without cookie)'라는 문구와 함께 입력란이 나오면 두 번째로 복사했던 일련의 문자열을 붙여넣기합니다.
+6. 로그인하면 볼 수 있는 모든 에피소드가 다운로드됩니다.
 
 ## 주의사항
-* 버프툰은 titleid를 자동으로 알아내지 않습니다. 하지만 cookie를 입력하면 자동으로 버프툰으로 인식합니다.
+
+* get_webtoon에서 cookie를 입력하면 자동으로 버프툰으로 인식합니다.
 
 # 네이버 포스트 다운로드하기
 
 1. 웹툰이 있는 페이지로 가서 seriesNo와 memberNo를 복사하세요. 예시에서는 각각 597061과 19803452입니다.
-   ![img](https://raw.githubusercontent.com/ilotoki0804/WebtoonScraper/master/naver_post.png)
+   ![img](https://raw.githubusercontent.com/ilotoki0804/WebtoonScraper/master/images/naver_post.png)
 2. 다음의 파이썬 코드를 웹툰이 다운로드되길 원하는 폴더 내에서 실행해 주세요.
+
    ```python
    from WebtoonScraper import Webtoon as wt
 
    wt.get_webtoon(597061, wt.M) # 우선 seriesNo만 여기에 입력해주세요.
    ```
-   혹은 memberNo를 코드 내에 포함할 수 있습니다. 
+
+   혹은 memberNo를 코드 내에 포함할 수 있습니다.
+
    ```python
    from WebtoonScraper import Webtoon as wt
 
-   wt.get_webtoon(597061, wt.M, member_no='19803452')
+   wt.get_webtoon(597061, wt.M, member_no=19803452)
    ```
 3. 'Enter memberNo of 597061(해당 웹툰의 seriesNo)'라는 말과 함께 입력란이 나오면 거기에 아까 복사해 놓은 memberNo를 붙여넣습니다.
    만약 앞에서 이미 member_no를 사용했다면 이 단계는 건너뛰어집니다.
+
    ```
    Enter memberNo  of 597061: 19803452
    ...진행됨...
    ```
 4. 만화 뷰어 앱을 통해 다운로드한 웹툰을 시청할 수 있습니다.
+
 ## 주의사항
+
 * 가끔씩 이유 없는 오류가 발생할 수 있습니다. 그럴 때는 조금 시간이 지난 후에 다시 시도해 보세요.
-* 네이버 포스트는 titleid를 자동으로 알아내지 않습니다. 하지만 member_no를 입력하면 자동으로 포스트로 인식합니다.
+* 네이버 포스트는 titleid를 get_webtoon_platform으로 알아낼 수 없습니다.
+* member_no를 입력하면 자동으로 포스트로 인식됩니다.
+
 # 여러 회차 하나로 묶기
 
 1. 웹툰을 상기한 대로 다운로드받습니다.
 2. 다음과 같이 코드를 짭니다.
    ```python
-   from WebtoonScraper import *
+   from WebtoonScraper import FolderManager
 
-   folder = WebtoonFolderManagement('webtoon_merge')
-   folder.divide_all_webtoons(5)
+   fm = FolderManager()
+   fm.divide_all_webtoons(5)
    ```
 3. webtoons 폴더에 있는 **모든** 웹툰이 'webtoon_merge' 폴더에 5화씩 묶여져 다운로드됩니다.
 
 ## 주의사항
 
 * 시작 시 꼭 디렉토리를 선택해 주세요. 아니면 오류가 납니다.
 * 작업 중간에 폴더가 사라지고 이미지가 폴더 밖으로 나오는데, 이는 정상 과정입니다.
-* 너무 큰 숫자를 입력하면 웹툰 뷰어가 제대로 작동하지 않을 수 있음을 유의하세요.
+* 너무 큰 수를 입력하면 웹툰 뷰어가 제대로 작동하지 않을 수 있음을 유의하세요.
 
 # 묶인 회차 다시 원래대로 되돌리기
 
 1. 윗글의 기능으로 묶인 회차를 준비합니다.
 2. 다음과 같이 코드를 짭니다.
    ```python
-   from WebtoonScraper import *
+   from WebtoonScraper import FolderManager
 
-   folder = WebtoonFolderManagement('webtoon_merge')
-   folder.revert_to_original_state('webtoon/1초(725586)')
+   fm= FolderManager()
+   fm.restore_webtoons_in_directory('webtoon/1초(725586)')
    ```
 3. 'webtoon/1초(725586)' 폴더에 있던 모든 웹툰이 웹툰을 처음 다운로드했던 상태로 되돌아갑니다.
 
 # QNA
 
-## 회차가 띄엄띄엄 있거나 설정된 회차 번호가 작가가 설정한 회차 번호와 다릅니다./회차 묶기를 사용했는데 묶인 회차 수가 설정한 수보다 더 적습니다.
+## 회차 번호 관련
 
-### 생기는 이유
+### 문제와 이유
 
+회차가 띄엄띄엄 있거나 설정된 회차 번호가 작가가 설정한 회차 번호와 다르거나 회차 묶기를 사용했는데 묶인 회차 수가 설정한 수보다 더 적은 이유는 다음과 같습니다.
 이 프로젝트에서 웹툰의 회차 번호는 ID를 기준으로 합니다. 이는 작가가 정한 회차와는 다를 수 있습니다. 작가가 프롤로그부터 시작하는 경우(프로젝트의 회차 번호가 하나 빠름), 작가가 리메이크를 해서 전에 있던 작품을 제거해 ID가 연속적으로 있지 않는 경우(주로 베도에서 일어남/회차 번호가 띄엄띄엄하게 있음), 논란이나 작가 실수 등으로 회차가 삭제된 경우(한 회차를 건너띔) 등에서 ID가 불연속적이거나 작품과 일치하기 않는 경우가 생기게 됩니다.
 
 ### ID를 회차 번호로 그대로 사용하는 이유
 
 우선 작가가 설정한 회차 번호에 맞추는 것은 힘듭니다. 우선 번호가 어디에 있을지 알기 어렵고, 프롤로그가 있을지 없을지 알 수 없으며, 여러 화에 걸쳐 같은 에피소드를 진행하는 경우도 있고, 외전으로 본편의 회차에서 분리된 화를 운영하는 경우가 있어 화에 맞추어서 번호를 정하는 것을 어렵습니다.
 1부터 시작해서 끝까지 일정한 번호를 유지하는 것도 고려해볼 만하나 만약 그렇게 된다면 무결성 체크를 사용하기 어렵게 됩니다.
 따라서 작가가 설정한 회차를 그대로 사용하는 것도 어렵고, 만약 가능하다 할 지라도 무결성 체크를 포기하기 어렵기 때문에 현재는 ID를 회차 번호로 사용하고 있습니다.
 
 # Relese Note
 
+1.0.0: 네이버 게임 추가, FolderManager 리펙토링 및 개선, 정식 버전, docs 개선
+
 0.1.1: 네이버 포스트 추가, readme 작성, pbar 표시 내용 변경, 버그 수정
 
 0.1.0: 버프툰 추가, 빠진 부분 재추가
 
 0.0.19.3: merge 속성 추가, get_webtoon 함수로 변경
 
 0.0.19.1: pbar에 표시되는 내용 변경, 내부적 개선
```

### Comparing `WebtoonScraper-0.1.2/WebtoonScraper.egg-info/SOURCES.txt` & `WebtoonScraper-1.0.0/WebtoonScraper.egg-info/SOURCES.txt`

 * *Files 14% similar despite different names*

```diff
@@ -1,22 +1,23 @@
 LICENSE
 MANIFEST.in
 README.md
 setup.py
 WebtoonScraper/BestChallengeScraper.py
 WebtoonScraper/BufftoonScraper.py
+WebtoonScraper/FolderManager.py
+WebtoonScraper/NaverGameScraper.py
 WebtoonScraper/NaverPostScraper.py
 WebtoonScraper/NaverWebtoonScraper.py
 WebtoonScraper/Scraper.py
 WebtoonScraper/TelescopeScraper.py
 WebtoonScraper/Webtoon.py
 WebtoonScraper/WebtoonCanvasScraper.py
 WebtoonScraper/WebtoonOriginalsScraper.py
 WebtoonScraper/__init__.py
-WebtoonScraper/foldermanagement.py
 WebtoonScraper.egg-info/PKG-INFO
 WebtoonScraper.egg-info/SOURCES.txt
 WebtoonScraper.egg-info/dependency_links.txt
 WebtoonScraper.egg-info/not-zip-safe
 WebtoonScraper.egg-info/requires.txt
 WebtoonScraper.egg-info/top_level.txt
 test/test.py
```

### Comparing `WebtoonScraper-0.1.2/setup.py` & `WebtoonScraper-1.0.0/setup.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 from setuptools import setup, find_packages
+import re
 
 with open('README.md', 'r', encoding='utf-8') as f:
     long_description = '이 설명은 최신 버전이 아닐 수 있습니다. 만약 최신 버전을 확인하고 싶으시다면 [여기](https://github.com/ilotoki0804/WebtoonScraper)를 참고하세요.\n'
     long_description += f.read()
-    long_description = long_description.replace('naver_webtoon.png', 'https://raw.githubusercontent.com/ilotoki0804/WebtoonScraper/master/naver_webtoon.png')
-    long_description = long_description.replace('webtoons_original.png', 'https://raw.githubusercontent.com/ilotoki0804/WebtoonScraper/master/webtoons_original.png')
-    long_description = long_description.replace('manhwakyung.png', 'https://raw.githubusercontent.com/ilotoki0804/WebtoonScraper/master/manhwakyung.png')
-    long_description = long_description.replace('naver_post.png', 'https://raw.githubusercontent.com/ilotoki0804/WebtoonScraper/master/naver_post.png')
+    # 사진 대체
+    repl = '![\g<1>](https://raw.githubusercontent.com/ilotoki0804/WebtoonScraper/master/\g<2>)'
+    long_description = re.sub(r'!\[(.+?)\]\((images\/.+?)\)', repl, long_description)
 
 setup(
     name='WebtoonScraper',
-    version='0.1.2',
+    version='1.0.0',
     description='Scraping webtoons and some utils for it',
     author='ilotoki0804',
     author_email='ilotoki0804@gmail.com',
     long_description=long_description,
     long_description_content_type='text/markdown',
     license='MIT',
     url='https://github.com/ilotoki0804/WebtoonScraper',
```

