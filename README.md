## dockertraining
[$ Git clone https://github.com/bbachi/angular-nodejs-example.git]
* Selected sample gulpfile.js as source code .
## Dockerfile for apline image using Vi editor by $ vi Dockerfile"
```
(FROM node:alpine 
RUN mkdir mytemp
COPY gulpfile.js /mytemp/gulpfile.js  
COPY . /mytemp/
CMD ["npm" "start"])
```
## Created another image using same code With new Dockefile
```
(FROM node:latest
RUN mkdir mytemp
COPY gulpfile.js /mytemp/gulpfile.js  
COPY . /mytemp/
CMD ["npm" "start"])
```
## Created docker image using 
```
$ "docker build -t myangular_alpinejs:1.0 ."
```
## To confrim that  docker image is  build  , use
```
$ "docker images "
```

* After successfull completion of docker image by using below command created conatiner myangular_alpinejs:1.0

```
 $ "docker run -itd --name angularjs_sample myangular_alpinejs:1.0"
```

## creating new repository in git hub named "dockertraining" 
* sucessfully cloned "docker training repository"by using 
```
 "git clone git@github.com:Prem2212/dockertraining.git"
```
*  To local machine.
*   Genrated ssh public and private key and adding public key to git hub ,by following the guide (https://docs.github.com/en/authentication/connecting-to-github-with-ssh/generating-a-new-ssh-key-and-adding-it-to-the-ssh-agent).

* After cloning , adding lab1 and lab-angular-js directories  which contain source code and Dockrfile to the dockertraining reposistory .
By using 
```
"git add lab1 lab-angular-js/"
```
* adding file to stating area and ready for commit.
```
"git commit -am "new docker images "
``` 
* successful commited files .
* pushed the local reposistory to the git hub and it is successful by using below command.

```
" git push "
``` 
