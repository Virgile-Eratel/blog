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
---

### Blocage de distractions : 
- Réseaux sociaux
- Sites de streaming (films/anime)
- Tout élément susceptible de consommer mon temps sans que je l'aie décidé

# Mes actions

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
- Ajoutez le flag `schg` (⚠️ assurez-vous d'avoir listé tous les sites avant)
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