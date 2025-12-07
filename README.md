# React Evil

Un quiz immersif axé sur la narration, développé avec React, TypeScript et Vite. React Evil allie une histoire captivante à un gameplay interactif, mettant les joueurs au défi d'explorer un monde rempli d'intrigues et de mystères.

🚀 **Caractéristiques principaless**

*   **Récit interactif dans un manoir hanté**: Progressez pièce après pièce dans un manoir mystérieux où chaque salle renferme une question de culture générale. Entre chaque épreuve, des passages narratifs immersifs dévoilent les secrets du manoir et renforcent la tension.
*   **Gestion stratégique de votre équipe**: Vous disposez de 4 personnages, chacun représentant une vie précieuse. À chaque mauvaise réponse, un membre de l’équipe disparaît. Préservez-les en jouant intelligemment et en utilisant vos ressources au bon moment.
*   **Progression en difficulté**: Faites face à 12 questions réparties en trois paliers : 4 faciles pour entrer dans le manoir, 4 moyennes pour s’enfoncer dans ses couloirs, 4 difficiles pour atteindre les zones les plus dangereuses.
Chaque question doit être résolue en 15 secondes, ajoutant une pression constante.
*   **Système de combos et jokers**: Enchaînez plusieurs bonnes réponses pour obtenir des jokers permettant de faciliter l’avancement dans les salles les plus périlleuses : temps supplémentaire, protection d’un personnage, ...
*   **Ambiance visuelle soignée**: Explorez un manoir hanté magnifiquement mis en scène, avec des environnements détaillés et une direction artistique immersive qui donne vie aux pièces traversées.
*   **Intégration audio atmosphérique**: Bénéficiez d’une bande-son inquiétante et d’effets sonores qui évoluent avec votre progression pour renforcer l’immersion dans ce lieu maudit.
*   **Suivi de progression et succès**: Débloquez des succès au fil de votre exploration : survie sans perte, partie parfaite, premier joker obtenu, ...
*   **Disponible sur mobile**: Profitez pleinement de l’expérience sur smartphone : interface optimisée, commandes fluides et immersion totale où que vous soyez.

🛠️ **Stack Technique**

| Catégorie    | Technologie                      | Description                                                                                                |
| :---------- | :------------------------------ | :--------------------------------------------------------------------------------------------------------- |
| Frontend    | React                           | Bibliothèque principale pour la création de l'interface utilisateur.                                                              |
|             | React Router                    | Assure le routage et la navigation au sein de l'application.                                                     |
|             | React DOM                       | Fournit des méthodes spécifiques au DOM pour React.                                                                   |
| Language    | TypeScript                      | Ajoute le typage statique à JavaScript, améliorant ainsi la qualité et la maintenabilité du code.                               |
| Build Tool  | Vite                            | Un outil de compilation rapide et un serveur de développement.                                                                    |
|             | @vitejs/plugin-react-swc       | Plugin Vite pour utiliser React avec SWC (Speedy Web Compiler).                                                 |
| Linting     | ESLint                          | Un linter JavaScript permettant d'identifier et de corriger les problèmes liés au style du code.                                          |
|             | @biomejs/biome                  | Un linter et un formateur pour la qualité du code.                                                                   |
| Git Hooks   | Husky                           | Gestionnaire de hooks Git pour exécuter des scripts avant les commits.                                                        |
| Environment | dotenv                          | Charge les variables d'environnement à partir d'un fichier `.env`.                                                            |
| Local Packages | beercontest, gg, lesperses    | Paquets locaux au sein du projet.                        |

📦 **Pour commencer**

##### Conditions préalables

*   Node.js (>=18)
*   npm or yarn or pnpm

##### Installation

1.  Cloner le dépôt :

    ```bash
    git clone <repository_url>
    cd reactevil
    ```

2.  Installer les dépendances :

    ```bash
    npm install # or yarn install or pnpm install
    ```

##### Exécution en local

