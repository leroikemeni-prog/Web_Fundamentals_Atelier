# 📒 Mon carnet de bord

**Nom :** 

**Prénom :** 

**Adresse de mon site :** https://______.pythonanywhere.com

> Modifiez ce fichier directement sur GitHub (icône crayon ✏️) pour répondre aux questions de chaque exercice.
> Écrivez avec vos propres mots : une réponse courte et juste vaut mieux qu'un long copier-coller ! 🙂

---

## 🟢 Exercice 1 — Mon premier déploiement

1. Où se trouve physiquement le code qui fabrique votre page : sur votre ordinateur, sur GitHub ou sur PythonAnywhere ?

   > _Ma réponse : GITHUB

2. Pourquoi votre voisin(e) peut-il voir votre site, alors que vous n'avez rien installé sur son ordinateur ?

   > _Ma réponse : Parceque mon serveur est connecter a phyton anywhere version web

---

## 🟢 Exercice 2 — Les URL et les routes

1. Dans l'URL `https://www.google.com/maps`, quel est le nom de domaine ? Quel est le chemin ?

   > _Ma réponse :_ www.google.com et le chemin c'est maps

2. Que veut dire le message *Not Found* ? Qui l'a envoyé : votre navigateur ou le serveur ?

   > _Ma réponse :_ c'est le serveur qui l'envoie ca veut dire la page est introuvable 

