# Flux : l'appli Android

Ce dossier contient le projet complet de l'appli. GitHub la compile pour toi,
gratuitement, et te donne le fichier **Flux.apk** à installer sur ton téléphone.

## 1. Faire compiler l'appli (une seule fois, environ 10 minutes, sur PC)

1. Crée un compte gratuit sur **github.com** (ou connecte-toi).
2. En haut à droite : **+** → **New repository**. Nom : `flux`, coche **Private**, puis **Create repository**.
3. Sur la page du dépôt vide, clique sur le lien **« uploading an existing file »**.
4. Ouvre ce dossier `flux-android` sur ton PC, sélectionne **tout son contenu**
   (y compris le dossier `.github`) et glisse-le dans la page.
   - Sur Windows, si tu ne vois pas `.github` : Explorateur → Affichage → coche « Éléments masqués ».
   - Ne glisse pas `node_modules` s'il existe (il n'est pas dans le zip).
5. Clique sur **Commit changes**.
6. Va dans l'onglet **Actions** : la compilation démarre toute seule (pastille jaune).
   Elle prend 5 à 8 minutes. Quand elle est verte, c'est prêt.

## 2. Installer sur ton téléphone Android

1. Sur ton téléphone, ouvre la page de ton dépôt GitHub (connecté à ton compte),
   puis **Releases** (à droite, ou en bas sur mobile).
2. Touche **Flux.apk** pour le télécharger.
3. Ouvre le fichier. Android demande d'autoriser l'installation depuis ton navigateur :
   accepte (« Autoriser depuis cette source »), puis **Installer**.
4. Si Play Protect affiche un avertissement (appli inconnue), touche
   « Plus de détails » → « Installer quand même ». C'est normal pour une appli perso
   qui ne vient pas du Play Store.

L'icône Flux (vinyle orange) apparaît dans tes applis.

## Mettre à jour plus tard

Remplace les fichiers modifiés sur GitHub (glisser-déposer → Commit). Une nouvelle
version apparaît dans Releases ; installe-la par-dessus l'ancienne :
tes favoris et tes téléchargements sont conservés.

## Autre option : Android Studio

Si tu as Android Studio : `npm install`, `npx cap sync android`, puis ouvre le
dossier `android` dans Android Studio → Build → Build APK(s).

## Bon à savoir

- La musique vient d'Audius (gratuit, sans pub, légal). Il faut du réseau pour
  découvrir et télécharger. Les morceaux téléchargés (icône ↓) s'écoutent sans connexion.
- Les sons téléchargés restent dans l'appli. Si tu la désinstalles, ils sont supprimés.
- `android/app/flux.keystore` est la clé qui signe l'appli. Garde-la : sans elle,
  les mises à jour ne pourraient plus s'installer par-dessus.
