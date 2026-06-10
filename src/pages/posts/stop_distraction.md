---
layout: ../../layouts/post.astro
title: "Comment j'ai contrôlé mon addiction aux distractions"
pubDate: 2025-07-30
description: "Bloquer les distractions numériques sur mobile et PC : les méthodes et applications que j'utilise pour réduire mon temps d'écran et rester concentré au quotidien."
author: "Virgile"
isPinned: false
excerpt: "J'ai testé beaucoup d'applications et de réglages pour bloquer les distractions sur mon téléphone et mon PC. Voici ce qui a marché pour moi, et comment ça a évolué."
image:
  src:
  alt:
tags: ["discipline", "productivité"]
spotifyEmbed: "https://open.spotify.com/embed/episode/3uLKdXWGQhxqaiDUkMw1bN"
---

### Ce que j'appelle distraction : 
- Réseaux sociaux
- Sites de streaming
- Jeux vidéo
- Tout élément susceptible de consommer mon temps sans que je l'aie décidé
---

### Chronologiquement

<div class="not-prose my-10 text-stone-700 dark:text-stone-300">
  <p class="mb-6 text-xs text-stone-400 dark:text-stone-500"><span class="font-semibold text-stone-700 dark:text-stone-200">gras</span> = encore utilisé&nbsp;·&nbsp;<span class="text-stone-400 line-through decoration-stone-300 dark:text-stone-500 dark:decoration-stone-600">barré</span> = remplacé&nbsp;·&nbsp;<span class="text-sky-600 dark:text-sky-400">mbl</span> mobile&nbsp;·&nbsp;<span class="text-amber-600 dark:text-amber-400">pc</span> ordinateur</p>
  <ol class="relative ms-1 space-y-8 border-s border-stone-300 dark:border-stone-700">
    <li class="ms-7">
      <span class="absolute -start-[5px] mt-2 h-2.5 w-2.5 rounded-full bg-stone-300 dark:bg-stone-600"></span>
      <div class="flex items-baseline gap-2.5">
        <time class="text-sm font-semibold text-stone-900 dark:text-white">30/07/2025</time>
      </div>
      <ul class="mt-2.5 space-y-1.5">
        <li class="flex flex-wrap items-baseline gap-x-2.5"><span class="w-6 shrink-0 text-[10px] tracking-wide text-sky-600/80 uppercase dark:text-sky-400/80">mbl</span><a href="#désinstallation-des-applications" class="font-semibold text-stone-800 underline-offset-4 transition-colors hover:text-orange-600 hover:underline hover:decoration-orange-400/50 dark:text-stone-100 dark:hover:text-orange-400">Désinstallation des apps</a></li>
        <li class="flex flex-wrap items-baseline gap-x-2.5"><span class="w-6 shrink-0 text-[10px] tracking-wide text-sky-600/80 uppercase dark:text-sky-400/80">mbl</span><a href="#stayfree" class="text-stone-400 line-through decoration-stone-300 transition-colors hover:text-orange-500 dark:text-stone-500 dark:decoration-stone-600 dark:hover:text-orange-400">StayFree</a><span class="text-sm text-stone-400 dark:text-stone-500">→ Ascent</span></li>
        <li class="flex flex-wrap items-baseline gap-x-2.5"><span class="w-6 shrink-0 text-[10px] tracking-wide text-amber-600/80 uppercase dark:text-amber-400/80">pc</span><a href="#extensions-chrome" class="font-semibold text-stone-800 underline-offset-4 transition-colors hover:text-orange-600 hover:underline hover:decoration-orange-400/50 dark:text-stone-100 dark:hover:text-orange-400">Extensions Chrome</a></li>
        <li class="flex flex-wrap items-baseline gap-x-2.5"><span class="w-6 shrink-0 text-[10px] tracking-wide text-amber-600/80 uppercase dark:text-amber-400/80">pc</span><a href="#fichier-etchost" class="text-stone-400 line-through decoration-stone-300 transition-colors hover:text-orange-500 dark:text-stone-500 dark:decoration-stone-600 dark:hover:text-orange-400">/etc/hosts + schg</a><span class="text-sm text-stone-400 dark:text-stone-500">→ FocusServer</span></li>
      </ul>
    </li>
    <li class="ms-7">
      <span class="absolute -start-[5px] mt-2 h-2.5 w-2.5 rounded-full bg-stone-300 dark:bg-stone-600"></span>
      <div class="flex items-baseline gap-2.5">
        <time class="text-sm font-semibold text-stone-900 dark:text-white">19/11/2025</time>
      </div>
      <ul class="mt-2.5 space-y-1.5">
        <li class="flex flex-wrap items-baseline gap-x-2.5"><span class="w-6 shrink-0 text-[10px] tracking-wide text-sky-600/80 uppercase dark:text-sky-400/80">mbl</span><a href="#application-ascent" class="text-stone-400 line-through decoration-stone-300 transition-colors hover:text-orange-500 dark:text-stone-500 dark:decoration-stone-600 dark:hover:text-orange-400">Ascent</a><span class="text-sm text-stone-400 dark:text-stone-500">→ ScreenZen</span></li>
        <li class="flex flex-wrap items-baseline gap-x-2.5"><span class="w-6 shrink-0 text-[10px] tracking-wide text-sky-600/80 uppercase dark:text-sky-400/80">mbl</span><a href="#modification-du-launcher-pour-indistractable" class="font-semibold text-stone-800 underline-offset-4 transition-colors hover:text-orange-600 hover:underline hover:decoration-orange-400/50 dark:text-stone-100 dark:hover:text-orange-400">Launcher Indistractable</a></li>
        <li class="flex flex-wrap items-baseline gap-x-2.5"><span class="w-6 shrink-0 text-[10px] tracking-wide text-sky-600/80 uppercase dark:text-sky-400/80">mbl</span><a href="#suppression-de-presque-toutes-les-notifications" class="font-semibold text-stone-800 underline-offset-4 transition-colors hover:text-orange-600 hover:underline hover:decoration-orange-400/50 dark:text-stone-100 dark:hover:text-orange-400">Notifications coupées</a></li>
      </ul>
    </li>
    <li class="ms-7">
      <span class="absolute -start-[5px] mt-2 h-2.5 w-2.5 rounded-full bg-stone-300 dark:bg-stone-600"></span>
      <div class="flex items-baseline gap-2.5">
        <time class="text-sm font-semibold text-stone-900 dark:text-white">27/11/2025</time>
      </div>
      <ul class="mt-2.5 space-y-1.5">
        <li class="flex flex-wrap items-baseline gap-x-2.5"><span class="w-6 shrink-0 text-[10px] tracking-wide text-amber-600/80 uppercase dark:text-amber-400/80">pc</span><a href="#sur-pc" class="text-stone-400 line-through decoration-stone-300 transition-colors hover:text-orange-500 dark:text-stone-500 dark:decoration-stone-600 dark:hover:text-orange-400">FocusServer</a><span class="text-sm text-stone-400 dark:text-stone-500">→ Cold Turkey</span></li>
      </ul>
    </li>
    <li class="ms-7">
      <span class="absolute -start-[5px] mt-2 h-2.5 w-2.5 rounded-full bg-stone-300 dark:bg-stone-600"></span>
      <div class="flex items-baseline gap-2.5">
        <time class="text-sm font-semibold text-stone-900 dark:text-white">01/04/2026</time>
      </div>
      <ul class="mt-2.5 space-y-1.5">
        <li class="flex flex-wrap items-baseline gap-x-2.5"><span class="w-6 shrink-0 text-[10px] tracking-wide text-amber-600/80 uppercase dark:text-amber-400/80">pc</span><a href="#application-cold-turkey" class="font-semibold text-stone-800 underline-offset-4 transition-colors hover:text-orange-600 hover:underline hover:decoration-orange-400/50 dark:text-stone-100 dark:hover:text-orange-400">Cold Turkey</a></li>
      </ul>
    </li>
    <li class="ms-7">
      <span class="absolute -start-[5px] mt-2 h-2.5 w-2.5 rounded-full bg-orange-500 dark:bg-orange-400"></span>
      <div class="flex items-baseline gap-2.5">
        <time class="text-sm font-semibold text-orange-600 dark:text-orange-400">07/04/2026</time>
      </div>
      <ul class="mt-2.5 space-y-1.5">
        <li class="flex flex-wrap items-baseline gap-x-2.5"><span class="w-6 shrink-0 text-[10px] tracking-wide text-sky-600/80 uppercase dark:text-sky-400/80">mbl</span><a href="#application-screenzen" class="font-semibold text-stone-800 underline-offset-4 transition-colors hover:text-orange-600 hover:underline hover:decoration-orange-400/50 dark:text-stone-100 dark:hover:text-orange-400">ScreenZen</a></li>
      </ul>
    </li>
  </ol>
