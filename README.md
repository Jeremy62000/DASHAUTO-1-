# DashAuto v4 (design moderne)

Accueil pour autoradio Android (1024x600) : horloge, météo (température, min/max, pluie), compteur de vitesse GPS en jauge (+ trajet : distance, durée, moyenne, max), Waze et Spotify en grosses tuiles, boutons précédent / lecture / suivant, dock de raccourcis (AutoLink, Navi, Maps, Radio, Bluetooth, YouTube) et liste de toutes les apps.

Waze et Spotify tournent directement sur l'écran : il faut Internet (partage de connexion du téléphone) et se connecter à ses comptes une fois. Si l'app manque, la tuile affiche « Installer » et ouvre le Play Store.

## Compiler l'APK (gratuit)
1. Dépôt GitHub **public** (aucun secret dedans) avec tout le contenu de ce dossier.
2. Onglet **Actions** → **Build APK** (~3 min), puis onglet **Releases** : `app-debug.apk`.

## Installer sur l'écran (sans USB)
1. Partage de connexion du téléphone → écran en Wi-Fi → **Chrome** sur l'écran → page Releases → télécharge `app-debug.apk`.
2. **FileManager** → Download → touche l'APK (ou **ApkInstaller**).
3. Home → **DashAuto → Toujours**. Autorise la **localisation** au premier lancement.

## Connexion automatique à chaque trajet
- Sur l'écran : enregistre le réseau du téléphone une fois ; il se reconnecte seul quand il le voit.
- Sur le téléphone : désactive l'arrêt automatique du point d'accès. Option : une routine (Samsung Routines, Tasker…) qui active le point d'accès à la connexion Bluetooth de la voiture.

## Personnaliser
`app/src/main/assets/index.html` : bloc `DOCK` (raccourcis du bas), `LAT/LON` (météo), couleurs en haut du fichier.
