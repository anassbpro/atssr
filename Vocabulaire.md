### Glossaire

**Modèle OSI - Open systeme Interconnexion** : un modèle en 7 couches qui explique comment les données voyagent d'un ordinateur à un autre. C'est comme une chaîne d'étapes où chaque couche a son rôle. Ca permet de faire un diagnostique.

- **Couche 1 – Physique** : la partie matérielle. Câbles RJ45, le Wi-Fi, les signaux électriques. C'est ici que les données deviennent des 0 et des 1.

- **Couche 2 – Liaison de données** : elle gère l'échange entre deux appareils voisins sur le même réseau grâce aux adresses MAC. Elle détecte aussi certaines erreurs.

- **Couche 3 – Réseau** : elle trouve le meilleur chemin pour envoyer les données grâce aux adresses IP. Le routeur travaille à ce niveau.

- **Couche 4 – Transport** : elle s'assure que les données arrivent bien et dans le bon ordre. On y trouve TCP (fiable) et UDP (rapide).

- **Couche 5 – Session** : elle ouvre, maintient et ferme la connexion entre deux appareils, un peu comme un appel qu'on démarre et qu'on raccroche.

- **Couche 6 – Présentation** : elle traduit les données dans un format compréhensible. Elle gère aussi le chiffrement et la compression.

- **Couche 7 – Application** : la couche la plus proche de l'utilisateur. C'est là que fonctionnent les protocoles comme HTTP, FTP ou DNS.

- **Encapsulation** : quand les données descendent les couches, chacune ajoute ses propres informations. Je le vois comme une lettre qu'on met dans plusieurs enveloppes.


**Modèle TCP/IP** : une version simplifiée du modèle OSI, en 4 couches. C'est celui qu'on utilise vraiment sur Internet.

- **Couche 1 – Accès réseau (ou Liaison)** : elle envoie physiquement les données sur le réseau local, par câble ou Wi-Fi. Pour moi, c'est les couches 1 et 2 de l'OSI réunies.

- **Couche 2 – Internet** : elle donne les adresses IP et fait passer les paquets d'un réseau à l'autre grâce aux routeurs. Elle correspond à la couche 3 de l'OSI.

- **Couche 3 – Transport** : elle s'occupe de livrer les données, soit de façon fiable avec TCP, soit rapidement avec UDP. Elle correspond à la couche 4 de l'OSI.

- **Couche 4 – Application** : elle regroupe les protocoles utilisés par les logiciels, comme HTTP, DNS ou SMTP. Je retiens qu'elle fusionne les couches 5, 6 et 7 de l'OSI.

**BIOS / UEFI**:

- **BIOS** : le tout premier programme qui se lance quand j'allume l'ordinateur. Il vérifie que le matériel fonctionne puis lance le système d'exploitation. C'est l'ancien système, assez limité.

- **UEFI** : le remplaçant moderne du BIOS. Il fait le même travail mais en mieux : démarrage plus rapide, interface plus pratique, prise en charge des gros disques et plus de sécurité.


**ISO / Image** : un fichier unique qui contient une copie complète d'un CD, d'un DVD ou d'un système d'exploitation. Pour moi, c'est une boîte qui contient tout ce qu'il faut pour installer Windows ou Linux.

**WDS** : un service de déploiement Windows Server qui permet d'installer Windows sur plusieurs ordinateurs en même temps, directement par le réseau, sans clé USB ni DVD.

**Déploiement** : le fait d'installer et de configurer un système ou un logiciel sur un ou plusieurs ordinateurs. Je le vois comme la mise en place d'un parc de machines prêtes à l'emploi.

**Bridged / NAT / Host-Only** : les trois modes réseau d'une machine virtuelle.
- **Bridged** : la VM est connectée directement au réseau, comme un vrai ordinateur, avec sa propre adresse IP.
- **NAT** : la VM passe par l'ordinateur hôte pour accéder à Internet, mais elle reste cachée du reste du réseau.
- **Host-Only** : la VM communique uniquement avec l'ordinateur hôte, sans accès à Internet.

