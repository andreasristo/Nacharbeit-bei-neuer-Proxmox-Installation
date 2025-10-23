# Nacharbeit-bei-neuer-Proxmox-Installation

Um die Meldung der Subscription zu deaktivieren, in der Shell des pve diesen Befehl ausführen:

bash -c "$(wget -qLO - https://github.com/community-scripts/ProxmoxVE/raw/main/misc/post-pve-install.sh)"

Source List aktualisieren

We recommend to configure this repository in /etc/apt/sources.list.
File /etc/apt/sources.list

deb http://ftp.debian.org/debian bookworm main contrib\
deb http://ftp.debian.org/debian bookworm-updates main contrib\
##Proxmox VE pve-no-subscription repository provided by proxmox.com,\
##NOT recommended for production use\
deb http://download.proxmox.com/debian/pve bookworm pve-no-subscription\
##security updates\
deb http://security.debian.org/debian-security bookworm-security main contrib\
