docker run -d --name apache -p 80:80  httpd

docker cp index.html apache:/tmp
ocker exec -it apache sh 
cd /tmp
cd /usr/local/apache2/htdocs/

docker cp index.html apache:/usr/local/apache2/htdocs/index.html