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

<code>/app
  |_ main.py
  |_ options.txt
  |_ requirements.txt
  |_ run.sh
  |_ log.txt
  |_ blocked_pages/
        |_ blocked_{time}.txt
  |_ splashscreen/
        |_ main.py
        |_ ssl/
            |_ main.py
            |_ cert.crt
            |_ private.key
  |_ domains/
        |_ ads.txt
        |_ blocked_domains.txt
        |_ game-ads.txt
</code>
