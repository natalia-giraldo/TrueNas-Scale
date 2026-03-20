# 🛡️ Projet TrueNAS SCALE : Infrastructure, Stockage RAID & Sécurisation

Titre : TrueNAS SCALE_Debian 
Auteur : Evan Bonnal, Natalia Giraldo
Formation : Bachelor IT en Cybersécurité
Durée : 1 semaine Établissement : La plateforme_

Ce dépôt documente la mise en place complète d'un environnement de stockage réseau (NAS) basé sur TrueNAS SCALE, incluant la configuration de volumes RAID sécurisés, l'exposition de services critiques (SSH, SFTP, HTTPS) et l'intégration de solutions de virtualisation et conteneurisation (Docker/Vaultwarden).

---

# 🏗️ Architecture du Projet

##1. Serveur TrueNAS SCALE
- Processeur : 2 cœurs
- RAM : 4 Go
- Stockage Système : 2 x 16 Go
- Stockage de Données : 5 disques de 2 To configurés en RAID 6 logiciel (ZFS RAID-Z2).

### Objectif : Tolérance de panne de 2 disques simultanés avec le pool nommé "Stockage".

## 2. Client d'Administration (Debian Desktop)

- Processeur : 2 cœurs | RAM : 2 Go | DD : 8 Go.

### Rôle : Station de contrôle pour les accès distants et tests de services.
---

# 🔒 Focus Cybersécurité
Ce projet met en avant plusieurs piliers de la sécurité informatique :

- Disponibilité : Redondance des données via RAID 6.
- Intégrité : Utilisation de ZFS pour prévenir la corruption silencieuse des données.
- Confidentialité : Chiffrement des transferts via SFTP/HTTPS et gestion des secrets avec Vaultwarden.
- Hardening : Changement des ports standards et désactivation des services inutiles.
---

## 🤝 Équipe

- [Evan Bonnal](https://github.com/EvanBonnal/)
- [Natalia Giraldo](https://github.com/natalia-giraldo/)
---

# 🎓 Contexte
Projet réalisé dans le cadre de la formation d'Administration Système / Cybersécurité à La Plateforme.
