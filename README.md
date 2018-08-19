# SurvUp
Quick start, stop, restart the Apache2, MySQL (MariaDB) and Webmin services or see service status.

SurvUp is a utility sript for easy activation/deactivation of web services installed locally within a GUI environment.

Use to improve system bootup times. Enable web services only when they are required.
Use to reduce system resource usage. Disable web services when not requred.
Use to quickly check status of the server services.

# Install
- Download SurvUp-Black.deb or SurvUp-White.deb. The only difference is the colour of the icons.
- Click the package to install the utility.
- Open your Task Launcher and browse to Utilities.
- Right-click the SurvUp icon (looks like a server) and pin it to the Task Manager.

After installation, if your server is installed on a local machine and is not needed from boot, you might optionally configure Apache2, MySQL and Webmin to not start at boot time.

# To Use
- Left-click the application icon to start/stop the Apache2, MySQL and Webmin services. Active services will stop, inactive services will start.
- Right-click the application icon to select a specific service action: start, stop, restart, status.

# Command Line Use
Run as `SurvUp` or as `SurvUp start|stop|restart|about`

- `SurvUp` will enable/disable the Apache2, MySQL and Webmin services.
- `SurvUp start` will start web services.
- `SurvUp stop` will stop web services.
- `SurvUp restart` will restart web services.
- `SurvUp reload` will reload web services. This is only available to command line SurvUp.
- `SurvUp status` will show the run status of the 3 web services.
- `SurvUp about` will show the SurvUp version number.

# Home Build
Rebuild the package with different icons or extra features. Edit the files in SurvUp-Black or SurvUp-White and build the installer with `dpkg-deb -b SurvUp-Black` or `dpkg-deb -b SurvUp-White`, respectively.

The debian SurvUp package template was created with the help of [softman package](https://github.com/VR51/softman) utility.

# Changelog
## 1.0.1
- Added status view option
- Added information output for actions
- Changed package folder name to denote icon colours
- Various minor changes.
