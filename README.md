# CS3219 OTOT Task A1

## Steps

-   `git clone https://github.com/aizatazhar/poopypants.git`
-   `cd poopypants`
-   `docker-compose build`
-   `docker-compose up`

---

## Task instructions

CS3219 OTOT Task A1 is split into 3 parts. Read up on reverse proxy [here](https://www.upguard.com/blog/reverse-proxy-vs-load-balancer).

First, clone the repository

```sh
git clone https://github.com/marcustw/ay2022-23_cs3219_otot_taska1 cs3219_otot_taska1
cd cs3219_otot_taska1
```

### A1.1 - Dockerize node app in `app` folder

In the `app/index.html` file, search for "TODO" and fill in the blanks.

Follow these guide to Dockerize the sample node app.

-   [https://codeforgeek.com/render-html-file-expressjs/](https://codeforgeek.com/render-html-file-expressjs/)
-   [https://www.cloudbees.com/blog/using-docker-compose-for-nodejs-development](https://www.cloudbees.com/blog/using-docker-compose-for-nodejs-development)
-   [https://expressjs.com/en/starter/hello-world.html](https://expressjs.com/en/starter/hello-world.html)

### A1.2 - Dockerize NGINX reverse proxy in `nginx-sample` folder

In the `nginx-sample/index.html` file, search for "TODO" and fill in the blanks.

Follow these guide to dockerise the sample NGINX reverse proxy to serve the static HTML in `nginx/index.html`.

-   [https://docs.nginx.com/nginx/admin-guide/web-server/serving-static-content/](https://docs.nginx.com/nginx/admin-guide/web-server/serving-static-content/)
-   [https://docs.nginx.com/nginx/admin-guide/web-server/reverse-proxy/](https://docs.nginx.com/nginx/admin-guide/web-server/reverse-proxy/)
-   [https://www.nginx.com/blog/deploying-nginx-nginx-plus-docker/](https://www.nginx.com/blog/deploying-nginx-nginx-plus-docker/)

### A1.3 - Use NGINX to serve the node app using `docker-compose`

Create a new NGINX conf file and Dockerfile in `nginx` folder. Run the application stack in `app` and `nginx` using `docker-compose`.

Follow this guide to use NGINX to act as a reverse proxy such that when a browser makes a HTTP request, the request first goes to the reverse proxy and then sends the request to the appropriate web server. Your final task, you have to server the node app in `app` folder. Use a separate config file from A1.2.

-   [https://ashwin9798.medium.com/nginx-with-docker-and-node-js-a-beginners-guide-434fe1216b6b](https://ashwin9798.medium.com/nginx-with-docker-and-node-js-a-beginners-guide-434fe1216b6b)
