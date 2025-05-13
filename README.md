# 📡 Projet d'Analyse Réseau avec Wireshark et Tshark

Ce projet explore les fondamentaux de l'analyse réseau à travers Wireshark et Tshark, en couvrant le modèle OSI, les protocoles clés, et l'automatisation des captures.

---

## 📚 Sommaire

### [Partie 1 : Initiation à Wireshark et Modèle OSI](#partie-1--initiation-à-wireshark-et-modèle-osi)
1. [Présentation de Wireshark](#présentation-de-wireshark)
2. [Concepts de base (Trame, Paquet, PCAP/PCAPNG)](#concepts-de-base)
3. [Pratique avec Wireshark (ARP/UDP/TCP, Désencapsulation OSI)](#pratique-avec-wireshark)
4. [Analyse des en-têtes (MAC/IP, Spécifications ARP/UDP/TCP)](#analyse-des-en-têtes)
5. [Mécanisme TCP (Three-Way Handshake)](#mécanisme-tcp)

### [Partie 2 : Capture Ciblée de Protocoles](#partie-2--capture-ciblée-de-protocoles)
1. [Lab réseau avec 2 VM](#lab-réseau)
2. [Analyse des protocoles (DHCP, DNS, FTP, HTTPS...)](#analyse-des-protocoles)
3. [Sauvegarde des paquets](#sauvegarde-des-paquets)

### [Partie 3 : Automatisation avec Tshark](#partie-3--automatisation-avec-tshark)
1. [Installation de Tshark](#installation-tshark)
2. [Commandes avancées](#commandes-tshark)
3. [Traitement des données](#traitement-des-données)

---

## 🛠️ Prérequis
- **Wireshark** : [Guide d'installation](https://www.wireshark.org/docs/wsug_html_chunked/ChapterBuildInstall.html)
- **Machine Linux** (ou VM)  
- **Accès root** (`sudo`)  

---

## Partie 1 : Initiation à Wireshark et Modèle OSI

### Présentation de Wireshark
Outil open-source d'analyse de paquets.  
📖 [Documentation officielle](https://www.wireshark.org/docs/)  

### Concepts de base
- **Trame** (L2) vs **Paquet** (L3)  
- **PCAP/PCAPNG** : Formats de capture.  
🔍 [Explications détaillées](#concepts-de-base)

### Pratique avec Wireshark
- Capture de :
  - **ARP** : `arp`  
  - **UDP** : `udp.port == 53` (DNS)  
  - **TCP** : `tcp.port == 80` (HTTP)  
🎥 [Tutoriel vidéo](#pratique-avec-wireshark)

### Analyse des en-têtes
| Champ          | Exemple (ARP)       |
|----------------|---------------------|
| MAC Source     | `00:1a:2b:3c:4d:5e` |
| IP Destination | `192.168.1.1`       |  
📊 [Exemples complets](#analyse-des-en-têtes)

### Mécanisme TCP
```mermaid
sequenceDiagram
    Client->>Serveur: SYN
    Serveur->>Client: SYN-ACK
    Client->>Serveur: ACK