**Octets / Bits** : le bit est la plus petite unité d'information en informatique, il vaut 0 ou 1. Un octet, c'est un groupe de 8 bits. Pour moi, le bit est une lettre et l'octet un petit mot.

**PXE** : une technologie qui permet à un ordinateur de démarrer directement par le réseau, sans disque dur ni clé USB. C'est souvent utilisé avec WDS pour installer Windows à distance.

**DHCP (Dynamic Host Configuration Protocol)** : un service qui donne automatiquement une adresse IP aux appareils qui se connectent au réseau. Pour moi, c'est comme un accueil qui attribue un numéro à chaque nouvel arrivant, sans avoir à tout configurer à la main.

**MBR / GPT** : deux façons d'organiser un disque dur pour savoir où se trouvent les partitions.
- **MBR (Master Boot Record)** : l'ancienne méthode, utilisée avec le BIOS. Elle est limitée à des disques de 2 To et à 4 partitions principales.
- **GPT (GUID Partition Table)** : la méthode moderne, utilisée avec l'UEFI. Elle gère des disques beaucoup plus gros et bien plus de partitions.

**Rufus / Ventoy** : deux logiciels qui permettent de créer une clé USB bootable pour installer un système d'exploitation.
- **Rufus** : il copie une seule image ISO sur la clé. Simple et rapide, mais il faut refaire la clé à chaque fois qu'on change d'ISO.
- **Ventoy** : on l'installe une fois sur la clé, puis il suffit d'y glisser plusieurs ISO. Au démarrage, je choisis celle que je veux lancer.

**Partition** : une division d'un disque dur en plusieurs parties indépendantes. 

**NTFS (New Technology File System)** : le système de fichiers utilisé par Windows. Il organise la façon dont les fichiers sont rangés sur une partition. 

**SHA-256 (Secure Hash Algorithm 256 bits)** : un calcul qui transforme un fichier en une suite unique de caractères, comme une empreinte digitale. Je m'en sers pour vérifier qu'une ISO téléchargée n'a pas été modifiée ou abîmée : si l'empreinte correspond à celle du site officiel, le fichier est bon. 

**VMware** : un logiciel qui permet de créer des machines virtuelles

**Windows Server** : la version de Windows faite pour les serveurs. Elle sert à gérer un réseau et ses services, comme le DHCP, WDS ou les comptes utilisateurs. C'est le Windows qui organise et contrôle les autres ordinateurs.

**Hyperviseur type 1 / type 2** : un hyperviseur est le logiciel qui fait tourner des machines virtuelles.
- **Type 1** : il s'installe directement sur le matériel, sans système d'exploitation en dessous. Plus performant, il est utilisé sur les serveurs (ex. : VMware ESXi, Hyper-V).

- **Type 2** : il s'installe comme un logiciel classique sur Windows ou Linux. Plus simple, je l'utilise pour tester sur mon PC (ex. : VMware Workstation, VirtualBox).

**DNS (Domain Name System)** : un service qui traduit un nom de domaine, comme google.fr, en adresse IP. Pour C'est l'annuaire d'Internet : je tape un nom, et il trouve le bon numéro pour que l'ordinateur sache où aller.

**Adresse IP / MAC** : deux adresses qui permettent d'identifier un appareil sur un réseau.
- **IP (Internet Protocol)** : l'adresse de l'appareil sur le réseau. Elle peut changer selon le réseau où je me connecte. C'est une identification d'un appareil sur le réseau.

- **MAC (Media Access Control)** : l'identifiant unique gravé dans la carte réseau. Elle ne change pas, comme un numéro de série.

**IEEE 802.3 / Ethernet II** : deux normes qui définissent comment les données sont envoyées sur un réseau filaire (Ethernet).
- **IEEE 802.3** : la norme officielle de l'Ethernet, créée par l'IEEE (Institute of Electrical and Electronics Engineers). Elle fixe les règles des câbles, des vitesses et du format des trames.

- **Ethernet II** : un format de trame plus ancien et plus simple. C'est celui qu'on retrouve le plus souvent aujourd'hui, notamment pour transporter des paquets IP.
