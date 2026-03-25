<div align="center">
  <img src="https://readme-typing-svg.demolab.com?font=Fira+Code&weight=600&size=40&pause=1000&color=0073AA&center=true&vCenter=true&width=800&height=100&lines=Projet+de+Stage+:+E-Commerce;Boutique+WordPress+&+WooCommerce" alt="Typing SVG" />
</div>

<p align="center">
  <img src="https://img.shields.io/badge/WordPress-%23117EB9.svg?style=for-the-badge&logo=wordpress&logoColor=white" alt="WordPress" />
  <img src="https://img.shields.io/badge/WooCommerce-96588A.svg?style=for-the-badge&logo=woocommerce&logoColor=white" alt="WooCommerce" />
  <img src="https://img.shields.io/badge/PHP-%23777BB4.svg?style=for-the-badge&logo=php&logoColor=white" alt="PHP" />
  <img src="https://img.shields.io/badge/MySQL-%234479A1.svg?style=for-the-badge&logo=mysql&logoColor=white" alt="MySQL" />
  <img src="https://img.shields.io/badge/Gutenberg-%23000000.svg?style=for-the-badge&logo=wordpress&logoColor=white" alt="Gutenberg" />
</p>

# 📖 Documentation Technique du Projet

Bienvenue dans la documentation technique de ce projet de stage. L'objectif principal est la création, la personnalisation et la gestion d'une boutique en ligne (e-commerce) complète, robuste et esthétique en s'appuyant sur le CMS **WordPress** et sa solution phare **WooCommerce**.

## 🚀 Fonctionnalités Principales

- **Déploiement d'une Boutique en Ligne** : Mise en place d'un catalogue de produits, gestion du panier d'achat, et configuration du processus de commande.
- **Design et Mise en Page Modulaires** : Utilisation de modèles de démarrage et d'éditeurs de blocs avancés.
- **Formulaires Hautement Personnalisés** : Suivi, engagement client et prise de contact fluide grâce à des extensions dédiées (SureForms, Contact Form 7).
- **Navigation Optimisée (Filtres)** : Recherche multicritères perfectionnée pour les produits grâce à Filter Everything.
- **Support & Interaction en Temps Réel** : Module de messagerie instantanée via WP Live Chat Support pour un meilleur taux de conversion.
- **Automatisation & Suivi SEO** : Mise en place de règles automatisées via SureTriggers et optimisation du référencement via SureRank.
- **Mode Catalogue** : Capacité de transformer la boutique en simple catalogue vitrine grâce à ELEX WooCommerce Catalog Mode.

## 🎨 Thèmes Utilisés

Le design visuel de la boutique repose de manière stratégique sur des thèmes renommés pour leurs performances et leur flexibilité de conception :

