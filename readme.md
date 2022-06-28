- 把我们的项目 交给GitHub托管， 可以直接访问
    1. 这项服务的名字叫 github pages
    2. 免费的二级域名
        纯静态资源
    3. 如果push的时候使用https链接 错误：
        fatal: unable to access 'https://github.com/goldenfishzhenianqi/try-react-gh.git/': SSL certificate problem: unable to get local issuer certificate
        解决： git config --global http.sslVerify false  忽略证书错误
    
- 相对地址有问题
    工程化vite 配置， 将index.html 与 assets 的关系
    配置成 base: './'
    github 中可能有好多个项目
    /根路径

- 在GitHub 中上传了源码

- npm i gh-pages -D
    专门负责dist目录的在线访问
- package.json配置
    "deploy": "gh-pages -d dist"
