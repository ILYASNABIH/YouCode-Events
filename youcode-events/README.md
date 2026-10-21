# YouCode Events 📅

> Plateforme web centralisée, responsive et accessible dédiée à l'annonce et à l'inscription aux événements, ateliers, conférences et hackathons de YouCode.

## 📝 À propos du projet

**YouCode Events** réunit tous les événements organisés sur les différents campus YouCode au même endroit. Le site permet aux apprenants et aux visiteurs de consulter l'agenda complet, de découvrir les intervenants et partenaires, et de s'inscrire facilement aux activités.

Projet réalisé en équipe dans le cadre du cursus **YouCode**, du **12 au 16 octobre 2026**.

## 👥 Équipe et répartition des rôles

| Membre | Rôle | Pages & Responsabilités |
| ----- | ----- | ----- |
| **Ilyas Nabih** | Git Master & Developer | Page Accueil (co-réalisée), Page Intervenants, Page Inscription, Workflow Git Flow |
| **Anas Ameziane** | Lead UI/UX & Developer | Page Accueil (co-réalisée), Page Événements, Page Événement Detail, Design System Figma |

## 🛠️ Technologies utilisées

* **Design & Prototypage :** Figma (Design System, composants, prototypes)
* **Structure & Sémantique :** HTML5 (balisage sémantique, normes WAI-ARIA)
* **Stylisation & Layout :** CSS3 (variables CSS, Flexbox, CSS Grid)
* **Fonts & Icons :** Google Fonts, Font Awesome / Lucide Icons
* **Versionning & Collaboration :** Git, GitHub, Git Flow
* **Gestion de Projet :** GitHub Projects / Jira (Tableau Kanban)

## 📁 Structure du projet

```
youcode-events/
├── index.html                # Page d'accueil
├── evenements.html           # Liste des événements
├── evenement-detail.html     # Page de détail d'un événement
├── intervenants.html         # Page intervenants & partenaires
├── inscription.html          # Formulaire d'inscription
├── css/
│   ├── style.css             # Styles généraux, variables & composants
│   └── responsive.css        # Adaptation responsive (Media Queries)
├── assets/
│   ├── images/               # Images et photos des intervenants
│   └── icons/                # Icônes SVG / graphiques
└── README.md                 # Documentation du projet
```

## ⚙️ Workflow Git & Collaboration

Afin d'assurer une collaboration fluide et un suivi rigoureux des évolutions de code, l'équipe a suivi la méthodologie **Git Flow** :

### 1. Structure des branches
* `main` : Branche de production (stable et protégée).
* `develop` : Branche principale d'intégration (protégée).
* `feature/<numero-issue>-<sujet>` : Branches individuelles par fonctionnalité (ex: `feature/12-page-accueil`).

### 2. Format des Commits
Les commits respectent la convention standard :
* `feat:` Ajout d'une nouvelle fonctionnalité
* `fix:` Correction d'un bug
* `style:` Modifications visuelles ou CSS sans impact logique
* `docs:` Mise à jour de la documentation ou du README

### 3. Règles des Pull Requests (PR)
* Interdiction de push direct sur `main` et `develop`.
* Chaque PR doit être liée à son issue GitHub (`Closes #12`).
* Relecture obligatoire par au moins un coéquipier pour approbation.
* Interdiction d'auto-fusionner sa propre PR.
* Résolution des conflits sur la branche `feature/*` après mise à jour depuis `develop`.

## 📐 Points de rupture & Choix Responsive

La maquette a été conçue selon une approche **Desktop-First**, avec une intégration pensée pour s'adapter progressivement aux écrans plus petits :
* **Desktop (`> 1024px`) :** Disposition multi-colonnes complète, grilles larges pour les événements et les cartes intervenants.
* **Tablette (`768px - 1024px`) :** Recomposition des cartes en 2 colonnes, ajustement des espacements et de la taille des typographies.
* **Mobile (`< 768px`) :** Layout à colonne unique, adaptation de la navigation (menu mobile) et optimisation de la lisibilité des formulaires.

## ♿ Accessibilité (A11y)

* **Sémantique :** Utilisation stricte des balises `<header>`, `<nav>`, `<main>`, `<section>`, `<article>`, `<footer>`.
* **Titres :** Hiérarchie `<h1>` à `<h3>` cohérente sur l'ensemble des pages.
* **Images :** Attribut `alt` descriptif présent sur toutes les images informatives.
* **Formulaires :** Association explicite des `<label>` avec leurs `<input>`, types adaptés (`email`, `tel`) et validation HTML5 native.
* **Navigation :** Focus visible conservé sur tous les éléments interactifs et navigation clavier fonctionnelle.

## 🔗 Liens utiles

* 🎨 **Maquette Figma :** [Consulter la maquette Figma](https://www.figma.com/design/NBGqZKzgJ8gCszCVPDFC39/YouCode-Events-%E2%80%94-Maquette--Brief-2-?node-id=5-2&p=f&t=PPPENJokvMAepO80-0)

## 🚀 Installation et exécution

1. Cloner le dépôt :
   ```bash
   git clone https://github.com/votre-equipe/youcode-events.git
   ```
2. Accéder au dossier :
   ```bash
   cd youcode-events
   ```
3. Ouvrir le fichier `index.html` dans votre navigateur web.