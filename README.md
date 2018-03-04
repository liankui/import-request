# import-request
爬取网页的通用代码框架
import requests
def getHTMLText(url):
    try:
        r = requests.get(url, timeout=30)
        r.raise_for_status()
        r.encoding = r.apparent_encoding
        return r.text
    except:
        return "产生异常"
if _name_ =="_main_";
    url = "http://www.baidu.com"
    print(getHTMLText(url))
suibianx写下的内容，你不知道多少人比你更自律。
