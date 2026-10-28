# Lab BSGRAPH Studio — Infrastructure d'une agence de 5 salariés

Projet personnel de montée en compétences en **administration systèmes et réseaux**, préparé dans le cadre de ma reconversion vers le titre **Administrateur d'Infrastructures Sécurisées** (RNCP niveau 6).

Je construis de A à Z l'infrastructure d'une agence fictive, **BSGRAPH Studio** : réseau, annuaire, partage de fichiers, serveur web, supervision et sécurité. Chaque étape est documentée avec ses configurations, ses tests et **les problèmes rencontrés avec leur résolution**.

## Environnement

- Hôte : MacBook M2 (ARM64), 8 Go de RAM
- Virtualisation : VirtualBox
- Contrainte : architecture ARM, donc pas de pfSense ni de Windows Server x86 → solutions Linux équivalentes

## Avancement

| Étape | Contenu | Outils | Statut |
|---|---|---|---|
| 1 | Serveur Linux de base | Ubuntu | ✅ |
| 2 | [Routeur, NAT, DHCP, DNS](etape-02-routeur/) | Ubuntu Server, nftables, dnsmasq, Netplan | ✅ |
| 3 | [Annuaire du domaine `bsgraph.local`](etape-03-annuaire-samba-ad/) | Samba AD, Kerberos, DNS | ✅ |
| 4 | Poste client joint au domaine | Windows 11 ARM | ⏳ |
| 5 | Serveur de fichiers, droits par service | Samba | ⏳ |
| 6 | Serveur web + administration SSH | Nginx, OpenSSH | ⏳ |
| 7 | Supervision | Uptime Kuma | ⏳ |
| 8 | Sécurité : sauvegardes, durcissement, audit | Kali Linux | ⏳ |

## Auteur

**Stanley Bellerose** — [Portfolio](https://stanleybellerose.github.io/Portfolio/)
