# 关于Szuba的开发

### os:windows 64bit

## 1.创建虚拟环境(无其他库)
   1. python -m venv venvname在当前目录创建一个虚拟环境
   2. windows激活 进入目录下 运行activate
   3. pip config set global.index-url https://mirrors.aliyun.com/pypi/simple/      换源
   4. python -m pip install --upgrade pip 更新pip
   
## 2.安装所需安装包 
   1. pip freeze > filename.txt(在目录中导出所需安装包)
   2.  pip install -r filename.txt(一键安装)
   3. **conda install ffmpeg -c conda-forge**

## 3. 打包成exe
   1. pip install pyinstaller
   2. * pyinstaller -F -w --hidden-import pydicom.encoders.gdcm --hidden-import pydicom.encoders.pylibjpeg szuba.py
         * -F  打包成一个exe
         * -w  无控制台模式
         * -i  将图标导入exe
       * 配置spec文件(可以对依赖文件进行打包、内部的文件在exe解压时可以自动解压到临时目录，在程序关闭时可以删除，exe更加简化)
          * 
```python 
def resource_path(relative_path):
   if getattr(sys, 'frozen', False): #是否Bundle Resource
      base_path = sys._MEIPASS
   else:
   base_path = os.path.abspath(".")
   return os.path.join(base_path, relative_path)

filepathwavs = resource_path(os.path.join("wav","clearly-602.wav"))
filepathwavq = resource_path(os.path.join("wav","done-for-you-612.wav"))
filepathwavn = resource_path(os.path.join("wav","all-of-a-sudden-405.wav"))
```
修改spec
           
   