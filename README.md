# 🛠️ Projet : Gestion des demandes avec GLPI

## 🎯 Objectif

Reconstituer un serveur GLPI sous Debian, restaurer ses fonctionnalités de ticketing, et mettre en place un système d’inventaire automatique du parc via l’agent GLPI.

## 🔍 Contexte

Suite à une panne, toutes les demandes d'assistance ont été regroupées dans un système GLPI reconstruit sur Debian. Ce projet s'inscrit dans une logique de gestion d'incidents et de support utilisateur au sein d'une DSI.

Deux objectifs principaux :
- Restaurer un serveur GLPI fonctionnel et sécurisé
- Automatiser l’inventaire du parc informatique via GLPI Agent

## 🧠 Compétences mobilisées

- Administration Linux (Debian)
- Déploiement d'un serveur GLPI
- Installation et configuration de l'agent GLPI 1.7
- Gestion des incidents en N1/N2
- Rédaction d’un logigramme de traitement des tickets
- Restauration d'une base de données `.sql` dans MariaDB

## 🧩 Architecture mise en place

- GLPI installé sur Debian 12
- Base de données restaurée à partir du fichier `Vouette_Christophe_1_export_042024.sql`
- Agent GLPI installé sur un poste Windows 10 (VM VirtualBox)
- Communication avec le serveur via le plugin GLPI Inventory (port 6354)

## 🖼️ Captures & documents

- 🔗 [Présentation Agent GLPI (PDF)](./Vouette_Christophe_3agent_glpi_042024.pdf)
- 🔗 [Logigramme de traitement des tickets (PDF)](./Vouette_Christophe_4_logigramme_042024.pdf)
- 💾 [Base de données exportée (SQL)](./Vouette_Christophe_1_export_042024.sql)

## ⚙️ Exemple de configuration

**Adresse GLPI utilisée par l'agent** :  
`http://192.168.68.54/glpi`

**Port utilisé pour le plugin Inventory** :  
`6354`

## ✅ Résultats obtenus

- Refonte complète du serveur GLPI sur Debian 12
- Réception automatique des données du poste utilisateur sous Windows 10 grâce à GLPI Agent
- Suivi des tickets possible en N1 et N2 avec logigramme de validation

## 📚 Technologies utilisées

- Debian 12
- GLPI 10.x
- GLPI Agent 1.7
- MariaDB
- VirtualBox

## 📁 Arborescence du dossier

