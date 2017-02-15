curl 使用
https://curl.haxx.se/docs/manpage.html
在chrome中 在XHR可以copy as cURL

* -H添加header

```
-H 'Referer: https://www.sighthound.com/products/cloud' -H 'Origin: https://www.sighthound.com' -H 'User-Agent: Mozilla/5.0 (Macintosh; Intel Mac OS X 10_12_3) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/56.0.2924.87 Safari/537.36'
```

* 添加时间 -w选项

```
%{speed_upload}:%{speed_download}:%{time_appconnect}:%{time_connect}:%{time_namelookup}:%{time_pretransfer}:%{time_redirect}:%{time_starttransfer}:%{time_total}
```

* POST data -D --data-binary或者用-F multipart POST data

```
--data_binary @"filepath"
or
-F "filecomment=This is an image file" \
-F "image=@/home/user1/Desktop/test.jpg" \
 ```