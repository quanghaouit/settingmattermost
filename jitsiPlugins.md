## setting mattermost plugins
- In file config.json. Find `PluginSettings` and enable `EnableUploads = TRUE`. This option allow upload file plugin in server as format file `tar.gz`.
- We also need to create folder `client/plugins` in folder `cmd/mastermost` for store plugins file.
- Restart server.

## jitsiPlugin
- git clone `https://github.com/seansackowitz/mattermost-plugin-jitsi.git`
- Forllow instruction for build plugin include server and webapp. Then build as `tar.gz` file.
- Or you can download release file as `https://github.com/seansackowitz/mattermost-plugin-jitsi/releases`
- Access to mattermost server as admin. Open system-console `http://localhost:9005/admin_console/reporting/system_analytics`
- Open `Plugin managerment` and upload jitsi plugins
- Setting Jitsi server URL. You can set up your jitsi server or can use `https://meet.jit.si/`
- Back to chat app and you will see appear `camara icon` for start jitsi meating.