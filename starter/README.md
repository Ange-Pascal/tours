## Figma URL

[Tours](https://www.figma.com/file/OnLoM3AzBFaHzSc2iolJS0/Tours?node-id=0%3A1&t=wiRXOlTLN5ehekYI-1)

## Steps

#### Setup
#### Configuration

Créez d'abord les trois composants (Tours, Tour et Loading), vous pouvez créer trois fichiers distincts dans votre répertoire de projet : Tours.jsx, Tour.jsx et Loading.jsx. Dans chacun de ces fichiers, vous définirez un composant fonctionnel React qui renvoie du code JSX pour le rendu du composant correspondant.

#### Récupérer les tournées

Le composant Tours sera responsable du rendu d'une liste de composants de tournées. Dans App.jsx, vous récupérerez les données des circuits à partir d'une URL à l'aide de l'API fetch. Avant que les données ne soient chargées, vous devez afficher un spinner ou un message de chargement, qui peut être mis en œuvre à l'aide du composant Loading.

#### Render Tours

Once the data is loaded, you can set the state of your component to store the tours data. You can then map over the tours array and render a Tour component for each tour. Each Tour component will receive the tour data as props, including the tour's id, image, info, name, and price.

#### Remove Tour

To implement the "remove tour" functionality, you can add a button to each Tour component that, when clicked, removes the tour from the list of tours. You can achieve this by updating the state of the Tours component to remove the tour from the tours array.

#### Read More

To implement the "read more" functionality, you can add a button to each Tour component that, when clicked, expands the description of the tour. You can achieve this by updating the state of the Tour component to toggle a "read more" flag, and conditionally rendering the full description based on the flag.

#### Re-fetch Tours

Finally, you can implement a "re-fetch" functionality by adding a button or other user interface element that, when clicked, re-fetches the tours data from the URL and updates the state of the Tours component. You may also want to add a loading state again during the re-fetching process.

Overall, the flow of the application should look something like this:

- App.jsx fetches tours data from a URL and sets the state of the Tours component to store the data.
- The Tours component maps over the tours array and renders a Tour component for each tour.
- Each Tour component has a "remove tour" button and a "read more" button.When the "remove tour" button is clicked, the Tours component updates its state to remove the tour from the tours array.

- When the "read more" button is clicked, the Tour component updates its state to toggle a "read more" flag and conditionally renders the full description.

- When the "re-fetch" button is clicked, the Tours component re-fetches the tours data from the URL and updates its state.
