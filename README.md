# nginx-docker

hosting simple static page on nginx using docker container

Steps:
1.Create repo in github:
  git init nginx-docker

2.Clone repo and open it:
  git clone https://github.com/RahulX7r/nginx-docker.git
  cd nignx-docker

3.Create Dockerfile in repo:
  nano Dockerfile
  #Dockerfile for nginx
    FROM nginx:latest
    COPY web /usr/share/nginx/html
    EXPOSE 80

4.Create directory in repo and add index.html file:
  mkdir web
  nano index.html
  #simple web page
  <html>
    <h1> Hello from Nginx </h1>
  </html

5.Add, commit and push files to repo:
  git add .
  git commit -m "adding Dockerfile and code"
  git push origin main

6.Build Dockerfile and run container:
  docker build -t simple-app 
  docker run -itdp 8090:80 simple-app 

7.Test website:

  ![image](https://github.com/user-attachments/assets/9d2000cd-7bc9-41a9-8738-06643d5e5a93)

  
  
