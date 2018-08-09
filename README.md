# Docker Wordpress Development
This project allows a developer to set up a quick wordpress development environment using docker containers.

# Features
- Sets up database
- Download and installs wordpress
- Configures environment
- Creates the following volumes for development
    - ./wp-content/themes/my-theme:/var/www/html/wp-content/themes/my-theme # mapping our custom theme to the container
    - ./wp-content/plugins:/var/www/html/wp-content/plugins # map our plugins to the container
    - ./wp-content/uploads:/var/www/html/wp-content/uploads # map our uploads to the container

# Requirements
You need to have **docker** installed on your machine.

# Steps
- **Install docker**
- Open your **terminal** and run the following: *docker-compose up -d*
- navigate to localhost:8000 or whatever port number you changed ports to within your docker-compose file.

#Exporting Data
You can export data by running the *export.sh* script in your terminal.
Use **sh export.sh** if you are on a mac. Note: this can only be done after docker-compose has set up your environment and created the correct folders.