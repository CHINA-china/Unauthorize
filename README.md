# Unauthorized

### 一款高效率的前端未授权访问检测工具


![logo](.\static\logo.png)

## 工具特点

- 内置常见高频未授权访问路径字典
- 自动从前端js文件中提取泄露的接口进行测试
- 采用selenium框架实现对“#”传参网址的测试

## 环境搭建

- **安装依赖库**
```
pip install -r requirements.txt
```

- **下载浏览器driver驱动**

- 查看浏览器版本
![chrome](.\static\picture\Install\chrome.png)
- 下载对应版本驱动（若没有对应版本，可下载相近版本）
```
下载地址：https://registry.npmmirror.com/binary.html?path=chromedriver/                                  
```

![chrome](.\static\picture\Install\drive1.png)

![chrome](.\static\picture\Install\drive2.png)
- 将driver移动到python3根目录
![chrome](.\static\picture\Install\python3.png)

## 使用

- **简单使用**

- ❌使用姿势-->直接传入域名
- ✔使用姿势-->将需要访问的网址先用浏览器访问一遍，再复制地址传入
```
python Unauthorized.py -u http://example.com
```
- **扩展使用**

- -d 指定自定义的字典(不使用该参数，程序将使用默认字典)
```
python Unauthorized.py -u http://example.com -d 自定义字典路径
```

## 引用
- 默认字典来自以下优先项目：
  1. RouteVulScan (https://github.com/F6JO/RouteVulScan)






