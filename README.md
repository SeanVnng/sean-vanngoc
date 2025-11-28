# ⚡ Sean Van Ngoc - Portfolio Personnel

![HTML5](https://img.shields.io/badge/HTML5-E34F26?style=for-the-badge&logo=html5&logoColor=white)
![Tailwind CSS](https://img.shields.io/badge/Tailwind_CSS-38B2AC?style=for-the-badge&logo=tailwind-css&logoColor=white)
![JavaScript](https://img.shields.io/badge/JavaScript-F7DF1E?style=for-the-badge&logo=javascript&logoColor=black)
![Design](https://img.shields.io/badge/Design-Minimalist-black?style=for-the-badge)

**Sean Van Ngoc | Portfolio** est une interface web immersive de nouvelle génération ("Electric Blue Edition"). Il ne se contente pas d'afficher du texte : **il offre une expérience fluide**. Grâce à l'intégration de **Lenis Scroll** et d'un système **i18n natif**, le site s'adapte instantanément à la langue et au thème de l'utilisateur, le tout sans aucun rechargement de page.

---

## ✨ Fonctionnalités Principales

* **🎨 UI/UX Immersive :**
    * **Design "Electric Blue" :** Esthétique épurée avec grille interactive en arrière-plan.
    * **Animations Reveal :** Apparition séquencée des éléments au défilement (Intersection Observer).
    * **Smooth Scroll :** Navigation ultra-fluide grâce au moteur *Lenis*.
* **🌍 Internationalisation (i18n) :**
    * Traduction **FR / EN** instantanée via JavaScript (DOM Manipulation).
    * Aucun rechargement de page nécessaire.
    * Détection automatique de la langue préférée.
* **🌗 Gestion de Thème Avancée :**
    * **Dark Mode :** Support natif avec persistance des préférences (LocalStorage).
    * **Glassmorphism :** Effets de flou (backdrop-blur) sur le header et les menus.
* **🛠️ Stack Technique Légère :**
    * **Zero-Build :** Utilisation de Tailwind CSS via CDN pour un prototypage ultra-rapide.
    * **Icônes Vectorielles :** Intégration de la librairie *Lucide Icons*.
    * **Responsive :** Interface Mobile-First parfaitement adaptée à tous les écrans.

---

## ⚙️ Prérequis

Ce projet étant statique (Frontend uniquement), les prérequis sont minimes :

* Un **Navigateur Web Moderne** (Chrome, Firefox, Safari, Edge).
* **Git** (Pour cloner le projet).
* *(Optionnel)* **VS Code** avec l'extension "Live Server".

---

## 🚀 Installation

1.  **Cloner le dépôt :**
    ```bash
    git clone [https://github.com/SeanVnng/ton-repo.git](https://github.com/SeanVnng/ton-repo.git)
    cd ton-repo
    ```

2.  **Lancer le projet :**
    Il n'y a pas de dépendances NPM à installer.
    
    * **Option A (Simple) :** Double-cliquez simplement sur le fichier `index.html`.
    * **Option B (Recommandée) :** Si vous utilisez VS Code, faites un clic droit sur `index.html` et choisissez `Open with Live Server`.

---

## 🎮 Configuration & Personnalisation

### 1. Modifier les Textes (Traductions)
Le site utilise un dictionnaire JSON interne situé dans `script.js`.

* Ouvrez `script.js`.
* Modifiez l'objet `translations` au début du fichier :

    ```javascript
    const translations = {
        fr: {
            hero_subtitle_1: "Votre nouveau texte ici...",
            // ...
        },
        en: {
            hero_subtitle_1: "Your new text here...",
            // ...
        }
    };
    ```

### 2. Ajouter un Projet
Pour ajouter une entrée dans la section "Projets", éditez `index.html` dans la section `<section id="work">`.

Copiez le bloc suivant et adaptez le contenu :

```html
<a href="LIEN_GITHUB" target="_blank" class="project-item group py-12 flex ... reveal">
    <div class="md:w-1/4 z-10">
        <span class="badge-style...">TAGS</span>
    </div>
    <div class="md:w-2/4 z-10">
        <h3 class="text-3xl..." data-i18n="ID_TRADUCTION">Titre du Projet</h3>
        <p class="opacity-60 text-sm">Description technique</p>
    </div>
    </a>
```

## 📂 Structure du Projet

L'architecture du projet est conçue pour être **légère et maintenable**. Tout tient en trois fichiers principaux, sans dossiers complexes ni dépendances lourdes.

```bash
.
├── index.html      # 🏗️ Cœur du site : Structure DOM, textes et import Tailwind
├── style.css       # 🎨 Design System : Variables CSS (:root), animations et Dark Mode
├── script.js       # 🧠 Logique : Dictionnaire de traduction (i18n) et interactivité
└── README.md       # 📖 Documentation du projet

Réalisé par Seann
