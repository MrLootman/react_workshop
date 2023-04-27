### Entraînement avec React.js


## __Préambule__ :
#### Te voilà prêt à démarrer. Si tu tentes la commande :

npm run dev

#### Tu constateras qu'il n'y a rien d'affiché. C'est normal : J'ai nettoyé le fichier App.jsx, et j'ai supprimé les fichiers .css. En résumé : il n'y a rien d'autre qu'une <div> parente.

#### Pour cet exercice, tu vas devoir créer un petit projet permettant d'afficher tous les Simpsons, et de les filtrer. Voici les étapes :

  ## 0. Voici le lien vers le template, pour que tu aies une idée visuelle de ce qui devra être créé :

  https://www.figma.com/file/zod7tucuxealQKeYVOh0Bf/Untitled?node-id=0-1&t=wbqpwBqZPuKQ8Mra-0
 
  #### Tu peux commencer à créer ton architecture (l'organisation des fichiers), et le CSS qui sera associé à chaque composant. Je t'invite à installer SCSS dans ton projet :

  *npm install sass*

  ## 1. Petite aide pour composer l'architecture : Le composant App doit importer les composants suivants :
##    ---> Header;
##    ---> HomePage;
##    ---> ContactPage;
##    ---> Footer;

  ##  `*1.bis : __Rappel :__ C'est le composant HomePage qui sera le propriétaire des données provenant de l'API.`
  ## `*1.ter : __A ce stade...__ Tu devras créer le header et le footer par toi-même, conformément à la maquette.` 

  ## 2. Dans le composant page, tu vas désormais fetcher ce qui vient de l'API (je te donne le lien dans quelques instants). Pour cela, tu as deux solutions :
    💡 Télécharger la librairie __axios__ (npm install axios);
    💡 Utiliser la méthode fetch, qui est nativement présente en JavaScript.
  ### Si ta mémoire te fait défaut, ou si tu veux explorer, je t'invite à lire la documentation d'une des deux méthodes. Tu peux aussi remettre le nez dans les quêtes pour voir comment faire 😊

  ##  `*2.bis : __Le endpoint__ de l'API sera le suivant ; c'est cette adresse qu'il faudra interroger pour récupérer les données :`
##    ---> https://thesimpsonsquoteapi.glitch.me/quotes?count=20

  ### Tu es bloqué ? 🧐 Revisite tes quêtes, ou regarde comment on fetch des données en React.js.

  ## 3. Stocke ces données dans un state (ou variable d'état) nommé data.
  ###   `* 4.bis : A l'initialisation, la valeur du state doit être un tableau vide.`
  ###   `*4.ter : Un petit console.log te permettra de savoir si tu as bien récupéré les données ✅`

  ## 4. 🔍️ Désormais, il est temps de faire fonctionner ta mémoire, et de faire tes propres recherches. Ton objectif est de mapper le tableau de Simpsons, pour retourner une carte par personnage. Il est volontaire de ma part de ne pas te guider davantage, pour que ta réussite soit le résultat de tes recherches et de ta curiosité 😊

  ## 5. ... Après cette longue phase de travail, tu devrais avoir : ce stade, tu devrais avoir une liste de cartes