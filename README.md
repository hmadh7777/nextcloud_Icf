##Welkom bij het Nextcloud_Icf Project!


Dit GitHub-repository vormt de kern van het Mangum Ops-project voor Nextcloud-implementatie en -beveiliging. Hier vind je de geautomatiseerde tools om Nextcloud te implementeren, beveiligingsmaatregelen te configureren en een robuust Nextcloud-systeem te ontwikkelen. Volg onze gedetailleerde documentatie om stap voor stap door het proces te gaan.


Waarom Nextcloud?
Nextcloud is een krachtig en veelzijdig open-source platform. Het biedt een zelf-gehoste oplossing voor bestandsopslag, synchronisatie, samenwerking en meer. Als open-source platform is de broncode vrij beschikbaar voor aanpassingen en verbeteringen. Bovendien geeft het zelf hosten van Nextcloud gebruikers volledige controle en privacy over hun gegevens.


Beveiligingsmaatregelen en Hardening
Veiligheid staat voorop bij het implementeren van Nextcloud. We implementeren strenge beveiligingsmaatregelen, zoals firewallregels om onnodige toegang tot de server te blokkeren. We gebruiken LetsEncrypt om gratis SSL-certificaten te verkrijgen voor HTTPS-encryptie van Nextcloud-verkeer. Ook voeren we beveiligingshardening uit op zowel het besturingssysteemniveau als het applicatieniveau om kwetsbaarheden te verminderen.


Project Setup
Dit project automatiseert de installatie en configuratie van Nextcloud, Jitsi-server en Moodle op een Rocky Linux master en een Ubuntu client machine met behulp van Ansible.



#Vereisten
master machine
client machine
Ansible geïnstalleerd op de Rocky Linux machine
SSH-toegang tussen de Rocky Linux machine en de Ubuntu client machine
Installatie
Volg onze gedetailleerde stappen om Ansible te installeren op Rocky Linux en SSH-toegang te configureren tussen de master en de client machine.

Laten we samen werken aan een veilig en betrouwbaar Nextcloud-systeem!

# Project Setup

Dit project automatiseert de installatie en configuratie van Nextcloud, Jitsi-server, en Moodle op een Rocky Linux master en een Ubuntu client machine met behulp van Ansible.

## Vereisten

- **Rocky Linux 9** VM als master machine
- **Ubuntu** client machine
- **Ansible** geïnstalleerd op de Rocky Linux machine
- SSH-toegang tussen de Rocky Linux machine en de Ubuntu client machine

## Installatie

### Ansible Installeren op Rocky Linux

1. Update je pakketlijst en installeer de EPEL-release:

2. Installeer Ansible:

3. Controleer de Ansible-installatie:


### SSH Keypair Genereren en Configureren

1. Genereer een SSH keypair:


2. Kopieer de publieke sleutel naar de Rocky Linux VM en de Ubuntu clientmachine:
 

### Inventarisbestand Configureren

Maak een `hosts.ini` inventarisbestand aan:

