1.  Démarrer le serveur de développement :

    ```bash
    npm run dev # or yarn dev or pnpm dev
    ```

    Cela lancera le serveur de développement Vite, et vous pourrez accéder à l'application dans votre navigateur à l'adresse fournie (généralement `http://localhost:5173`).

📂 **Structure du projet**

```
React Evil/
├── .husky/                 # Git hooks configuration
├── src/                    # Source code directory
│   ├── assets/             # Static assets (images, sounds, etc.)
│   ├── components/         # Reusable React components
│   │   ├── Endings.tsx     # Ending screen component
│   │   ├── Navbar.tsx      # Navigation bar component
│   │   ├── RainEffect.tsx  # Rain effect component
│   │   ├── Timer.tsx       # Timer component
│   │   ├── Notification.tsx # Notification component
│   │   ├── Success.tsx      # Success message component
│   ├── contexts/         # React context providers
│   │   ├── AudioContext.tsx    # Audio context
│   │   ├── CharacterContext.tsx# Character context
│   │   ├── SuccessContext.tsx  # Success context
│   ├── data/               # Game data (characters, rooms, narration)
│   │   ├── GameData.ts     # Static game data
│   │   ├── NarrationData.ts# Narration texts
│   ├── pages/              # Application pages
│   │   ├── Game.tsx        # Main game page
│   │   ├── Home.tsx        # Home page
│   ├── styles/             # CSS stylesheets
│   │   ├── App.css         # General styles
│   │   ├── game.css        # Game page styles
│   │   ├── Home.module.css # Home page styles (CSS modules)
│   │   ├── index.css       # Global styles
│   │   ├── mobile.css      # Mobile-specific styles
│   │   ├── navbar.css      # Navbar styles
│   ├── types/              # TypeScript type definitions
│   │   ├── GameDataTypes.ts# Types for game data
│   │   ├── GameTypes.ts    # Types for game logic
│   ├── App.tsx             # Root component
│   ├── main.tsx            # Entry point
│   ├── Router.tsx          # Router configuration
├── .env                    # Environment variables
├── .eslintignore           # ESLint ignore file
├── .eslintrc.cjs          # ESLint configuration
├── biome.json              # Biome configuration
├── commitlint.config.js    # Commitlint configuration
├── index.html              # HTML entry point
├── package.json            # Project metadata and dependencies
├── tsconfig.json           # TypeScript configuration
├── tsconfig.node.json      # TypeScript configuration for Node.js
├── vite.config.ts          # Vite configuration
```

📸 **Captures d'écran**

<img width="1470" height="796" alt="Capture d’écran 2025-12-07 à 13 14 39" src="https://github.com/user-attachments/assets/0b9dc48a-53ba-46dd-8e61-ca6867a7191a" />

<img width="1470" height="796" alt="Capture d’écran 2025-12-07 à 16 57 13" src="https://github.com/user-attachments/assets/df01a142-2792-4396-b655-794161a3693a" />

<img width="1470" height="796" alt="Capture d’écran 2025-12-07 à 16 57 30" src="https://github.com/user-attachments/assets/4ccae517-c106-4e16-a7b3-ebb6e63f034b" />

<img width="1470" height="795" alt="Capture d’écran 2025-12-07 à 16 58 27" src="https://github.com/user-attachments/assets/a20d0bc6-f74f-4a5d-8a2f-afe0e487920a" />

👥 **Équipe**

* Luna Soler : https://github.com/DevByEclipse
* Emeric Mouillat : https://github.com/Emericodes
* Jugurta Kadri : https://github.com/Jugurta-Kadri
* Lisa Bureau : https://github.com/Lisa-Bureau


📬 **Contact**

Si vous avez des questions ou des suggestions, n'hésitez pas à me contacter :

*   bureau.lisa03@gmail.com
  

💖 **Remerciements**

Merci d'avoir découvert React Evil ! Nous espérons que vous apprécierez le jeu et prendrez plaisir à l'explorer. Votre soutien et vos commentaires sont très appréciés !
