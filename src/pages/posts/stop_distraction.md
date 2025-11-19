---
layout: ../../layouts/post.astro
title: "Comment j'ai contrôlé mon addiction aux distractions"
pubDate: 2025-07-30
description: "Comment j'ai réussi à reprendre le contrôle de mon temps en réduisant les distractions."
author: "Virgile"
isPinned: false
excerpt: Découvrez les méthodes concrètes que j'ai utilisées pour limiter les distractions numériques et reprendre le contrôle de mon temps au quotidien
image:
  src:
  alt:
tags: ["discipline"]
spotifyEmbed: "https://open.spotify.com/embed/episode/3uLKdXWGQhxqaiDUkMw1bN"
---

### Blocage de distractions : 
- Réseaux sociaux
- Sites de streaming (films/anime)
- Tout élément susceptible de consommer mon temps sans que je l'aie décidé
---
# Update 19/11/2025

Beaucoup de choses ont changé depuis quelques mois, mes méthodes de contrôle ont évolué, c'est pourquoi je veux en faire part ici.

## Sur mobile 📱

J'utilise un [Google Pixel 8](https://support.google.com/pixelphone/answer/7158570?hl=fr#zippy=%2Cpixel) qui tourne sous Android, ce qui me permet d'aller plus loin dans la personnalisation du système que des téléphones sous iOS, ce que je vais expliquer est donc uniquement valable pour les téléphones Android.

## Modification du launcher pour [**Indistractable**](https://www.indistractable.xyz/)
Le launcher c'est ce qui gère une partie importante de l'affichage du téléphone.

<div class="my-4">
  <p class="text-center">Il transforme l'interface du téléphone comme ça :</p>
  <div class="flex flex-col md:flex-row md:gap-18 items-center justify-center">
    <img src="/images/imagePixel.webp" alt="Interface launcher Pixel" title="Interface avec le launcher Pixel" class="rounded-lg shadow-xl max-h-96 max-w-full" />
    <img src="/images/imageIndistractable.webp" alt="Interface launcher Indistractable" title="Interface avec le launcher Indistractable" class="rounded-lg shadow-xl max-h-96 max-w-full" />
  </div>
</div>

Cette interface simpliste me permet d'utiliser mon téléphone pour une action prédéfinie avant son ouverture, rien ne distrait l'utilisateur entre l'ouverture du téléphone et la réalisation de sa tâche.
<br>
L'installation du launcher est simple et le retour arrière est possible à tout moment.

## Application [**Ascent**](https://ascent-app.com/)
Cette application permet d'ajouter un **timer avant d'accéder à certaines applications** choisies. Je l'ai mis en place pour lutter contre un comportement que j'avais, le fait d'ouvrir presque frénétiquement Strava, mes mails et rafraîchir en boucle. En ajoutant un timer avant l'ouverture de ces applications, le comportement s'est effacé.

## Suppression de presque toutes les notifications 🔔
Les seules notifications que j'ai gardées sont celles des messages directs sur mes différentes applications, et celles de mes tâches [Google Tasks](https://tasks.google.com/tasks/). Mis à part ces deux cas je n'ai plus de notifications sur mon téléphone.


---
# Post original 30/07/2025


## Sur mobile 📱
**Désinstallation des applications** distrayantes et utilisation de l'application **[StayFree](https://stayfreeapps.com/)**.

### Désinstallation des applications

Rendre l'utilisation des services aussi restrictive que possible, conformément à la méthode proposée par James Clear dans _Atomic Habits_ : « make it unsatisfying ». Accéder à YouTube, Twitch, etc., via un navigateur plutôt qu'une application permet de réduire significativement le temps passé sur ces services.

### StayFree
La deuxième action qui m'a permis de quasiment cesser d'utiliser mon téléphone est [StayFree](https://stayfreeapps.com/). Cette application gratuite permet de fixer des limites de temps sur l'utilisation des sites ou applications et de les bloquer une fois la limite dépassée. Bien que contournable, cela complique suffisamment l'accès pour faire disparaître progressivement l'habitude d'utiliser constamment son téléphone.

## Sur PC 💻
**Extensions de navigateur** et blocage via le **fichier `/etc/hosts`**.

### Extensions chrome

- [uBlock Origin](https://chromewebstore.google.com/detail/ublock-origin/cjpalhdlnbpafiamejdnhcphjbkeiagm)
    
    La fonctionnalité « Element picker mode » permet de sélectionner et supprimer visuellement des éléments de pages web.



- [Unhook](https://chromewebstore.google.com/detail/unhook-remove-youtube-rec/khncfooichmfjbepaaaebmommgaepoid) ou [UnTrap for YouTube](https://chromewebstore.google.com/detail/untrap-for-youtube/enboaomnljigfhfjfoalacienlhjlfil)

    Extensions spécialement dédiées à YouTube pour supprimer certaines parties du site, rendre floues les miniatures, ajouter un filtre noir et blanc, définir le nombre de vidéos recommandées...



- [Remove Twitch Recommended Channels, Live Chat](https://chromewebstore.google.com/detail/remove-twitch-recommended/kgoadafofbfjlfofcogilchhnabiffnh)

  Extension pour Twitch permettant de supprimer des éléments sur le site web.

### Fichier `/etc/host`
Modifier ce fichier pour ajouter une URL la rend inaccessible depuis votre ordinateur. Toutefois, j'ai appris avec l'expérience que l'édition simple de ce fichier était insuffisante, car dans les moments de tentation, je commentais simplement les lignes du fichier.

Pour remédier à cela, j'ai ajouté un flag `schg` sur le fichier `/etc/hosts`, ce qui rend le fichier immuable (non modifiable) sauf dans certains cas rares que je ne partagerai pas ici, car connaître la solution peut réactiver l'addiction (DYOR).

#### Sur **Mac OS** :
- Ouvrez un terminal
- Éditez le fichier avec un éditeur de texte (par exemple : nano, vi, vim, nvim...)
    ```bash
    sudo nvim /etc/hosts
    ``` 
- Ajoutez à la fin du fichier les sites à bloquer
    ```text
    127.0.0.1 www.twitch.tv
    127.0.0.1 twitch.tv
    127.0.0.1 www.youtube.com
    127.0.0.1 youtube.com
    ...
    ```
- Enregistrez le fichier puis appliquez les modifications (un redémarrage fonctionne très bien aussi)
    ```bash
    sudo killall -HUP mDNSResponder
    ```
⚠️ **Je ne recommande pas l’étape suivante si vous n’avez pas de solides bases en informatique** (enlever le flag sur Mac est très complexe)
- Ajoutez le flag `schg` (assurez-vous d'avoir listé tous les sites avant)
    ```bash
    sudo chflags schg /etc/hosts
    ```

#### Sur **Windows** :
- Ouvrez PowerShell en tant qu'administrateur
- Ouvrez le fichier `/etc/hosts` dans un bloc note
    ```bash
      notepad $env:SystemRoot\System32\drivers\etc\hosts
    ```
- Ajoutez à la fin du fichier les sites à bloquer
    ```text
    127.0.0.1 www.twitch.tv
    127.0.0.1 twitch.tv
    127.0.0.1 www.youtube.com
    127.0.0.1 youtube.com
    ...
    ```
- Enregistrez puis videz le cache DNS
  ```bash
    ipconfig /flushdns
    ```
  
# Conclusion
Ces outils m'ont aidé à gagner du temps de vie, mais ce temps gagné doit être utilisé pour autre chose, sinon vous retomberez dans vos vieux démons. Remplacez ces distractions par du sport, de la lecture, du développement, de l'art… ce qui vous plaît !