Cordova

1) Il vous faut android studio pour pouvoir lancer l'application sur portable.  
2) Il vaut mieux le faire tourner sur votre t�l�phone que l'�mulateur car sur l'�mulateur cela bug un peu pour notre cas
3) Une fois l'application lancer sur le portable, il faut pas oublier d'activer la g�olocalisation sur votre portable, si vous voyez une erreur apparaitre comme "error: The Geolocation service failed", il faut fermer/kill l'app sur votre android j'insiste sur cela il ne faut pas juste fermer l'application et le rouvrir il faut le kill et ensuite le relancer, normalement �a devrait vous localiser.
4) La g�olocalisation risque de prendre un petit peu de temps pour vous localiser 


Electron

1) Il faut faire la commande "npm start" depuis le terminal dans le dossier "map electron" et l'application se lancera.

Bug rencontr�s pour electron

La g�olocalisation sur electron ne fonctionne pas, il faut y ajouter un module google map API g�rant la g�olocalisation. Nous avons essay� plusieurs modules google map API tels que "google-maps", "google-maps-api", "googlemaps" et d'autres; mais il s'av�re que le service de g�olocalisation n'est pas fournit � travers ces modules ou la documentation fournit avec est incompl�te voir imcompr�hensible.
Nous avons n�anmoins essay� d'autres utilitaires comme electron � savoir appjs et nwjs, mais les r�sultats ne sont pas convainquants (par exemple appjs nous donne une erreur de type o� le navigateur ne supporte pas la g�olocalisation).