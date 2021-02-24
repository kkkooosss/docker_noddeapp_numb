# docker_noddeapp_numb
This application creates a docker container with a web server which returns a name depends on the number of port and the path.

For to build the application clone the repository and run

```
docker build -t nodeapp .
```
For to run docker container with app 1111 on port=1111 run 
```
docker run -p 1111:9999 -d -e APPID=1111 nodeapp
```
The application will be avelable on: 

- Hello page:   http://127.0.0.1:1111
- App1 page:   http://127.0.0.1:1111/app1
- App2 page:   http://127.0.0.1:1111/app2
- Admin page:   http://127.0.0.1:1111/admin
