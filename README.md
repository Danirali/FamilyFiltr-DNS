# FamilyFiltr-DNS
An open-source python based DNS server built to protect children.
<br>
### Our Aim
To help keep people safe online by creating a simple and easy to use UI to manage DNS ads and website blocking. We hope to keep this project open source :D
<br>
### Open Source
We try to keep all files in the python programming language to ensure that is accessable to all.

### Installation
Docker: [danirali2007/FamilyFiltr-DNS](https://hub.docker.com/r/danirali2007/familyfiltr-dns)

# Docker Variables Configuration
#### Volume Variables
To link the docker container storage volume to a local directory, this can be done via the docker GUI by setting the container path as `/app`.
#### Network Ports
The default ports for the container are:
<br>
<code>HTTP: 80
HTTPS: 443
DNS: 53
</code>

These can be altered via docker GUI or from cli with flag `-p {container}:{host}`.

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
    * main.py
    * ssl/
      * main.py
      * cert.crt
      * private.key
  * domains/
    * ads.txt
    * blocked_domains.txt
    * game-ads.txt

