## interaction_lift

interaction_lift est un script 100% standalone permettant aux joueurs d’interagir physiquement entre eux pour aider à monter ou se hisser grâce à des mécaniques réalistes de support (Legs Up & Pull Up).

Le script est conçu pour être immersif, optimisé, et totalement indépendant de tout framework (ESX / QBCore / etc.).

### Dependencies

#### Required

Aucune 
Le script fonctionne 100% standalone

Optional (auto-detected)

ox_target

ContextMenu

Le script détecte automatiquement les ressources disponibles et s’adapte sans configuration supplémentaire.


### Features

### 🦵 Legs Up (Courte échelle)

- Un joueur peut servir de support pour permettre à un autre de monter

- Vérifications de position, hauteur et environnement

- Animation synchronisée

- Interaction via target ou menu contextuel

### 🧗 Pull Up (Aide à la montée)

- Aide un joueur à se hisser depuis un rebord

- Distance minimale et maximale configurable

- Gestion physique propre (pas de glitch / boost)

### Smart Interaction System

- Support activable via :

- ox_target (Third Eye)

- ContextMenu

- Touches clavier (fallback)

- Labels & icônes dynamiques (ex : “Support actif”)

- Impossible de s’auto-cibler

- Impossible de spam (cooldown visuel)

### Proxy Ped System (Third Eye Compatible)

- Pour contourner les limitations de targeting sur les peds en animation :

- Création d’un proxy ped réseau

- Visible et ciblable par tous les joueurs

- Identifiant réseau partagé (netId)

- Suppression synchronisée côté serveur

- Aucun impact visuel pour le joueur support

### Security & Safety

- Le support est automatiquement désactivé si :

- Le joueur prend des dégâts

- Le joueur est tazé

- Le joueur meurt

- Le joueur tombe / ragdoll

- Le joueur quitte le serveur

### Nettoyage serveur + client garanti (aucun proxy fantôme)

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

Script / System	Status
ox_target	✅ Full
ContextMenu	✅ Full
ESX	❌ Not required
QBCore	❌ Not required
Standalone	✅ 100%
