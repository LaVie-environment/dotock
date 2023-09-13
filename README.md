Run the web container
> docker container run --detach --publish 8088:80 diamol/ch02-hello-diamol-web
20ed16e2ca44736e2ed05129c339b693fcd9b42cdabc0ba930f5f365339a5479

Check the HTML page in the container is in the expected location:
> docker container exec 20e  ls /usr/local/apache2/htdocs
index.html

Browse to the published port on http://localhost:8088 - to see the content:
image.png

![image](https://github.com/LaVie-environment/dotock/assets/19356065/ae68cdc0-c201-4d16-b018-e1896811f4c1)

