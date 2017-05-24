Cordova

1) Il vous faut android studio pour pouvoir lancer l'application sur portable.  
2) Il vaut mieux le faire tourner sur votre téléphone que l'émulateur car sur l'émulateur cela bug un peu pour notre cas
3) Une fois l'application lancer sur le portable, il faut pas oublier d'activer la géolocalisation sur votre portable, si vous voyez une erreur apparaitre comme "error: The Geolocation service failed", il faut fermer/kill l'app sur votre android j'insiste sur cela il ne faut pas juste fermer l'application et le rouvrir il faut le kill et ensuite le relancer, normalement ça devrait vous localiser.
4) La géolocalisation risque de prendre un petit peu de temps pour vous localiser 


Electron

1) Il faut faire la commande "npm start" depuis le terminal dans le dossier "map electron" et l'application se lancera.

Bug rencontrés pour electron

La géolocalisation sur electron ne fonctionne pas, il faut y ajouter un module google map API gérant la géolocalisation. Nous avons essayé plusieurs modules google map API tels que "google-maps", "google-maps-api", "googlemaps" et d'autres; mais il s'avère que le service de géolocalisation n'est pas fournit à travers ces modules ou la documentation fournit avec est incomplète voir imcompréhensible.
Nous avons néanmoins essayé d'autres utilitaires comme electron à savoir appjs et nwjs, mais les résultats ne sont pas convainquants (par exemple appjs nous donne une erreur de type où le navigateur ne supporte pas la géolocalisation).