⚡ React + TypeScript + Vite Starter
Ce projet est un template minimal pour démarrer rapidement une application React avec TypeScript et Vite, incluant une configuration de base d'ESLint et de Hot Module Replacement (HMR).

🧰 Technologies utilisées
⚛️ React

⚡ Vite

🟦 TypeScript

📏 ESLint

🔁 Fast Refresh via @vitejs/plugin-react

🚀 Démarrage rapide
bash
Copier
Modifier
# 1. Cloner le dépôt
git clone https://github.com/votre-utilisateur/nom-du-projet.git
cd nom-du-projet

# 2. Installer les dépendances
npm install

# 3. Démarrer le serveur de développement
npm run dev
Accédez ensuite à http://localhost:5173 pour voir l'application.

📦 Scripts disponibles
Script	Description
npm run dev	Démarre le serveur de développement
npm run build	Build de production optimisé
npm run preview	Lance un serveur local pour prévisualiser le build
npm run lint	Analyse le code avec ESLint

📐 Configuration ESLint recommandée
Pour activer des règles de lint plus poussées et basées sur les types TypeScript :

Modifiez le parserOptions comme suit :

js
Copier
Modifier
parserOptions: {
  project: ['./tsconfig.node.json', './tsconfig.app.json'],
  tsconfigRootDir: import.meta.dirname,
}
Utilisez une configuration avec typage strict :

js
Copier
Modifier
tseslint.configs.recommendedTypeChecked
// ou
tseslint.configs.strictTypeChecked
Ajoutez les plugins React (ex : eslint-plugin-react) :

js
Copier
Modifier
// eslint.config.js
import react from 'eslint-plugin-react'

export default tseslint.config({
  settings: {
    react: { version: '18.3' }, // ou détectée automatiquement
  },
  plugins: { react },
  rules: {
    ...react.configs.recommended.rules,
  },
})


## 📸 Aperçu du projet
![Aperçu du projet](https://github.com/Trikisalem/interview-training-ai/raw/main/a.png)


