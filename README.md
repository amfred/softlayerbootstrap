softlayerbootstrap
==================

Bootstrap scripts for SoftLayer: automatically install popular open source packages on Softlayer bare metal servers or virtual machines.  Put these bootstrap scripts somewhere where you can reference them using HTTP or HTTPS.  Then, enter the URL into the provision script URL field when creating a new server (virtual or bare metal) or re-imaging a server. SoftLayer will download but not execute HTTP URLs, and will download and execute HTTPS URLs.

See the LICENSE file for licensing details.  These scripts are provided strictly AS-IS and unsupported.  Use at your own risk.  If you would like to help improve a script, you can use the usual Github methods, or contact me on Twitter @DukeAMO.

https://gist.github.com/amfred/527ad1f36254a5aa7d93 testDropbox.sh 
Dropbox is one way to get HTTPS URLs.  ChefConf demo.

https://gist.github.com/amfred/cdf321ff883acbc3897a bootstrapEurekaChefSoftLayer.sh 
Bootstrap a Eureka server, SoftLayer style.  This is also an example of Chef Solo setup and editing Chef config files.  See https://github.com/EmergingTechnologyInstitute/SoftLayer-NetflixOSS/wiki/Micro-service-location-services-documentation for more details on the SoftLayer Eureka setup.