</div>

# Update 07/06/2026

## Sur mobile 📱

J'utilise toujours le launcher [**Indistractable**](https://www.indistractable.xyz/), et mes notifications sont presque toutes supprimées. 

La modification importante depuis le [19/11/2025](#update-19112025). J'ai remplacé l'application [**Ascent**](https://ascent-app.com/) par [**ScreenZen**](https://screenzen.co/). J'avais observé un problème d'optimisation dans Ascent qui dévorait la batterie très rapidement, d'où le changement.

## Application [**ScreenZen**](https://screenzen.co/)

Quatre groupes de blocage :

1. **20 s d'attente** (avec une raison à écrire, fermeture automatique après 15 min) : uniquement **Chrome**.
2. **12 s d'attente** : les applications que j'ouvre par pulsion (**Strava, Gmail, Discord, WhatsApp**...).
3. **Blocage horaire**, sur les mêmes plages que [Cold Turkey](#application-cold-turkey) : les sites qui me distraient (**YouTube, Twitch, Reddit**...).
4. **Blocage total** : tous les sites pornographiques.

<div className="w-full flex justify-center">
<img src="/images/stop_distraction/screenZen1.png" alt="Panneau blocages screenZen" title="Panneau blocages screenZen" class="rounded-lg shadow-xl max-h-96 max-w-full" />
</div>



## Sur PC 💻

J'ai longtemps essayé de développer un outil qui permet de bloquer des sites sur mon Mac, et j'ai fini par en créer un qui fonctionne très bien.
[FocusServer](https://github.com/Virgile-Eratel/focusServer) permet de bloquer une liste de sites définie sur des horaires définis.
Je l'ai longtemps utilisé mais étant donné que je l'ai développé je connais toutes les manières de passer outre. Donc au final il ne permet pas de régler mon problème.

### Application [**Cold Turkey**](https://getcoldturkey.com/)

J'ai donc choisi de payer 35 euros pour une licence payante Cold Turkey, ce qui permet de créer des plages de blocages d'applications et de sites. À noter qu'une version gratuite est aussi disponible et fonctionne très bien.
Cette application est pensée pour être très dure à contourner, donc après plusieurs jours de configuration avec les failles que j'ai pu trouver, les contournements étaient en grande partie plus possibles.
Juste en termes d'exemple de contournement bloqué, j'ai utilisé **VMware Fusion** pour ouvrir ma VM Windows et accéder aux sites bloqués. Il suffit alors de bloquer également l'application **VMware Fusion** sur les plages non autorisées et problème réglé. 

#### Configuration Cold Turkey

![alt text](/images/stop_distraction/coldTurkey1.png)

Trois groupes de blocage :

- **Général** : les sites chronophages que je veux éviter (YouTube, Reddit...). Toujours actif, sauf deux fenêtres autorisées : 12h-13h30 et 18h-20h.
- **All** : bloque tous les sites, quelle que soit leur nature. Il me sert de rappel pour éteindre le Mac le soir : il se déclenche à 22h30 (désactivable), puis à 23h (non désactivable).
- **Porn** : tous les sites pornographiques. Toujours actif. Le seul moyen de le désactiver est de taper 250 caractères aléatoires sans se tromper. Autant dire que je ne le fais jamais.

![alt text](/images/stop_distraction/coldTurkey2.png) 


# Update 19/11/2025

## Sur mobile 📱

J'utilise un [Google Pixel 8](https://support.google.com/pixelphone/answer/7158570?hl=fr#zippy=%2Cpixel) qui tourne sous Android, ce qui me permet d'aller plus loin dans la personnalisation du système que des téléphones sous iOS, ce que je vais expliquer est donc uniquement valable pour les téléphones Android.

## Modification du launcher pour [**Indistractable**](https://www.indistractable.xyz/)
Le launcher c'est ce qui gère une partie importante de l'affichage du téléphone.

<div class="my-4">
  <p class="text-center">Il transforme l'interface du téléphone comme ça :</p>
  <div class="flex flex-col md:flex-row md:gap-18 items-center justify-center">
    <img src="/images/stop_distraction/imagePixel.webp" alt="Interface launcher Pixel" title="Interface avec le launcher Pixel" class="rounded-lg shadow-xl max-h-96 max-w-full" />
    <img src="/images/stop_distraction/imageIndistractable.webp" alt="Interface launcher Indistractable" title="Interface avec le launcher Indistractable" class="rounded-lg shadow-xl max-h-96 max-w-full" />
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
