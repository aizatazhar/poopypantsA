# AY2022/23 CS3219 Task A1 - Dockerizing the NGINX reverse proxy

There is a static `index.html` file. Your task is to serve this static html page using NGINX reverse proxy.

-   `docker build -t nginx-sample .`
-   `docker run -it --rm -d -p 8080:80 --name nginx-sample nginx-sample`
-   go to localhost:8080
-   `docker stop nginx-sample` to stop
