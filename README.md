
#  SABnzbd Dockerfile

### This project has moved to https://github.com/ajclark/usenet

# Instructions

* Build: `docker build -t sabnzbd .`
* Run: `run -d --name=sabnzbd_app --restart=always -v /data/warehouse/sabnzbd:/data -v /mnt/media:/mnt/media -p 8080:8080 sabnzbd`
