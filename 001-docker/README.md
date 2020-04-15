# 001 - Docker

Materijali za video: https://youtu.be/kl3i-C3HYSE

### Docker instalacija

#### MacOs i Windows
- https://docs.docker.com/get-docker/

#### Linux (Debian - Mint, Ubuntu..)
- sudo apt-get install apt-transport-https ca-certificates curl gnupg-agent software-properties-common
- curl -fsSL https://download.docker.com/linux/ubuntu/gpg | sudo apt-key add -
- sudo add-apt-repository "deb https://download.docker.com/linux/ubuntu disco stable"
- sudo apt-get update
- sudo apt-get install docker-ce
- sudo usermod -aG docker `` `whoami` ``
- sudo curl -L https://github.com/docker/compose/releases/download/1.25.0/docker-compose-`` `uname -s` ``-`` `uname -m` `` -o /usr/local/bin/docker-compose
- sudo chmod +x /usr/local/bin/docker-compose


#### Linux (ArchLinux i distribucije - Manjaro..)
- sudo pacman -Sy docker docker-compose && sudo usermod -aG docker `` `whoami` ``


Nakon instalacija napravite restart računala.

### Info
- Ukoliko imate problema s apache file permission (izbacuje vam access deny kada otvorite web host) promjenite www direktorij u src direktorij i promjenite unutar volumena putanju ili ako koristite linux - promjenite ovlasti nad folderom `sudo chown -x [naziv vašeg username-a] www` unutar direktorija gdje vam se nalazi folder. ( - Primjer 3)