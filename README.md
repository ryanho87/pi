# pi
Scripts to manage Home automation stuff running on my raspberry pi

### start-home ###
  If homeassistant is stopped while homebridge is running, homebridge will lose all devices being added by homeassistant.  This script will start the services in the correct order so that this does not happen.  In addition, this script will stop the services first if they are running.

### stop-home ###
  This script will stop both homebridge and homeassistant (in that order) so that homebridge will not lose homeassistant added devices.

### status-home ###
  This script will print the status of both homebridge and homeassistant to the console.  Status is determined from systemctl status.
