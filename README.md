# 🏢 ProprioFinder - SaaS de Recherche de Propriétaires Immobiliers

SaaS complet pour retrouver les propriétaires immobiliers en France à partir de bases de données PostgreSQL, avec enrichissement de contacts et système de crédits.

## 🎯 Fonctionnalités

### Recherches
- ✅ **Recherche par adresse** - Trouve tous les propriétaires d'un bien
- ✅ **Recherche par propriétaire** - Trouve toutes les propriétés d'un propriétaire
- ✅ **Recherche par zone géographique** - Dessine une zone sur carte interactive (Leaflet)

### Système de Crédits
- ✅ Facturation au nombre de lignes (pas de requêtes)
- ✅ Workflow : Estimation → Validation → Exécution
- ✅ Débit de crédits après validation uniquement
- ✅ Intégration Stripe pour paiements

### Enrichissement de Données
- ✅ **Liens gratuits** vers Google Maps, Street View, Pappers, Cadastre, DVF, Géoportail
- ✅ **Enrichissement contacts** (PRO/ENTERPRISE) via Dropcontact : email, téléphone, LinkedIn
- ✅ Worker asynchrone avec BullMQ et Redis

### Multi-tenant
- ✅ Organisations avec plusieurs utilisateurs
- ✅ Rôles : Owner, Admin, Member
- ✅ Crédits partagés par organisation

### Exports
- ✅ Export CSV avec tous les liens d'enrichissement
- ✅ Téléchargement instantané des résultats

## 🛠️ Stack Technique

- **Framework** : Next.js 14 (App Router)
- **UI** : shadcn/ui + Tailwind CSS
- **Base de données** : PostgreSQL + Prisma ORM
- **Authentification** : NextAuth.js
- **Paiements** : Stripe
- **Enrichissement** : Dropcontact API
- **Cartes** : React Leaflet + Leaflet Draw
- **Queue** : BullMQ + Redis
- **Géospatial** : Turf.js

## 📦 Installation

Consultez [QUICKSTART.md](./QUICKSTART.md) pour un guide de démarrage rapide.

Consultez [DEPLOYMENT.md](./DEPLOYMENT.md) pour le déploiement en production.

## 📄 Licence

Ce projet est fourni tel quel, sans garantie.

---

**Développé avec Next.js, Prisma, Stripe, et Dropcontact** 🚀