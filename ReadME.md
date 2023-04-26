### Entraînement avec React.js


# Tu es sur un fichier que j'ai initialisé avec la commande :

npm create vite@latest

# Si tu tentes la commande 

npm run dev

# Tu constateras qu'il n'y a rien d'affiché. C'est normal : J'ai nettoyé le fichier App.jsx, si bien qu'il n'y a rien d'autre qu'un <div> parente.

# Pour cet exercice, tu vas devoir créer un petit projet permettant d'afficher tous les Simpsons, et de les filtrer. Voici les étapes :

  # 0. Voici le lien vers le template, pour que tu aies une idée visuelle de ce qui devra être créé :

  https://www.figma.com/file/zod7tucuxealQKeYVOh0Bf/Untitled?node-id=0-1&t=wbqpwBqZPuKQ8Mra-0
 

  # 1. Le composant App doit importer deux composants pages :
##    ---> HomePage ;
##    ---> ContactPage;

  # 2. C'est le composant HomePage qui sera le propriétaire des données provenant de l'API. Ces données seront ensuite passer en props aux enfants.

  # 3. Télécharge la librairie axios, et rappelle-toi comme on "fetch" les données provenant de l'API. Dans notre cas, je t'invite à utiliser cet endpoint, qui te permettra de fetcher un tableau de simpsons (20 objets) :

##    ---> https://thesimpsonsquoteapi.glitch.me/quotes?count=num

  # 4. Stocke ces données dans un state.

  # 5. Un petit console.log te permettra de savoir si tu as bien récupéré les données ✅

  # 6. Ensuite, tu peux mapper le tableau de données dans le composant HomePage ! Et le return de cette méthode map devra appeler un composant Card ! Effectivement, ce composant n'existe pas encore. Tu vas simplement devoir le créer !

  # 7. Ce composant Card doit retourner les balises qui permettront d'afficher nos données. Console.log() à nouveau les données dans HomePage pour bien comprendre ce qu'il y a dedans, et voir quelles seront les balises adéquates 🚀 

