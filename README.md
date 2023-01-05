#### tailwind installation
## To setup tailwind css, run these commands

> must install Tailwind CSS IntelliSense in vscode

1. initial node

```
npm init -y
```
2. install dependencies

```
npm install -D tailwindcss postcss autoprefixer vite
```
3.  Install Tailwind CSS with auto postCSS configuration

```
npx tailwindcss init -p
```
4.  Create a css file "input.css", and below content in it

```
    @tailwind base;
    @tailwind components;
    @tailwind utilities;
```

5. add it to html file

6. In your tailwind.configjs file replace content: [ ], with content: ["*"],
```
/** @type {import('tailwindcss').Config} */
module.exports = {
  content: ["*"],
  theme: {
    extend: {},
  },
  plugins: [],
}
```

7.  Add "start": vite" to your scripts in package.json

```
  "scripts": {
    "start": "vite"
  }
```
8.  Run npm run start command to start a dev server
