# nginx-nextjs-setting


# add this to .conf file

1. Basic
```
location /_next {
        proxy_pass http://localhost:[port];
}
```


2. In case of using Next.js `API`
```
location /api {
        proxy_pass http://localhost:[port];
}
```


3. In case of using Next.js link/routing
```
location ~ ^/([^/]+)(.*)$ {
        proxy_pass http://localhost:4030;
}
```
