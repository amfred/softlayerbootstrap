softlayerbootstrap
==================
Authors: Ann Marie Fred, Esther Burwell, James Markham at IBM

Bootstrap scripts for SoftLayer: automatically install popular open source packages on SoftLayer bare metal servers or virtual machines (compute instances).  Put these bootstrap scripts somewhere where you can reference them using HTTP or HTTPS.  Then, enter the URL into the provision script URL field when creating a new server (virtual or bare metal) or re-imaging a server. SoftLayer will download but not execute HTTP URLs, and will download and execute HTTPS URLs.

See the LICENSE file for licensing details.  These scripts are provided strictly AS-IS and unsupported.  Use at your own risk.  If you would like to help improve a script, you can use the usual Github methods, or contact me on Twitter @DukeAMO.

+ https://gist.github.com/amfred/527ad1f36254a5aa7d93 testDropbox.sh 

  Dropbox is one way to get HTTPS URLs.  This is from my ChefConf 2014 demo.  It just writes a file and installs Chef.  Note: I do not consider Dropbox a secure repository.  DO NOT EVER put your passwords or other sensitive information into scripts that are saved in Dropbox.  Use a real, secure, HTTPS server for those bootstrap scripts.

+ https://gist.github.com/amfred/cdf321ff883acbc3897a bootstrapEurekaChefSoftLayer.sh 

  Bootstrap a Eureka server, SoftLayer style.  This is also an example of Chef Solo setup and editing Chef config files.  See https://github.com/EmergingTechnologyInstitute/SoftLayer-NetflixOSS/wiki/Micro-service-location-services-documentation for more details on the SoftLayer Eureka setup.

+ https://gist.github.com/amfred/2573ecabcb7c868b120a bootstrapDevstackUbuntuBaremetal.sh

  Install Devstack on a SoftLayer Ubuntu bare metal server.

+ https://gist.github.com/amfred/349f01c588836c17a0d3 bootstrapTomcatChefSoftLayer.sh

  Install Tomcat on a SoftLayer Ubuntu CCI, using Chef Solo.  This is also an example of Chef Solo setup and editing Chef config files.
  
+ https://gist.github.com/amfred/ecde9c0985e09a7d3821 bootstrapDisk2AndHostname.sh

  Add a secondary disk to a SoftLayer CentOS or RHEL compute instance, and format the hostname so it's easier to look up the hostname and FQDN.  Special thanks to http://firelitdesign.blogspot.com/2011/11/partition-and-mount-drive-on-centos.html for the paritioning tips.
