## Run mattermost-server
- git clone `https://github.com/mattermost/mattermost-server.git`
- Follow instruction in README.md
- If make not work or have trouble with docker build. 
    + Download mysqlserver with version require in mattermost docker-compose
    setting with environment:
      MYSQL_ROOT_HOST: "%"
      MYSQL_ROOT_PASSWORD: mostest
      MYSQL_PASSWORD: mostest
      MYSQL_USER: mmuser
      MYSQL_DATABASE: mattermost_test
    + cd to folder `cmd` and run `go run main.go`

## Run mattermost-webapp
- git clone `https://github.com/mattermost/mattermost-webapp.git`
- npm install && npm run dev-server

==> DONE

