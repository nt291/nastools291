
# nt292媒体库管理工具
致敬nastools,以nastools2.9.2为基础开发。

API: http://localhost:3000/api/v1/


## 功能：

NAS媒体库管理工具。
默认账号密码：admin/password


## 安装
### 1、Docker
```
docker pull jxxghp/nas-tools:latest
```

如无法连接Github，注意不要开启自动更新开关(NASTOOL_AUTO_UPDATE=false)，将NASTOOL_CN_UPDATE设置为true可使用国内源加速安装依赖。

### 2、本地运行
python3.11版本，需要预安装cython，如发现缺少依赖包需额外安装
```
git clone -b master https://github.com/jxxghp/nas-tools --recurse-submodule 
python3 -m pip install -r requirements.txt
export NASTOOL_CONFIG="/xxx/config/config.yaml"
nohup python3 run.py & 
```

### 3、Windows
下载exe文件，双击运行即可，会自动生成配置文件目录

https://github.com/jxxghp/nas-tools/releases


### 4、变更点

* 使用poetry管理python依赖
* 升级python 3.11.x，开发时使用poetry:1.5.1 python:3.11.4