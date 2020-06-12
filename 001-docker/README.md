# 001 - Docker

Materijali za video: https://youtu.be/kl3i-C3HYSE

### Docker instalacija

#### MacOs i Windows
- https://docs.docker.com/get-docker/

#### Linux (Debian - Mint, Ubuntu..)
- Upute na linku: [Ovdje](./docker-debian-setup.txt)

#### Linux (ArchLinux i distribucije - Manjaro..)
- sudo pacman -Sy docker docker-compose && sudo usermod -aG docker `` `whoami` ``

Nakon instalacija napravite restart računala.

### Info
- Ukoliko imate problema s apache file permission (izbacuje vam access deny kada otvorite web host) promjenite www direktorij u src direktorij i promjenite unutar volumena putanju ili ako koristite linux - promjenite ovlasti nad folderom `sudo chown -x [naziv vašeg username-a] www` unutar direktorija gdje vam se nalazi folder. ( - Primjer 3)
