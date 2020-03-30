# How to install Grafana from its latest Docker Image

*Step 1. Installing Docker:*
Using [Docker Hub Get Started Guide](https://docs.docker.com/get-started/) install and run Docker for your operation system

*Note:* If you are on a Linux system, you might need to add `sudo` before the commands below

*Step 2. Downloading Grafana Docker Image:*
With `docker pull grafana/grafana:latest` download the latest version of Grafana docker image. 

*Step 3. Running container:*
Use `docker run -d -p 3000:3000 grafana/grafana` to run the container witn the latest stable version of Grafana. Command will return your container's ID

*Note:* To stop the container use `docker container stop 123456789` where `123456789` is your container's ID. To resume it use `docker container start 123456789`

*Step 4. Logging in for the first time*
Open your web-browser and go to http://localhost:3000/. You are expecting to see a login page. Type `admin` in both login and password fields. Click "login" and change your password
