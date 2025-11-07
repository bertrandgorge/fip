# Fip et France Musique

Petit projet pour avoir un player léger pour Fip et France Musique.

- Très léger, pas de pub, pas d'éléments superfétatoires
- Compatible chromecast (flux aac hifi)
- Flux hifi HLS sur le navigateur
- Compatible avec les boutons pause/play/next/prev bluetooth (dans la voiture ou sur le casque), permet de passer d'une station à l'autre
- Affichage des titres en bluetooth
- Fonctionne sur téléphone, peut être enregistré comme icone sur l'écran d'accueil (web app) pour remplacer complètement l'application Radio France
- Possibilité de démarrer sur une radio en particulier en ajoutant ?radio=fiprock par exemple
- Utilise l'API GraphQL Radio France pour récupérer les titres des morceaux en cours (sur un intervale de 30s pour ne pas être trop lourd)

Dépendances :
- Utilise l'[API native de Google](https://developers.google.com/cast/docs/reference/web_sender?hl=fr) pour la partie ChromeCast (fonctionne mieux sur Chrome)
- https://github.com/video-dev/hls.js est utilisé pour HLS (en local)
- Voir l'[API Radio France](https://developers.radiofrance.fr/doc) pour la récupération des titres
- Bootstrap et jQuery

Limites :
- En utilisation avec Android Auto, les applis web ne peuvent pas s'intégrer correctement (nécessite de passer par des apps natives), et l'utilisation des boutons prev/next ne passe pas d'une radio à l'autre mais déclenche le démarrage de la première app musicale native trouvée...