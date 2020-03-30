# How to install Grafana from its latest Docker Image

*Step 1. Installing Docker:*  
Using [Docker Hub Get Started Guide](https://docs.docker.com/get-started/#set-up-your-docker-environment) install and run Docker for your operation system

>*Note*: If you are on a Linux system, you might need to add `sudo` before the commands below

*Step 2. Downloading Grafana Docker Image:*  
With `docker pull grafana/grafana:latest` download the latest version of Grafana docker image. 

*Step 3. Running container:*  
Use `docker run -d -p 3000:3000 grafana/grafana` to run the container witn the latest stable version of Grafana. Your container's ID will be returned

>*Note*: To stop the container use `docker container stop 123456789` where `123456789` is your container's ID. To resume it use `docker container start 123456789`

*Step 4. Logging in for the first time*  
Open your web-browser and go to http://localhost:3000/. You are expecting to see a login page. Type `admin` in both login and password fields. Click "login" and change your password

*Step 5. Adding data source*  
Click "Add data source" button and choose "TestData DB" on the bottom of the page. Then click "Save and test"  

*Step 6. Creating a test dashboard*  
- Click on the Grafana logo in the upper left corner to return to the home page.  
![](https://github.com/eltsovaad/GrafanaInstallation/blob/master/GrafanaLogo.JPG "grafana logo") 
- Click "New dashboard" button and "Add query" then. 
- In the "Query" field choose "TestData DB" instead of "default" and click button "Save dashboard" ![](https://github.com/eltsovaad/GrafanaInstallation/blob/master/saveDashboard2.JPG "grafana logo")  
  
You are awesome! Thank you for folowing this guide  
  
See also:  
https://docs.docker.com/engine/reference/commandline/pull/  
https://docs.docker.com/engine/reference/commandline/run/  
https://grafana.com/docs/grafana/latest/installation/docker/  
https://grafana.com/docs/grafana/latest/guides/getting_started/  
