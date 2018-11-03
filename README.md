# Usage

1. Create a "content" subdirectory via `mkdir content`
2. `docker-compose up -d`

Wordpress will be available via http://localhost:8000.  The wp-content directory will
be mapped to the `content` directory.

# Windows Users

If you are using Docker for Windows (not Docker Toolbox), make sure you are using _Linux_ containers instead
of Windows containers. Set this by right-clicking on the Docker icon in the system tray.

If the `docker-compose up` command hangs while creating the wordpress container, you may need to mark the drive
as shareable. To do this, right-click on the Docker icon in the system tray, choose "Settings" and go to the 
"Shared Drives" tab.

You may also need to set the `COMPOSER_FORCE_WINDOWS_HOST` and `COMPOSE_CONVERT_WINDOWS_PATHS`
environment variables.

```
set COMPOSER_FORCE_WINDOWS_HOST=1
set COMPOSE_CONVERT_WINDOWS_PATHS=1
```
