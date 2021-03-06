# Morning Knowing App

>It's like a clock with weather in more.

>The morning, when you prepare you can adjust your clothes depending the weather or never forgot the time by checking the app instead of looking for your smartphone.

![Screen web App](http://137.74.199.46/images.png)

## Install

There is a Docker integration for installing more easily.

In first, you have to install docker on the machine who will host the container, with one of this command :

- ```curl -sSL https://get.docker.com/ | sh```
- ```wget -qO- https://get.docker.com/ | sh``` 
- https://docs.docker.com/engine/installation/

Once Docker is installed, if you are on Mac or Windows, docker-compose is installed with it, so you have no problem to continue.

If you are on Linux, the best way to install docker-compose is by installing with pip packet manager with the following command :
```
 sudo easy_install pip
 sudo pip3 install docker-compose
```

For device using ARM and not x86_64 processors, docker is not implemented yet.

Then, once docker is installed go to the root directory of the project and type : 
 ```
    cd Docker/
    sudo docker-compose up -d 
  ```
Now, you should see running the app at **http://ip_server**

## Usage

Before launch the docker container, you have to fill the config file :
```
vim assets/config/config.js
```

Concerning the keys for the Weather Api, you have to create a developper account here : **https://www.wunderground.com/weather/api/** and get your api key.

Then relaunch the docker container with the same command inside the **Docker** directory :
 ```
 sudo docker-compose up -d
```

## Updates

There is a lot of things remains to be done concerning the app in particular :

- Add possibility to import theme.
- Add Customization.
- More languages friendly (Time)
- Add features like check the news of the day

## Author

Paul Rosset