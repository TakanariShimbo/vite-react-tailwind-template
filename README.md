## 🚀 About

My template of Vite x React x Tailwind

## 📝 Memo

- require: volta

### 1 upgrade node & npm

```sh
volta install node@latest
volta install npm@latest
```

### 2 scaffold for project

```sh
npm create vite@latest vite-react-tailwind-template -- --template react
```

### 3 remove eslint

- .eslintrc.cjs (remove file)
- package.json (remove a few row)

### 4 install modules

```sh
npm install
```

### 5 add tailwind

```sh
npm install -D tailwindcss postcss autoprefixer
npx tailwindcss init -p
```

- src/index.css (replace to the Tailwind directives)
- tailwind.config.js (add contents)
- src/App.jsx (replace to check tailwind installation)
- src/asserts (remove dir)
- src/App.css (remove file)

### 6 check

- check on vite server

```sh
npm run build
npm run preview
```

You can heck here (http://localhost:4173/) after building server.

- check on static server

```sh
npm run build
cd dist
python -m http.server
```

You can heck here (http://localhost:8000/) after building server.
