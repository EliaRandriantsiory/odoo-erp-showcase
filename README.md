# Odoo ERP — Personnalisation métier et infrastructure

> Adapter Odoo 18 Community aux processus d'une entreprise et organiser son exploitation avec Docker et PostgreSQL.

**Domaines :** ERP · Développement Python · Processus métier · Infrastructure Linux

## Le besoin

Une entreprise a besoin de relier ses opérations commerciales, sa facturation et ses documents métier dans un même outil. L'enjeu est d'adapter un ERP existant à ses règles de fonctionnement tout en conservant la cohérence des données et des droits d'accès.

Ce projet associe des extensions Odoo et une infrastructure conteneurisée. La présentation porte sur les capacités du projet ; elle ne constitue pas une démonstration publique de l'environnement client.

## Périmètre de réalisation

- Personnalisation d'Odoo 18 Community avec des modules métier.
- Adaptation des écrans, des champs produits et des documents.
- Gestion des restrictions d'accès et des menus selon les responsabilités.
- Organisation du déploiement, des sauvegardes, de la restauration et des mises à jour.

## Fonctionnalités représentatives

| Domaine | Fonctionnalités |
|---|---|
| Gestion commerciale | Adaptation du parcours devis, facturation et livraison |
| Produits | Champs complémentaires et spécifications produits |
| Documents | Personnalisation des rapports et documents commerciaux |
| Finance | Exports financiers et adaptations des traitements métier |
| Accès | Restrictions de menus et droits selon les profils |
| Exploitation | Scripts de sauvegarde, restauration et mise à jour |

Les extensions spécifiques complètent les fonctions natives d'Odoo et les modules communautaires intégrés. Cette distinction permet de valoriser le travail d'adaptation sans attribuer au projet le développement du socle ERP.

## Architecture

| Couche | Technologie et responsabilité |
|---|---|
| Application | Odoo 18 Community et extensions Python |
| Données | PostgreSQL 16 |
| Exécution | Docker et Docker Compose |
| Accès web | Nginx, reverse proxy HTTPS |
| Persistance | Volumes pour les données et les pièces jointes |
| Maintenance | Scripts d'exploitation et documentation |

La séparation entre application, base de données et reverse proxy permet de gérer chaque service distinctement. La persistance des pièces jointes complète celle de la base de données.

## Points d'ingénierie

- **Étendre l'existant :** privilégier les mécanismes de modules Odoo pour adapter les comportements.
- **Respecter les responsabilités :** traduire les profils métier en règles d'accès.
- **Préserver les données :** traiter la base et les fichiers associés dans les opérations de maintenance.
- **Documenter l'exploitation :** expliciter les étapes de restauration et de mise à jour.

## Ce que ce projet démontre

La capacité à relier un besoin opérationnel à une solution ERP, puis à prendre en charge son environnement technique : développement Python, intégration de modules, PostgreSQL, conteneurisation et administration Linux.

L'apport fonctionnel est une gestion centralisée adaptée aux usages de l'entreprise. Aucun gain chiffré ni niveau de disponibilité n'est revendiqué dans cette présentation.

## À propos

Projet présenté par [Elia Randriantsiory](https://github.com/EliaRandriantsiory).

Ce dépôt est une **présentation de portfolio**. Il ne contient pas le code source de l'application, ni de données métier, de configuration de production ou d'identifiants. Les technologies tierces restent la propriété de leurs auteurs respectifs.

### Autres réalisations

- [Odoo ERP — Personnalisation métier](https://github.com/EliaRandriantsiory/odoo-erp-showcase)
- [RNT Server Manager — Administration Linux](https://github.com/EliaRandriantsiory/rnt-server-manager-showcase)
- [Fanavotana — Plateforme communautaire](https://github.com/EliaRandriantsiory/fanavotana-showcase)
