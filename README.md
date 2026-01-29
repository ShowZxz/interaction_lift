## interaction_lift

interaction_lift est un script 100% standalone permettant aux joueurs d’interagir physiquement entre eux pour aider à monter ou se hisser grâce à deux mécaniques réalistes (Legs Up & Pull Up).

Le script est conçu pour être immersif, optimisé, et totalement indépendant de tout framework (ESX / QBCore / ContexMenu / etc.).

Il a été conçus pour être utilisable dans les serveurs RP et les serveurs PVP pour offrir une meilleur exploitation de la map gta V de façon RP

### Dependencies

#### Required

- Aucune le script fonctionne 100% standalone

#### Optional (auto-detected)

- ox_target

- ContextMenu

- Le script détecte automatiquement les ressources disponibles et s’adapte sans configuration supplémentaire.


### Features

### 🦵 Legs Up (Courte échelle)

- Un joueur peut servir de support pour permettre à un autre de monter

- Vérifications de position, hauteur et de l'environnement

- Animation synchronisée

- Interaction via ox_target ou ContextMenu (optional)

### 🧗 Pull Up (Aide à la montée)

- Aide un joueur à se hisser depuis un rebord

- Distance minimale et maximale configurable + Durée de l'animation réglabe via Config.lua

- Gestion physique propre (pas de glitch / boost)

### Smart Interaction System

#### Support activable via :

- ox_target (Third Eye)

- ContextMenu

- Touches clavier (fallback) Standalone

- Impossible de s’auto-cibler

- Impossible de spam (cooldown visuel)

### Proxy Ped System (Third Eye Compatible)

#### Pour contourner les limitations de targeting sur les peds en animation :

- Création d’un proxy ped réseau

- Visible et ciblable par tous les joueurs

- Identifiant réseau partagé (netId)

- Suppression synchronisée côté serveur + Gestion des crash

- Aucun impact visuel pour le joueur support

### Securité & Safety

#### Le support est automatiquement désactivé si :

- Le joueur prend des dégâts

- Le joueur est tazé

- Le joueur meurt

- Le joueur tombe / ragdoll

- Le joueur quitte le serveur ou crash

- Nettoyage serveur + client garanti (aucun proxy fantôme)

### Configuration

- Toutes les options sont centralisées dans config.lua :

- Distances min / max par mode

- Cooldowns

- Touches clavier

- Animations

- Modes activés / désactivés

### Performance

- Aucun thread lourd permanent

- Threads actifs uniquement en interaction

- Proxy peds créés uniquement quand nécessaire

- Impact CPU quasi nul en idle

- Compatible serveurs low / mid / high population

### Compatibility

Standalone	✅ 100%

ox_target	✅ Full

ContextMenu	✅ Full

ESX	❌ Not required

QBCore	❌ Not required
