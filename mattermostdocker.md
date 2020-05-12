## 1. Clone Mattermost docker
- git clone https://github.com/mattermost/mattermost-docker.git
- cd mattermost-docker/
- git checkout tags/5.19.0

## 2. Edit script and build files
 - docker-compose.yml docker-compose.yml
 - app/entrypoint.sh entrypoint_app.sh
 - web/entrypoint.sh entrypoint_web.sh
## 3. Start mattermost
 - docker-compose up -d
 - Start/Stop/Restart
    + docker-compose start
    + docker-compose stop
    + docker-compose restart 

