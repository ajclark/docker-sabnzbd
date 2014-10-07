
# This is an opinionated SABnzbd Dockerfile. 

The idea behind my opinions is to bundle my specific SABnzbd.ini and autoProcessTV.cfg files as part of the docker image. This means it's somewhat useless to other people distributed as an image - but it's easier (for me) to bundle files vs play games with host mounted states and directories for configuration files.

# Instructions:

* Replace the empty `sabnzbd.ini` file with a working copy (yours)
* Replace or modify the `autoProcessTV.cfg` file to suit your needs - for sickbeard integration
* Build: `docker built -t .`
* Run: `docker run -d --name="sabnzbd_app" -p 8080:8080 -v /data:/mnt/media sabnzbd` NOTE: the /data mount depends somewhat on your sabnzbd.ini file. 
