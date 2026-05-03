# Docker + WordPress
### Docker: https://www.docker.com/

<img src="https://i.ibb.co/d4vyrRm/docker-bg.png">

__Docker__ allows you to quickly build a set of containers and deploy __WordPress__ development. Then, just as quickly, transfer it all to any system. The "docker-compose" file is provided, which is a set of instructions for __Docker__ that will download and install all dependencies. You only need to install __Docker__ on your computer.

__command to start:__

```bash 
docker-compose up -d
```

**THIS IS A STARTER BOILERPLATE FOR LOCAL WORDPRESS DEPLOYMENT.**

It provides a pre-configured Docker environment for fast and reliable development, automating the setup of the web server, database, and management tools.

## Project Architecture

The environment consists of three main services:
- **WordPress**: The main web server with live file linking.
- **MySQL Database**: Persistent storage for all your content and settings.
- **PhpMyAdmin**: A web-based tool for easy database management (available on port 8008).

## Custom Features & Diagnostic Files

We have added specific files to improve the development experience:

1. **`uploads.ini`**: This file increases PHP limits (file uploads, memory, and execution time), which is essential for installing large WordPress themes and plugins.
2. **`info.php`**: A diagnostic tool that allows you to verify the server configuration and confirm that custom settings are applied.

> [!WARNING]
> **Security Note**: Always remove `info.php` before moving the project to a public or production server.
