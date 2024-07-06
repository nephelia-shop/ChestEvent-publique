# ChestEvent
Des coffres avec des objets précieux apparaissent dans des endroits pré-définis, se remplissent et disparaissent au fil du temps.

## Fonctionnalités
- Apparition et disparition automatiques des coffres.
- Temps de remplissage configurable pour le contenu des coffres.
- Durée de l'événement personnalisable.
- FloatingText gérant les coffres des events
- Commandes de gestion d'événements complètes.
- Messages de diffusion pour les mises à jour de l'événement.

## Installation
1. **Télécharger le Plugin**
    - Téléchargez la dernière version du plugin ChestEvent depuis ce [lien](https://github.com/nephelia-shop/ChestEvent).
2. **Télécharger le TexturePack (Pour les inventaires)** 
    - Téléchargez la dernière version du texture pack depuis ce [lien](https://github.com/tedo0627/InventoryUIResourcePack/releases/).

## Configuration
La configuration de ChestEvent se fait via le fichier `config.yml`, voici les informations qui le concernent :

```yaml
settings:
  timer: 120  # Durée de l'événement en secondes (2 minutes)
  shuffleItems: true  # Mélanger les objets dans les coffres à chaque remplissage
  spawnOnStart: true  # Faire apparaître les coffres au démarrage du serveur
  canOpenOnOff: false  # Permettre l'ouverture des coffres même si l'événement est désactivé
  autorefill:
    enabled: true  # Activer le remplissage automatique des coffres
    cooldown: 10  # Délai de remplissage automatique en secondes
```
- **timer**: La durée de l'événement en secondes.
- **shuffleItems**: Si activé, mélange les objets dans les coffres à chaque remplissage.
- **spawnOnStart**: Si activé, fait apparaître les ChestEvent au démarrage du serveur.
- **canOpenOnOff**: Permet d'ouvrir des coffres même si l'événement est désactivé.
- **autorefill**: Remplissage automatique des coffres avec un délai spécifié en secondes.

## Commandes
- **/chestevent create (name)** : Crée un chest event.
- **/chestevent edit (name)** : Modifie le contenu d'un coffre (items).
- **/chestevent start (timer = 10 secondes)** : Lancement du chestevent (10 secondes).
- **/chestevent stop** : Stoppe le chestevent.
- **/chestevent info** : Informations à propos du chestevent (**ChestEvent** → _position_).
- **/chestevent spawn** : Spawn test des chestevents.
- **/chestevent despawn** : Despawn test des chestevents.

## Permission
- **nepheliashop.chestevent**: Cette permission permet d'utiliser la commande et de bypass l'ouverture des coffres lorsque l'event est OFF.

## Support et Contribution
Pour toute question, problème ou demande de fonctionnalité, rejoignez notre communauté sur [Discord](https://discord.gg/pocketmine).

