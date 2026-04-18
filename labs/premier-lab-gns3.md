---
layout: default
title: "Lab GNS3 - Réseau d'entreprise"
---

# 🧪 Lab GNS3 : Réseau d'entreprise avec VLAN, DHCP, NAT

## Objectif
Simuler une petite entreprise avec :
- 2 départements (Ventes, Tech)
- 1 routeur Cisco pour l’accès internet
- 1 switch VLAN
- Serveur DHCP

## Topologie
*(tu pourras ajouter une image plus tard : `![schéma](/images/lab-gns3.png)`)*

## Commandes essentielles
```cisco
enable
configure terminal
vlan 10
name Ventes
exit
vlan 20
name Tech
interface vlan 10
ip address 192.168.10.1 255.255.255.0
no shutdown
