### Entraînement avec React.js


## __Préambule__ :
#### Te voilà prêt à démarrer. Si tu tentes la commande :

npm run dev

#### Tu constateras qu'il n'y a rien d'affiché. C'est normal : J'ai nettoyé le fichier App.jsx, et j'ai supprimé les fichiers .css. En résumé : il n'y a rien d'autre qu'une <div> parente.

#### Pour cet exercice, tu vas devoir créer un petit projet permettant d'afficher tous les Simpsons, et de les filtrer. Voici les étapes :

  ## 0. Voici le lien vers le template, pour que tu aies une idée visuelle de ce qui devra être créé :

  https://www.figma.com/file/zod7tucuxealQKeYVOh0Bf/Untitled?node-id=0-1&t=wbqpwBqZPuKQ8Mra-0
 
  #### Tu peux commencer à créer ton architecture (l'organisation des fichiers), et le CSS qui sera associé à chaque composant. Je t'invite à installer et utiliser SCSS dans ton projet :

  *npm install sass*

  #### Il te faudra donc créer un dossier style dans le dossier src/, lequel contiendra toutes les fiches de styles que tu créeras.

  ## 1. Petite aide pour composer l'architecture : Le composant App doit importer les composants suivants :
##    ---> Header;
##    ---> HomePage;
##    ---> ContactPage;
##    ---> Footer;

  ##  `*1.bis : __Rappel :__ C'est le composant HomePage qui sera le propriétaire des données provenant de l'API.`
  ## `*1.ter : __A ce stade...__ Tu devras créer le header et le footer par toi-même, conformément à la maquette.` 

  ## 2. Dans le composant HomePage, tu vas désormais fetcher ce qui vient de l'API (je te donne le lien dans quelques instants). Pour cela, tu as deux solutions :
    💡 Télécharger la librairie __axios__ (npm install axios);
    💡 Utiliser la méthode fetch, qui est nativement présente en JavaScript.
  ### Si ta mémoire te fait défaut, ou si tu veux explorer, je t'invite à lire la documentation d'une des deux méthodes. Tu peux aussi remettre le nez dans les quêtes pour voir comment faire 😊

  ##  `*2.bis : __Le endpoint__ de l'API sera le suivant ; c'est cette adresse qu'il faudra interroger pour récupérer les données :`
##    ---> https://thesimpsonsquoteapi.glitch.me/quotes?count=20
  ## `* Comme tu peux le constater, on interroge le endpoint /quotes, et on ajoute une query permettant de fetcher 20 informations.`

  ### Tu es bloqué ? 🧐 Revisite tes quêtes, ou regarde comment on fetch des données en React.js.

  ## 3. Stocke ces données dans un state (ou variable d'état) nommé data.
  ###   `* 3.bis : A l'initialisation, la valeur du state doit être un tableau vide.`
  ###   `*3.ter : Un petit console.log te permettra de savoir si tu as bien récupéré les données ✅`

  ## 4. 🔍️ Désormais, il est temps de faire fonctionner ta mémoire 🧠, et de faire tes propres recherches. Ton objectif est de mapper le tableau de Simpsons, pour retourner une carte par personnage. Il est volontaire de ma part de ne pas te guider davantage, pour que ta réussite soit le résultat de tes recherches et de ta curiosité 😊
  ###   `*4.bis : Un petit indice tout de même : tu dois créer un composant Card.`

  ## 5. ... Après cette longue phase de travail, tu devrais avoir une liste de cartes, au nombre de 20. Applique le style qu'il faut pour pour être au plus proche de la maquette.

  ## 6. Il est l'heure d'ajouter de l'intéractivité à ta page. Si tu ne l'as pas fait, tu peux créer un input (cf. maquette). Cet input doit filtrer les informations présentes à l'écran.
  ### `* 6.bis : Un exemple de User Story :`
  #### `[US-??] En tant qu'utilisateur, je veux pouvoir filtrer dynamiquement les cartes affichées dans la HomePage`
  #### `[US-??bis] En tant qu'utilisateur, mon filtre doit tolérer les lettres en minuscule (ex: J'écris "homer" dans l'input, les cartes avec Homer doivent apparaître)`

  ## 7. Rendus à la septième étape, il est temps de te concentrer sur la création du formulaire. Regarde la maquette, et construit la page conformément à celle-ci.
  ### `* 7.bis : Ton formulaire n'envoie rien pour le moment, et c'est normal. Ce qu'on souhaite, c'est que les éléments soient physiquement présents sur l'image`

  ## 8. Il est temps d'installer la dépendance suivante :
  `*    ---> npm install react-router-dom`
  ### Tu l'as compris : Il faut donner à l'utilisateur la possibilité de changer de page. Je te laisse replonger dans ce que tu as appris dans les quêtes concernant la navigation en React.js, et ses spécificités.

  ## 9. Nouvelle étape, nouveau palier difficulté : Les cartes doivent être cliquables, et renvoyer vers une page par id.
  ### `* 9.bis : Tu te rappelles de useParams ?`