下载文件
bash
Copy code
# 使用 nohup 命令在后台启动 wget 进程，递归下载所有文件，并指定下载目录
nohup wget -r -P my_custom_directory ftp://ftp.cngb.org/pub/CNSA/data3/CNP0001565/zeamap/99_MaizegoResources/01_CUBIC_related/Genotype/hybrid42k/ &
说明：

nohup 命令用于在后台运行 wget，& 用于将其挂起。
-r 选项用于递归下载所有文件。
-P 选项用于定义下载目录名称。
my_custom_directory 是你指定的下载目录。
ftp://ftp.cngb.org/pub/CNSA/data3/CNP0001565/zeamap/99_MaizegoResources/01_CUBIC_related/Genotype/hybrid42k/ 是要下载的目录的 URL。
将 .ipynb 文件转换为 .py
bash
Copy code
# 安装 nbconvert 工具
pip install nbconvert

# 使用 nbconvert 将 .ipynb 文件转换为 .py 文件
jupyter nbconvert --to script AA531coding.ipynb
说明：

pip install nbconvert 用于安装 nbconvert 工具。
jupyter nbconvert --to script AA531coding.ipynb 用于将 Jupyter Notebook 文件 .ipynb 转换为 Python 脚本文件 .py。




