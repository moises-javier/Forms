# Forms Clone

_In development_

## Running the project in local

### 🛠️ Installation

### Backend

1. Create and activate virtual environment

   _Windows:_

   ```sh
   py -3 -m venv venv
   venv\Scripts\activate
   ```

   _macOs/Linux:_

   ```sh
   python3 -m venv venv
   . venv/bin/activate
   ```

2. Install dependencies
   ```
   pip install -r requirements.txt
   ```
3. Create an **.env** file and add the credentials
   ```
   MYSQL_HOST = localhost
   MYSQL_USER = user_here
   MYSQL_DATABASE = quick_forms
   MYSQL_PASSWORD = password_here
   MYSQL_PORT = 3306
   ```
4. Create tables into database *(you need to previously create the database)*:
   ```
   python create_tables.py
   ```
5. To run the application:
   ```
	flask --app app --debug run
   ```

### Frontend

This template should help get you started developing with Vue 3 in Vite.

## Recommended IDE Setup

[VSCode](https://code.visualstudio.com/) + [Volar](https://marketplace.visualstudio.com/items?itemName=Vue.volar) (and disable Vetur)

## Customize configuration

See [Vite Configuration Reference](https://vitejs.dev/config/).

## Project Setup

```sh
npm install
```

### Compile and Hot-Reload for Development

```sh
npm run dev
```

### Compile and Minify for Production

```sh
npm run build
```

### Run Unit Tests with [Vitest](https://vitest.dev/)

```sh
npm run test:unit
```

### Run End-to-End Tests with [Cypress](https://www.cypress.io/)

```sh
npm run test:e2e:dev
```

This runs the end-to-end tests against the Vite development server.
It is much faster than the production build.

But it's still recommended to test the production build with `test:e2e` before deploying (e.g. in CI environments):

```sh
npm run build
npm run test:e2e
```

### Lint with [ESLint](https://eslint.org/)

```sh
npm run lint
```
