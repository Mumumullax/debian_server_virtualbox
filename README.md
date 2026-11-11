# Projet personnel — Cybersécurité, Administration systèmes et réseaux

## Présentation

Dans le cadre de ma montée en compétences en administration systèmes et réseaux et en cybersécurité, j'ai entrepris un projet personnel pratique pendant les premières vacances de mon école.

Ce projet s'articule autour de deux axes :

- **Administration système :** installer, configurer et administrer un serveur Debian 13 dans un environnement virtualisé avec Oracle VirtualBox.
- **Cybersécurité :** découvrir les services réseau accessibles sur une machine volontairement vulnérable (Metasploitable 2), identifier les logiciels et leurs versions, puis analyser les risques de sécurité associés.

L'objectif est de développer mes compétences à travers des manipulations concrètes, des investigations techniques et la documentation de chaque étape.

## Environnement technique

- Système hôte : Ubuntu 26.04
- Virtualisation : Oracle VirtualBox
- Système invité : Debian GNU/Linux 13 (Trixie)
- Machine de laboratoire : Metasploitable 2
- Architecture : x86_64
- Service distant : OpenSSH
- Outil d'analyse réseau : Nmap
- Outil de développement et documentation : Visual Studio Code
- Gestion de versions : Git et GitHub
- Langages et technologies étudiés : Bash, Linux, Lua (lecture de scripts NSE)

## Travaux réalisés

### 1. Administration système — Debian 13

- Installation de Debian 13.
- Partitionnement du disque virtuel.
- Configuration du réseau et attribution d'une adresse IP.
- Installation et activation du service SSH.
- Configuration d'une redirection de port dans VirtualBox.
- Connexion distante au serveur depuis Ubuntu.
- Vérification de la connectivité réseau et de l'état des services.

### 2. Cybersécurité — Investigation Metasploitable 2

Mise en place d'un environnement de laboratoire isolé avec VirtualBox et une machine Metasploitable 2 volontairement vulnérable.

**Travaux effectués :**

- Configuration du réseau Host-only (`vboxnet0`).
- Vérification de la communication entre Ubuntu et Metasploitable 2.
- Découverte des ports ouverts avec Nmap.
- Identification des services et de leurs versions avec `nmap -sV`.
- Analyse initiale des services FTP, SSH, Telnet, SMTP, DNS, HTTP et RPCbind.
- Vérification de l'accès FTP anonyme avec un script NSE.
- Étude des risques associés aux services et aux versions détectées.
- Découverte des anciens services Unix `rexec`, `rlogin` et `rsh`.
- Consultation et analyse de scripts NSE écrits en Lua, notamment `rlogin-brute.nse` et `rexec-brute.nse`.
- Étude des catégories de scripts Nmap (`brute`, `intrusive`).

**Méthodologie :**

Les investigations sont réalisées progressivement, service par service, en distinguant les résultats réellement observés, les hypothèses de vulnérabilité et les risques potentiels.

Aucune exploitation ni tentative de brute force n'a été réalisée dans les séances documentées à ce stade.

## Objectifs pédagogiques

- Comprendre le fonctionnement d'un système Linux serveur.
- Maîtriser les commandes fondamentales d'administration.
- Comprendre les mécanismes de communication réseau.
- Mettre en place un accès distant sécurisé.
- Comprendre le fonctionnement des ports et des services réseau.
- Apprendre à utiliser Nmap et ses scripts NSE.
- Développer une méthodologie de reconnaissance et d'analyse de sécurité.
- Identifier les risques liés aux services et à leurs configurations.
- Lire et comprendre des scripts techniques en Lua.
- Documenter une investigation et conserver une trace des manipulations réalisées.

## Organisation du projet

```text
debian_server_virtualbox/
│
├── README.md
│
├── jdb_s1_metasploitable2
│
├── jdb_s2_metasploitable2
│
└── debian_server_virtualbox/
    └── Journaux et documentation du serveur Debian
```

## Documentation

Les différentes étapes du projet sont documentées dans des journaux de bord techniques.

Ces documents retracent les commandes utilisées, les résultats obtenus, les analyses réalisées et les points restant à approfondir.

## Gestion de versions

Le projet est versionné avec Git et hébergé sur GitHub.

Dépôt : https://github.com/Mumumullax/debian_server_virtualbox

## Statut du projet

Projet personnel en cours de réalisation depuis le 09/11/2026.

Les investigations sur Metasploitable 2 et les travaux d'administration Debian se poursuivent progressivement, avec une approche pratique et documentée.
