# `insopti PowerPlan`

Ce script importe et active mon plan d'alimentation personnalisé **insopti PowerPlan**, conçu pour maximiser la réactivité du système et réduire au minimum la latence. Il télécharge automatiquement le fichier de configuration `.pow` depuis GitHub, l'importe dans Windows et l'active. Tout est **sûr**, **optimisé** et **entièrement réversible**.

# `1` Installation & Lancement

Faites un **clic droit** sur le fichier `.ps1` → **"Exécuter avec PowerShell"**.  
Le script demandera automatiquement les droits administrateur.

> [!CAUTION]
> Si vous n'avez pas l'autorisation d'exécuter des scripts PowerShell, activez-la d'abord via :
> ```
> Set-ExecutionPolicy RemoteSigned -Scope CurrentUser
> ```

Une fois lancé, le script vous proposera de choisir le profil adapté à votre configuration CPU.

# Choix du plan

| Option | Description |
|---|---|
| **`1` Static OC mode** | Pour les utilisateurs avec une fréquence CPU fixe manuellement et Precision Boost désactivé |
| **`2` Dynamic boost mode** | Pour tous les autres utilisateurs avec Precision Boost / Turbo activé (par défaut dans le BIOS) |

> [!IMPORTANT]
> Si vous ne savez pas lequel choisir, optez pour le **mode Dynamic boost** (`2`). C'est le réglage par défaut pour la majorité des configurations.

# `2` Ce que fait le script

| Optimisation | Ce que ça fait |
|---|---|
| **Import du PowerPlan** | Télécharge et importe le plan d'alimentation `insopti` dans Windows |
| **Activation automatique** | Active le plan immédiatement après l'import |
| **CPU no-throttle** | Désactive le bridage de fréquence CPU et les fonctions de mitigation de latence |
| **CPU Unparking** | Débloque tous les cœurs CPU (comme ParkControl) — aucun cœur n'est mis en veille par Windows |
| **USB Power Management** | Optimise la gestion d'alimentation USB pour réduire l'input delay |
| **Sleep state settings** | Configure les états de veille pour une réactivité maximale |

> [!NOTE]
> Le script ne modifie pas de fichiers système permanents. Changer de plan d'alimentation suffit à tout annuler.

# Infos supp

> [!IMPORTANT]
> Ce plan est conçu pour un usage **desktop branché sur secteur**. Son utilisation sur laptop en batterie n'est pas forcement recommandée car il maximise la consommation énergétique en permanence.








<details>
  <summary>Click here for an image example of launch arguments</summary>
  
[img]https://i.imgur.com/c4OZ65Z.png[/img]

</details>




https://i.imgur.com/c4OZ65Z.png

<p align="center">
  <sub>©insopti — <a href="https://guns.lol/inso.vs">guns.lol/inso.vs</a> | For personal use only.</sub>
</p>
