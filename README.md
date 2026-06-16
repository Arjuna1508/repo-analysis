  # React + TypeScript + Vite
  
  # Harshith - Repository Analysis
  
  This template provides a minimal setup to get React working in Vite with HMR and some ESLint rules.
  
  Currently, two official plugins are available:
  
  - [@vitejs/plugin-react](https://github.com/vitejs/vite-plugin-react/blob/main/packages/plugin-react) uses [Oxc](https://oxc.rs)
  - [@vitejs/plugin-react-swc](https://github.com/vitejs/vite-plugin-react/blob/main/packages/plugin-react-swc) uses [SWC](https://swc.rs/)
  
  ## React Compiler
  
  The React Compiler is enabled on this template. See [this documentation](https://react.dev/learn/react-compiler) for more information.
  
  Note: This will impact Vite dev & build performances.
  
  ## Expanding the ESLint configuration
  
  If you are developing a production application, we recommend updating the configuration to enable type-aware lint rules:
  
  ```js
  export default defineConfig([
    globalIgnores(['dist']),
    {
      files: ['**/*.{ts,tsx}'],
      extends: [
        // Other configs...
  
        // Remove tseslint.configs.recommended and replace with this
        tseslint.configs.recommendedTypeChecked,
        // Alternatively, use this for stricter rules
        tseslint.configs.strictTypeChecked,
        // Optionally, add this for stylistic rules
        tseslint.configs.stylisticTypeChecked,
  
        // Other configs...
      ],
      languageOptions: {
        parserOptions: {
          project: ['./tsconfig.node.json', './tsconfig.app.json'],
          tsconfigRootDir: import.meta.dirname,
        },
        // other options...
      },
    },
  ])
  ```
  
  You can also install [eslint-plugin-react-x](https://github.com/Rel1cx/eslint-react/tree/main/packages/plugins/eslint-plugin-react-x) and [eslint-plugin-react-dom](https://github.com/Rel1cx/eslint-react/tree/main/packages/plugins/eslint-plugin-react-dom) for React-specific lint rules:
  
  ```js
  // eslint.config.js
  import reactX from 'eslint-plugin-react-x'
  import reactDom from 'eslint-plugin-react-dom'
  
  export default defineConfig([
    globalIgnores(['dist']),
    {
      files: ['**/*.{ts,tsx}'],
      extends: [
        // Other configs...
        // Enable lint rules for React
        reactX.configs['recommended-typescript'],
        // Enable lint rules for React DOM
        reactDom.configs.recommended,
      ],
      languageOptions: {
        parserOptions: {
          project: ['./tsconfig.node.json', './tsconfig.app.json'],
          tsconfigRootDir: import.meta.dirname,
        },
        // other options...
      },
    },
  ])
  ```
  ## Student Details
  
  **Name:** Mayank Kothari
  
  **Roll Number:** 251EE235
  
  ## Repository Analysis
  
  ### Framework Versions
  
  The versions were identified from the `package.json` file:
  
  - React: 19.2.0
  - React DOM: 19.2.0
  - TypeScript: 5.6.2
  - Vite: 8.0.12
  - ESLint: 10.0.1
  
  ### Workflow Analysis
  
  The workflow file is present in:
  
  `.github/workflows`
  
 The workflow is triggered on pushes and pull requests to the main branch.

 The workflow performs automated checks such as linting, testing and build validation before changes are merged.
  ### Changes Made
  
  Added student details and repository analysis as part of the DEV SMP Task 4 submission.
  ## Git Commands Used
  
  ```bash
  git clone https://github.com/Arjuna1508/repo-analysis.git
  cd repo-analysis
  git checkout -b Mayank_25IEE235
  git add README.md
  git commit -m "Added repository analysis to README"
  git push origin Mayank_25IEE235