- **[Astra](https://wpastra.com/)** : Un thème réputé pour son extrême légèreté (optimisation du temps de chargement) et son haut niveau de personnalisation. Idéal pour une intégration native fluide avec WooCommerce.
- **[Kadence](https://www.kadencewp.com/)** : Un thème très performant doté de nombreuses options avancées, offrant un grand contrôle sur tout le design (en-têtes, pieds de page de type "builder").
- *Thèmes Natifs inclus* : Twenty Twenty-Two, Twenty Twenty-Three, Twenty Twenty-Four, Twenty Twenty-Five en cas de besoin ou en guise de thèmes de secours.

## 🔌 Extensions (Plugins) Majeures Intégrées

Les fonctionnalités ont été étendues grâce aux plugins suivants, soigneusement configurés :

### E-Commerce & Edition
- **WooCommerce** : Le moteur transactionnel de la boutique (gestion produits, commandes, taxes, livraisons).
- **Astra Sites & Kadence Starter Templates** : Permettent l'importation de librairies de modèles et sections pré-conçues pour un gain de temps considérable lors de l'intégration.
- **Ultimate Addons for Gutenberg** : Enrichit considérablement l'éditeur natif de WordPress avec des blocs avancés.

### Formulaires, SEO & Automation
- **SureForms** / **SureRank** / **SureTriggers** : Suite de plugins pour implémenter des formulaires de capture de leads, fluidifier et améliorer le classement de la boutique (SEO), et interconnecter des événements entre les plateformes.
- **Contact Form 7** : Permet la création des formulaires de contact standard et fiables pour un usage administratif classique.

### Fonctionnalités Spécifiques
- **Filter Everything** : Met en œuvre un filtrage à facettes intuitif pour trouver rapidement des produits par couleurs, prix, tailles ou autres attributs.
- **ELEX WooCommerce Catalog Mode** : Apporte le mode d'affichage sans boutons d'achat ("catalogue seul"), si nécessaire.
- **WP Live Chat Support** : Interface d'assistance par messagerie pour augmenter les ventes en assistant les visiteurs.
- **Akismet Anti-Spam** : Défense automatique efficace contre les spams postés dans les commentaires ou via les formulaires.

## 📂 Structure du Répertoire du Projet

- 📁 `wordpress/` : Contient l'intégralité des fichiers sources du site et du moteur de développement. Vous y retrouverez notamment les dossiers système de l'application : `wp-content/themes` (pour Astra et Kadence) et `wp-content/plugins` (pour l'ensemble des modules pré-installés).
- 💾 `stage.sql` : Le fichier d'export contenant la structure de la base de données relationnelle (MySQL/MariaDB) ; cela inclut l'intégralité des tables, de la configuration globale, des réglages des thèmes/plugins ainsi que toutes les fiches produits créées.

## 🛠️ Installation et Déploiement en Local

Voici les instructions de base pour faire tourner ce projet sur un environnement de développement local.

1. **Prérequis Serveur** : Disposer d'une pile logicielle comme XAMPP, WAMP, MAMP, ou un outil dédié tel que Local by Flywheel (incluant un serveur Web comme Apache/Nginx, PHP 7.4+, et MySQL/MariaDB).
2. **Transfert de Fichiers** : Copiez ou déplacez le dossier `wordpress/` dans le répertoire d'exécution racine de votre environnement local (ex. le dossier `htdocs` ou `www`).
3. **Mise en Place de la Base de Données** :
   - Depuis phpMyAdmin (ou autre gestionnaire SQL), créez une nouvelle base de données locale (exemple de nom : `bd_stage`).
   - Procédez à l'importation totale du fichier de dump **`stage.sql`** dans cette nouvelle base de données vierge.
4. **Configuration de la Connexion (`wp-config.php`)** :
   - Dans le dossier `wordpress/`, rouvrez (ou dupliquez `wp-config-sample.php` en) le fichier `wp-config.php`.
   - Modifiez les constantes dédiées avec vos propres identifiants locaux : `DB_NAME`, `DB_USER` (souvent `root`), `DB_PASSWORD` (souvent laissé vide), et `DB_HOST` (souvent `localhost`).
5. **Ajustement Temporaire des URLs** :
   - Les URLs dans le dump `stage.sql` font potentiellement référence à l'URL du serveur précédent ou à une adresse spécifique de développement.
   - Pour assurer la redirection locale sans conflit (par exemple vers `http://localhost/wordpress`), modifiez directement ces deux constantes temporairement dans votre `wp-config.php` (avant la ligne de charge principale) :
     ```php
     define( 'WP_HOME', 'http://localhost/wordpress' );
     define( 'WP_SITEURL', 'http://localhost/wordpress' );
     ```
   - (Alternativement) Exécutez une requête SQL d'UPDATE sur la table `wp_options` pour les clés `siteurl` et `home` avec l'outil de gestion de BDD de votre choix ou via *WP-CLI*.
6. **Lancement** : 
   - Ouvrez votre navigateur et naviguez vers votre URL locale `http://localhost/wordpress` pour apprécier le site. Note d'accès : Le tableau de bord de l'administrateur reste accessible via `/wp-admin`.

---

> *Ce document synthétique récapitule la stack technique et les outils associés choisis afin de développer ce projet de stage e-commerce avec polyvalence et professionnalisme.*
