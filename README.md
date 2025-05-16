# 📡 WireShark v2 – Analyse réseau & Automatisation

Ce dépôt contient un cours complet sur l'analyse réseau avec **Wireshark** et **TShark**, depuis les bases jusqu’à l’automatisation de la capture et du traitement des paquets réseau.

---

## 🗂️ Sommaire

### Partie 0 : Introduction

1. [Présentation de Wireshark](#1-présentation-de-wireshark)  
2. [Concepts de base (Trame, Paquet, Fichier de capture)](#2-concepts-de-base-trame-paquet-fichier-de-capture)  

### Partie 1 : Initiation à Wireshark et Modèle OSI sur L'Alcazar

1. [Pratique avec Wireshark (ARP, UDP, TCP)](#1-pratique-avec-wireshark-arp-udp-tcp)  
2. [Analyse des en-têtes (MAC/IP, ARP, UDP, TCP)](#2-analyse-des-en-têtes-macip-arp-udp-tcp)  
3. [Connexion TCP (Diagramme des étapes)](#3-connexion-tcp-diagramme-des-étapes)

### Partie 2 : Capture Ciblée de Protocoles
1. [Lab Réseau avec 2 VM (NAT)](#1-lab-réseau-avec-2-vm-nat)  
2. [Capture et analyse des protocoles](#2-capture-et-analyse-des-protocoles)  
3. [Sauvegarde des paquets pertinents](#3-sauvegarde-des-paquets-pertinents)

### Partie 3 : Automatisation avec TShark
1. [Installation et prise en main](#1-installation-et-prise-en-main)  
2. [Commandes de capture avancées](#2-commandes-de-capture-avancées)  
3. [Redirection et traitement des données](#3-redirection-et-traitement-des-données)

---

## Partie 0 : Introduction

### 1. Présentation de Wireshark
Introduction à l'outil Wireshark, son interface graphique, et ses fonctionnalités principales.

### 2. Concepts de base (Trame, Paquet, Fichier de capture)
Explication des notions fondamentales du réseau : trames, paquets, segments et fichiers `.pcap`.


## Partie 1 : Initiation à Wireshark et Modèle OSI

### 1. Pratique avec Wireshark (ARP, UDP, TCP)
Captures en temps réel de protocoles réseau comme ARP, UDP et TCP. Visualisation du trafic dans Wireshark.

### 2. Analyse des en-têtes (MAC/IP, ARP, UDP, TCP)
Décomposition des paquets pour examiner les en-têtes des couches 2 à 4 (adresse MAC, IP, ports, etc.).

### 3. Connexion TCP (Diagramme des étapes)
Étude du **handshake TCP** (SYN, SYN-ACK, ACK) à l’aide d’un diagramme de séquence et d’une capture réseau.

---

## Partie 2 : Capture Ciblée de Protocoles

### 1. Lab Réseau avec 2 VM (NAT)
Mise en place d’un environnement de test avec deux machines virtuelles en NAT (client/serveur).

### 2. Capture et analyse des protocoles
Observation et analyse du comportement des protocoles :
- **DHCP** (attribution d’adresse IP)
- **DNS** / **mDNS**
- **FTP** (fichiers)
- **SMB** (partage Windows)
- **HTTPS / TLS v1.2** (chiffrement)

### 3. Sauvegarde des paquets pertinents
Exportation des paquets capturés au format `.pcap` pour documentation ou analyse ultérieure.

---

## Partie 3 : Automatisation avec TShark

### 1. Installation et prise en main
Installation de TShark, version en ligne de commande de Wireshark, sur Linux ou Windows.

### 2. Commandes de capture avancées
Utilisation de filtres BPF, sélection d’interface, capture conditionnelle, durée ou taille.

### 3. Redirection et traitement des données
Redirection de la sortie (`JSON`, `text`, etc.) vers des fichiers ou des scripts pour exploitation automatisée.

---

## 🔗 Liens utiles

- 🌐 [Wireshark – Site officiel](https://www.wireshark.org/)  
- 📄 [TShark – Documentation](https://www.wireshark.org/docs/man-pages/tshark.html)  
- 📘 [Modèle OSI – Wikipedia](https://fr.wikipedia.org/wiki/Mod%C3%A8le_OSI)  
- 🧪 [Filtres d'affichage Wireshark](https://wiki.wireshark.org/DisplayFilters)

---