3. Que se passe-t-il si deux fonctions portent le même nom dans `flask_app.py` ? (Indice : essayez, puis lisez l'Error log.)

   > _Ma réponse : Je constate que le site ne s'ouvre pas ca peut etre due ont faites que ont a definir 2 fonction avec un meme nom et du coup ca cause un troble dans la base de donne il sait pas qoui envoyer comme information du coup il envoie un erreur 404 ce qui veut dire il na pas ete trouver

---

## 🔵 Exercice 3 — Le langage HTML

1. Quelle est la différence entre ce que le serveur **envoie** et ce que le navigateur **affiche** ?

   > _Ma réponse : Ce que le serveur envoie : Du code textuel brut composé de texte et de balises HTML (que l'on peut voir en faisant un clic droit puis « Afficher le code source de la page »).

Ce que le navigateur affiche : Une page web graphique et mise en forme, obtenue après que le navigateur a interprété ces balises pour structurer les éléments visuellement.

2. À quoi servent les balises `<h1>`, `<p>`, `<ul>` et `<li>` ?

   > _Ma réponse :_
   >  <h1> : Définit un titre principal (de niveau 1).

<p> : Définit un paragraphe de texte.

<ul> : Définit une liste à puces non ordonnée (unordered list).

<li> : Définit un élément (item) à l'intérieur d'une liste.

3. Pourquoi l'image s'affiche-t-elle alors qu'elle n'est pas sur votre serveur ?

   > _Ma réponse :_ Parce que la balise <img> utilise un lien URL absolu (via l'attribut src) qui pointe vers un serveur externe sur Internet. Le navigateur va donc chercher, télécharger et afficher l'image directement depuis cette adresse distante.

---

## 🔵 Exercice 4 — Les templates

1. Pourquoi est-ce une bonne idée de séparer le code Python et le HTML ? (Pensez à une équipe avec un développeur et un graphiste.)

   > _Ma réponse :_ Cela permet une division claire des rôles c'est a dire le devellopeur faire sa partie et le graphiste faire sa partie pour que si il ya un modification a faire sa ne boulverse pas tout le code.

2. Les `{{ prenom }}` sont-ils remplacés par le serveur ou par le navigateur ? Comment l'avez-vous vérifié ?

   > _Ma réponse :_ Ils sont remplacer par le serveur evidement je l'ai verifier en faissent un clic droit sur la page et puis afficher le code source ou alors ctrl U

---

## 🔵 Exercice 5 — Le CSS et les liens

1. Quelle est la différence de rôle entre le HTML et le CSS ?

   > _Ma réponse :_ Le HTML sert à définir la structure et le contenu de la page (les titres, les paragraphes, les images, les liens).

Le CSS sert à définir la mise en forme et l'apparence visuelle (les couleurs, les polices d'écriture, les marges, l'agencement).

2. Pour afficher votre page `/presentation`, combien de fichiers le navigateur doit-il télécharger ? (Vous pourrez le vérifier à l'exercice suivant !)

   > _Ma réponse :_ Il doit télécharger au moins 2 fichiers : le fichier HTML de la page et le fichier de style CSS associé (pour appliquer la mise en page).

3. Pourquoi faut-il parfois faire **Ctrl + F5** pour voir les changements de CSS ?

   > _Ma réponse :_ Pour contourner le cache du navigateur. Pour aller plus vite puisque la commande Ctrl + F5 force le navigateur à ignorer ce cache et à télécharger la toute dernière version du fichier CSS depuis le serveur.

---

## 🟣 Exercice 6 — Espionner le navigateur

1. Que signifie HTTP ? Qui envoie la **requête** et qui envoie la **réponse** ?

   > _Ma réponse :_ HTTP signifie HyperText Transfer Protocol (Protocole de transfert hypertextuel).La requête est envoyée par le navigateur (le client), et la réponse est renvoyée par le serveur.

2. Combien de requêtes votre page `/presentation` a-t-elle déclenchées ? Lesquelles ?

   > _Ma réponse :_ Elle déclenche généralement au moins 2 requêtes : une pour charger la page principale (presentation) et une seconde automatique du navigateur pour chercher l'icône du site (favicon.ico).

3. Que signifie le code `200` ? Et le code `404` de la favicon ?

   > _Ma réponse :_ Le code 200 signifie que la requête a réussi avec succès.Le code 404 signifie que la ressource demandée est introuvable sur le serveur.

4. Pourquoi les modifications faites dans l'onglet Éléments ne sont-elles pas visibles par les autres visiteurs ?

   > _Ma réponse :_ Parce que ces modifications sont faites uniquement en local dans la mémoire de notre propre navigateur. Le fichier stocké sur le serveur reste inchangé, donc les autres visiteurs continuent de recevoir la version originale.

---

## 🟣 Exercice 7 — Envoyer des informations dans l'URL

1. Dans l'URL `https://www.youtube.com/results?search_query=chat`, quel est le nom du paramètre ? Quelle est sa valeur ?

   > _Ma réponse :_ Le nom du paramètre est search_query et la valeur est chat

2. Pourquoi le serveur plante-t-il avec `a=bonjour` ? Que faudrait-il faire pour l'éviter ?

   > _Ma réponse :_ 

3. Pourquoi est-il dangereux d'afficher **tel quel** ce que l'utilisateur envoie ?

   > _Ma réponse :_ C'est dangereux car un utilisateur malveillant peut injecter du code arbitraire Cela pourrait modifier l'apparence de la page, voler des données sensibles ou exécuter des scripts à l'insu des visiteurs.

---

## 🟣 Exercice 8 — Les formulaires

1. Quelle est la différence visible entre GET et POST ?

   > _Ma réponse :_ Avec la méthode GET, les données du formulaire s'affichent directement en clair dans l'URL (dans la barre d'adresse sous forme de paramètres. Avec la méthode POST, les données sont transportées discrètement dans le corps de la requête HTTP et n'apparaissent pas dans l'URL.

2. Pour un formulaire de **recherche**, quelle méthode choisiriez-vous ? Et pour un formulaire de **connexion avec mot de passe** ? Pourquoi ?

   > _Ma réponse :_ Pour un formulaire de recherche, on choisit GET, car cela permet de copier, partager ou mettre l'URL en favori avec les résultats de recherche. Pour un formulaire de connexion avec mot de passe, on choisit POST, car il ne faut jamais exposer un mot de passe dans l'URL (ce qui le laisserait visible dans l'historique du navigateur).

3. Les données envoyées en POST sont-elles vraiment « secrètes » ? (Pensez à ce que vous avez vu dans l'onglet Réseau.)

   > _Ma réponse :_ Je ne pense pas qu'ils sont secret donc je dirai non

---

## 🔴 Exercice 9 — Les codes de statut

1. Quelle est la différence entre une erreur `4xx` et une erreur `5xx` ? Qui est « fautif » dans chaque cas ?

   > _Ma réponse :_ 

2. Comment fonctionne une redirection ? Qui fait la deuxième requête : le serveur ou le navigateur ?

   > _Ma réponse :_ 

3. Donnez un exemple de situation où un vrai site utilise une redirection.

   > _Ma réponse :_ 

---

## 🔴 Exercice 10 — Ce que le serveur sait de vous

1. Citez trois informations que le serveur connaît sur vous, sans que vous ayez rien rempli.

   > _Ma réponse :_ 

2. À quoi peut servir l'en-tête `Accept-Language` pour un site comme Wikipédia ?

   > _Ma réponse :_ 

3. Dans l'Access log, retrouvez une requête qui a reçu un code `404`. Quelle page était demandée ?

   > _Ma réponse :_ 

4. Après cet exercice, que pensez-vous de la notion de « navigation anonyme » ?

   > _Ma réponse :_ 

---

## 🔴 Exercice 11 — Le Web des machines : API et JSON

1. Quelle est la différence entre une page HTML et une réponse JSON ? À qui chacune est-elle destinée ?

   > _Ma réponse :_ 

2. Dans la page `/horloge`, quel code s'exécute sur le **serveur** et quel code s'exécute dans le **navigateur** ?

   > _Ma réponse :_ 

3. Citez une application de votre téléphone qui, selon vous, utilise une API. Quelles données échange-t-elle ?

   > _Ma réponse :_ 

---

## 🏁 Pour conclure

En quelques phrases, expliquez à un ami ce qui se passe entre le moment où il tape une adresse dans son navigateur et celui où la page s'affiche :

> _Ma réponse :_ 
