# FamilyFiltr-DNS
An open-source python based DNS server built to protect children.
<br>
### Our Aim
To help keep people safe online by creating a simple and easy to use UI to manage DNS ads and website blocking. We hope to keep this project open source :D
<br>
### Open Source
We try to keep all files in the python programming language to ensure that is accessable to all.

# Installation
- Docker: [danirali2007/FamilyFiltr-DNS](https://hub.docker.com/r/danirali2007/familyfiltr-dns)

  #### Once docker container is running: navigate to https://localhost:443/status to check for the status of the web server.

  On healthy start: <code>{"status":"healthy"}</code>

### Docker Variables Configuration
#### Volume Variables
To link the docker container storage volume to a local directory, this can be done via the docker GUI by setting the container path as `/app`.
#### Network Ports
The default ports for the container are:
<br>
<code>HTTPS: 443
DNS: 53
</code>

* NOTE: Port 8000 is a failover port for flask web server.

These can be altered via docker GUI or from cli with flag `-p {container}:{host}`.

# Add Addition Domains
Each domain type:

* Ads
* Game Ads
* Blocked Domains
* Social Media Domains

To modify which domains are blocked, append `options.txt` with one of the following domain types:

* ADS
* GAME_ADS
* BLOCKED_DOMAINS
* SOCIAL_MEDIA

<br>

# File Structure

/app
  * main.py
  * options.txt
  * requirements.txt
  * run.sh
  * log.txt
  * blocked_pages/
    * blocked_{time}.txt
  * splashscreen/
    * web.py
    * ssl/
      * gen.py
      * cert.crt
      * private.key
  * domains/
    * ads.txt
    * blocked_domains.txt
    * game-ads.txt
    * social_media_domains.txt

