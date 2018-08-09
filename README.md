# flask-py3.6
docker相关文件，Dockerfile,docker-compose.yml等等
用于编译docker images

#### 重要说明：
+ python docker images中安装pymssql 依赖freetds(版本是0.9几的，这个在alpine系统中下载包时v3.3环境中),
+ 这几次在build镜像时，FROM python:3.6-alpine 中会出错ERROR: unsatisfiable constraints:</br>
***解决方法FROM python:3.6-alpine3.4/python:3.6-alpine3.6</br>
python:3.6-alpine3.7也出现ERROR: unsatisfiable constraints:****
