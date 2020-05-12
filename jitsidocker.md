## 1. Clone jitsi docker
- Git clone https://github.com/jitsi/docker-jitsi-meet
## Quick start for windown
- Create a .env file by copying and adjusting env.example
    + cp env.example .env
- Set strong passwords in the security section options of .env file by running the following bash script
    + ./gen-passwords.sh
- Create required CONFIG directories
    mkdir jitsi-meet-cfg/{web/letsencrypt,transcripts,prosody/config,prosody/prosody-plugins-custom,jicofo,jvb,jigasi,jibri}
- Change setting in .env
    + Directory where all configuration will be stored
    + CONFIG=/.jitsi-meet-cfg
- Run docker-compose up -d
- Access the web UI at https://localhost:8443 (or a different port, in case you edited the compose file).