# Service EmulatorJS
- Image: lscr.io/linuxserver/emulatorjs:latest
- Container Name: emulatorjs
- Restart Policy: unless-stopped

# Usage
To start the EmulatorJS container, use the following command:
```
docker-compose up -d
```
*_This command will start the EmulatorJS service in detached mode._*

# Access
After starting the container, you can access the EmulatorJS web interface
- by navigating to `http://<your-server-ip>:3000` in your web browser to access game administration
- by navigating to `http://<your-server-ip>:80` in your web browser to access game play

# Notes
- Ensure the specified directories for volumes exist on your host machine.
- Adjust the PUID and PGID environment variables to match your system's user and group IDs.
- The :ro at the end of each volume path ensures the directories are mounted as read-only.

# Useful external links
- https://belginux.com/installer-emulatorjs-avec-docker/