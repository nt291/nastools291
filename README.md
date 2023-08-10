
# nt291媒体库管理工具
致敬nastools

API: http://localhost:3000/api/v1/


## 功能：

NAS媒体库管理工具。


## 安装
### 1、Docker
```
docker pull jxxghp/nas-tools:latest
```

如无法连接Github，注意不要开启自动更新开关(NASTOOL_AUTO_UPDATE=false)，将NASTOOL_CN_UPDATE设置为true可使用国内源加速安装依赖。

### 2、本地运行
python3.10版本，需要预安装cython，如发现缺少依赖包需额外安装
```
git clone -b master https://github.com/jxxghp/nas-tools --recurse-submodule 
python3 -m pip install -r requirements.txt
export NASTOOL_CONFIG="/xxx/config/config.yaml"
nohup python3 run.py & 
```

### 3、Windows
下载exe文件，双击运行即可，会自动生成配置文件目录

https://github.com/jxxghp/nas-tools/releases

### 4、群晖套件
添加矿神群晖SPK套件源直接安装：

https://spk.imnks.com/

https://spk7.imnks.com/
