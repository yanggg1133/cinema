### 要求
```
1 .php 7.1以上
```
```
2 php.ini 开放 proc_open exec shell_exec
```

### 第一个座位不能选择
```
1. 配置 .env
```
```
2. composer install 
```
```
3. php artisan key:generate
```
```
4. php artisan cinema:init
```
```
PS: screen and user 需要填充数据
```
###调试信息
```
详细页面出现错误

C:\phpStudy\WWW\9.com\cinema-master\app\Http\Controllers\HomeController.php

78行
        $cinemas = $this->getApi($url);
        dd($cinemas);
        
原因是        //获取影院信息
        $url = 'http://m.maoyan.com/cinemas.json';
        猫眼的api失效了

```
