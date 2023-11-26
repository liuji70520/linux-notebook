# 下载文件
## 使用 nohup 命令在后台启动 wget 进程，递归下载所有文件，并指定下载目录(可以配合screen命令创建新窗口)
```bash
screen
```
```python3
nohup wget -r -P my_custom_directory ftp://ftp.cngb.org/pub/CNSA/data3/CNP0001565/zeamap/99_MaizegoResources/01_CUBIC_related/Genotype/hybrid42k/ &
```
nohup 命令用于在后台运行 wget，& 用于将其挂起。
-r 选项用于递归下载所有文件。
-P 选项用于定义下载目录名称。
my_custom_directory 是指定的下载目录。  
ftp://ftp.cngb.org/pub/CNSA/data3/CNP0001565/zeamap/99_MaizegoResources/01_CUBIC_related/Genotype/hybrid42k/ 是要下载的目录的 URL。

在 Screen 会话中分离：
按下快捷键 Ctrl + A，然后按下 d。
# 将 .ipynb 文件转换为 .py
## 安装 nbconvert 工具
```bash
pip install nbconvert
```
## 使用 nbconvert 将 .ipynb 文件转换为 .py 文件    
```bash              
jupyter nbconvert --to script AA531coding.ipynb
```


