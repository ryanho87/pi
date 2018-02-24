# pi
Scripts to manage Home automation stuff running on my raspberry pi

### start-home ###
  If homeassistant is stopped while homebridge is running, homebridge will lose all devices being added by homeassistant.  This script will start the services in the correct order so that this does not happen.  In addition, this script will stop the services first if they are running.

### stop-home ###
  This script will stop both homebridge and homeassistant (in that order) so that homebridge will not lose homeassistant added devices.

### status-home ###
  This script will print the status of both homebridge and homeassistant to the console.  Status is determined from systemctl status.

### Upgrade ###
  Instructions for how to upgrade versions.  This script is currently non-functional, but lists out the commands to peform the upgrade
  
 ### Notes ###
home-assistant@homeassistant.service and homebridge.service located at /etc/systemd/system control the automatic startup of services.  A dependency has been created for homebridge.service which causes it to start after home-assistant@homeassistant.service
