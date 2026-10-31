YULIA JACQUES — MISE À JOUR DU SITE (31 OCTOBRE 2026)

PROBLÈME CORRIGÉ
Le site public affiche encore l'ancien widget Calendly et la mention "par téléphone".
Cette version retire Calendly, remplace la réservation par le lien Google Agenda
et indique clairement Google Meet (30 min) et les langues FR / EN / RU.

LIEN DE RÉSERVATION
https://calendar.app.google/RwhKF2XNBLoir8R66

COMMENT PUBLIER SUR GITHUB PAGES
1. Ouvrez le dépôt GitHub QUI ALIMENTE yuliajacques.com.
2. Dans Settings > Pages, vérifiez la branche et le répertoire source (racine / ou /docs).
3. Dans ce répertoire SOURCE, remplacez au minimum "site.js" et "styles.css"
   par les fichiers présents dans cette archive. Pour mettre tout le site à jour,
   remplacez également index.html, coaching.html, about.html, contact.html et
   tarifs.html, et les fichiers à l'intérieur du dossier assets.
4. NE PAS déposer le fichier ZIP ni le dossier "yulia_jacques_publication_2026_10_31"
   comme sous-dossier dans le dépôt. Il faut téléverser LE CONTENU du dossier.
5. Conserver tout fichier CNAME, .nojekyll, et la configuration GitHub Pages.
6. Cliquez sur "Commit changes"; contrôlez Actions / Pages si nécessaire.
7. Ouvrez https://yuliajacques.com/contact.html?lang=fr#booking, faites
   Cmd+Shift+R (Mac) ou ouvrez une fenêtre privée. Vérifiez la disparition
   du logo Calendly et la présence du bouton "Google Agenda".
8. Faites une réservation d'essai : le formulaire Google doit demander la langue.

DIAGNOSTIC SI L'ANCIEN MODULE RESTE EN PLACE
Dans GitHub, ouvrez "site.js" dans le répertoire publié : cherchez "Calendly".
Il ne doit plus être présent. Cherchez "BOOKING_URL" : il doit contenir
"https://calendar.app.google/RwhKF2XNBLoir8R66".
Si c'est correct sur GitHub mais pas sur yuliajacques.com, vérifiez
Settings > Pages (branche/répertoire), Actions > dernier déploiement,
puis faites un rafraîchissement forcé de la page.

La génération de ces fichiers ne publie rien automatiquement.
