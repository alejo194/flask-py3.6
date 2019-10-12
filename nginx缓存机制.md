参：https://www.cnblogs.com/kevingrace/p/6198287.html
#### proxy_cache
```bash
proxy_cache 
语法：proxy_cache zone_name ;

proxy_cache_path
语法：proxy_cache_path path [levels=number] keys_zone=zone_name:zone_size [inactive=time] [max_size=size];
例： proxy_cache_path /usr/local/nginx/proxy_cache_dir levels=1:2 keys_zone=cache_one:500m inactive=1d max_size=30g ;
path 表示存放目录
levels 表示指定该缓存空间有两层hash目录,第一层目录为1个字母,第二层目录为2个字母,
保存的文件名会类似/usr/local/nginx/proxy_cache_dir/c/29/XXXXXX ;
keys_zone参数用来为这个缓存区起名.
500m 指内存缓存空间大小为500MB
inactive的1d指如果缓存数据在1天内没有被访问,将被删除。相当于expires过期时间的配置；
max_size的30g是指硬盘缓存空间为30G

proxy_tmp_path
```
#### fastcgi_cache
```bash
fastcgi_tmp_path
```
