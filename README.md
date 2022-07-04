# v.hbu.cn
盒带教务系统


* 登录webvpn

  post
    https://v.hbu.cn/do-login

headers  

    Host: v.hbu.cn  
    User-Agent: Mozilla/5.0 (Windows NT 10.0; Win64; x64; rv:102.0) Gecko/20100101 Firefox/102.0  
    Accept: */*  
    Accept-Language: zh-CN,zh;q=0.8,zh-TW;q=0.7,zh-HK;q=0.5,en-US;q=0.3,en;q=0.2  
    Content-Type: application/x-www-form-urlencoded; charset=UTF-8  
    X-Requested-With: XMLHttpRequest  
    Origin: https://v.hbu.cn
    Connection: keep-alive  
    Referer: https://v.hbu.cn/login  
    Sec-Fetch-Dest: empty  
    Sec-Fetch-Mode: cors  
    Sec-Fetch-Site: same-origin  
    Cache-Control: no-cache  
    Accept-Encoding: gzip, deflate  
    Content-Length: 119  
  
  body
auth_type=local&username=学号&sms_code=&password=密码&captcha=&needCaptcha=false


返回的响应头中会出现  
Set-Cookie: wengine_vpn_ticketv_hbu_cn=  
wengine_vpn_ticketv_hbu_cn做为cookie使用  

* 登陆教务系统

  post  
    https://v.hbu.cn/http/77726476706e69737468656265737421eaff4b8b69386a45300b87/sigin

headers  

    Host: v.hbu.cn  
    User-Agent: Mozilla/5.0 (Windows NT 10.0; Win64; x64; rv:102.0) Gecko/20100101 Firefox/102.0  
    Accept: text/html,application/xhtml+xml,application/xml;q=0.9,image/avif,image/webp,*/*;q=0.8  
    Accept-Language: zh-CN,zh;q=0.8,zh-TW;q=0.7,zh-HK;q=0.5,en-US;q=0.3,en;q=0.2  
    Content-Type: application/x-www-form-urlencoded  
    Origin: https://v.hbu.cn  
    Connection: keep-alive  
    Referer: https://v.hbu.cn/http/77726476706e69737468656265737421eaff4b8b69386a45300b87/login  
    Cookie: show_vpn=0; show_faq=0; wengine_vpn_ticketv_hbu_cn=上一次请求返回的cookie; remember_token=; refresh=1  
    Upgrade-Insecure-Requests: 1  
    Sec-Fetch-Dest: document  
    Sec-Fetch-Mode: navigate  
    Sec-Fetch-Site: same-origin  
    Sec-Fetch-User: ?1  
    Cache-Control: no-cache  
    Accept-Encoding: gzip, deflate  
    Content-Length: 39  
    
  body  
username=学号&password=密码
