# web crawler 
利用爬虫下载【新時代的我們】和【達蓋爾的旗幟】两个板块帖子内的图片 
# 环境要求
## 解释器版本
Python 3.x
## 模块列表
pip install -r requirements.txt
##  海外下载only
不设置代理，不考虑墙。 
```
 
# 使用方法
## 命令行:<br>
```python main_web_crawler.py [-h] [-c CLASS_ID] [-s START] [-e END] [-m MAX_THREAD]```<br>
```[-h]``` 显示帮助信息<br>
```[-c]``` 下载类别，```1```下载【新時代的我們】板块 , ```2```下载【達蓋爾的旗幟】板块 , ```0```同时下载两个板块<br>
```[-s]``` 下载的起始页（默认1）<br>
```[-e]``` 下载的尾页<br>
```[-m]``` 设置最大下载线程（默认60）<br>
```[-p]``` '0':禁用代理配置  默认'1'：启用代理 <br>
下载完成的图片会保存在./t66y目录
## example:<br>
```python Spider_of_t66y.py -c 1 -s 1 -e 2 -m 300```<br>
```python Spider_of_t66y.py -c 2 -p 0```<br>
```python Spider_of_t66y.py -h```<br>
