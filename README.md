# sae-yii2-memcache
Yii2 在Sina App Engine上使用Memcache
## 安装步骤
将SaeMemcache.php 文件放入vendor/yiisoft/yii2/caching文件夹即可
文件太少就不用composer了。
## 使用方法
1. 在Sina App Engine 上初始化Memcache服务
2. 配置Memcache 组件
```
  'components' => [
    ...
    //缓存配置
    'cache' => [
      'class' => 'yii\caching\SaeMemCache',
      'keyPrefix' => 'frontend',
    ],
    ...
  ],
```  
