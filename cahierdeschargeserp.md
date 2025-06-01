# 📘 Cahier des Charges Détailé – Portail Pédagogique Interactif : Comprendre un ERP

## 1. 🎯 Objectif pédagogique

Ce projet a pour but de permettre aux étudiants de comprendre de manière interactive et visuelle :

* Ce qu’est un ERP (Enterprise Resource Planning)
* Les **20 principaux modules fonctionnels d’un ERP**
* Les **liens métiers** entre ces modules (ex: une vente génère une facture → une écriture comptable)
* Le **fonctionnement transversal** des processus métiers
* Les outils technologiques de base du développement web : **HTML, CSS, JS, Bootstrap**

Ce portail doit permettre à un étudiant :

* D'explorer chaque module
* De comprendre les **données entrantes / sortantes**
* De simuler un **workflow d’entreprise**
* D’avoir une **expérience utilisateur réaliste** (UX)

---

## 2. 🧑‍🎓 Public cible

| Public                           | Objectif pédagogique                                        |
| -------------------------------- | ----------------------------------------------------------- |
| Étudiants informatique           | Comprendre l’architecture fonctionnelle d’un ERP            |
| Étudiants gestion / comptabilité | Visualiser les flux de gestion et leur automatisation       |
| Étudiants logistique             | Comprendre l’impact des stocks, achats, ventes              |
| Étudiants RH                     | Voir le lien entre gestion du personnel, paie, comptabilité |
| Formateurs                       | Utiliser le portail comme support pédagogique interactif    |

---

## 3. 💡 Fonctionnalités détaillées

### F1. **Page d’accueil**

* Présentation du portail
* Définition d’un ERP
* Objectif de l’outil

### F2. **Tableau de bord des modules (Dashboard)**

* Vue cartes (grid Bootstrap)
* Chaque module → une carte cliquable
* Icône, titre, courte description

### F3. **Fiche explicative par module**

* Définition
* Objectifs
* Entrées / Sorties
* Lien avec autres modules
* Exemples d'utilisation
* ERP open-source qui le propose

### F4. **Simulations interactives**

* Exemple : un client crée une commande → une facture est générée → mise à jour du stock → écriture comptable
* Utilisation de JavaScript pour simuler un workflow simple (sans base de données)

### F5. **Cartes liées**

* Quand une carte est ouverte, montrer les autres cartes qui y sont liées (via des boutons ou surlignage)

### F6. **Recherche / filtre par fonctionnalité**

* Permet de filtrer les cartes selon un besoin (ex : finance, logistique, RH)

---

## 4. 🧩 Modules à intégrer (Top 20 + exemples open source)

| #  | Module               | Description                      | Exemples open source            |
| -- | -------------------- | -------------------------------- | ------------------------------- |
| 1  | CRM                  | Gestion relation client          | Odoo, ERPNext, Dolibarr, Axelor |
| 2  | Vente                | Devis, bons de commande          | Odoo, Tryton, ERP5              |
| 3  | Facturation          | Factures clients et fournisseurs | Dolibarr, Metasfresh            |
| 4  | Comptabilité         | Journaux, bilans, TVA            | Odoo, iDempiere                 |
| 5  | Achats               | Demande d’achat, fournisseur     | ERPNext, Dolibarr               |
| 6  | Stock                | Gestion des entrées/sorties      | Odoo, OpenBoxes                 |
| 7  | Supply Chain         | Livraison, transport             | ERPNext, Tryton                 |
| 8  | RH                   | Employés, contrats               | OrangeHRM, Odoo                 |
| 9  | Paie                 | Bulletin de salaire, charges     | Sentrifugo, Odoo                |
| 10 | Projets              | Suivi de tâches, planning        | ERPNext, Dolibarr               |
| 11 | BI / Reporting       | KPI, tableaux de bord            | Metabase, Superset              |
| 12 | Gestion documentaire | GED intégrée                     | Alfresco, Nextcloud             |
| 13 | E-commerce           | Intégration boutique             | Prestashop + Odoo               |
| 14 | SAV / Support        | Tickets clients                  | Zammad, GLPI                    |
| 15 | Budgets              | Prévisions, contrôle             | ERPNext, Axelor                 |
| 16 | Planning             | Gantt, disponibilités            | Dolibarr, ERPNext               |
| 17 | Workflow             | Processus automatisés            | Bonita BPM, ProcessMaker        |
| 18 | Utilisateurs & rôles | Sécurité des accès               | Keycloak (IAM), Odoo            |
| 19 | API / Connecteurs    | Echange avec d'autres systèmes   | WSO2, MuleSoft, Zapier          |
| 20 | Conformité           | RGPD, ISO 27001                  | Module annexe, mentions légales |

---

## 5. 🧱 Architecture technique

* **Frontend uniquement** (HTML, CSS, JS, Bootstrap)
* **Pas de base de données**
* **Fichier unique `index.html`** ou application mono-page (SPA)
* **Javascript natif** ou possibilité d’évoluer avec Vue/React en V2
* **Responsive design** (mobile/tablette/desktop)

---

## 6. 📂 Arborescence du projet

```
erp-dashboard/
├── index.html
├── css/
│   └── style.css
├── js/
│   └── main.js
├── img/
│   └── icons/
├── modules/
│   └── vente.html (et autres modules)
└── README.md
```

---

## 7. 🎓 Scénarios pédagogiques

1. **Cas 1 – Du CRM à la comptabilité**

   * Créer un client → saisir un devis → valider une commande → générer une facture → enregistrer dans les journaux

2. **Cas 2 – Gestion de stock et achat**

   * Rupture de stock → génération automatique d’un bon de commande fournisseur → réception → mise à jour stock

3. **Cas 3 – RH et paie**

   * Embauche d’un salarié → génération du contrat → traitement de la paie → impact en comptabilité

---

## 8. ✅ Critères de réussite (évaluation pédagogique)

| Critère                         | Pondération |
| ------------------------------- | ----------- |
| Respect du cahier des charges   | 20%         |
| Qualité du code (HTML/CSS/JS)   | 20%         |
| Pertinence pédagogique          | 20%         |
| Interactivité (JS, simulations) | 20%         |
| UX/UI & ergonomie (Bootstrap)   | 20%         |

---

## 9. 📌 Livrables

* Code source (fichiers HTML/CSS/JS)
* Documentation technique (README.md)
* Guide utilisateur (PDF ou page HTML)
* Présentation synthétique du portail

---

## 10. 🔄 Évolutivité

* V2 avec backend (Flask, Node.js)
* Utilisation de base de données
* Ajout de logs, journalisation, authentification
* Intégration avec ERP réel en open source (ex: Odoo)

---

Souhaitez-vous que je commence maintenant à générer **les 20 cartes de modules ERP avec interactivité pédagogique** selon ce cahier des charges ?
