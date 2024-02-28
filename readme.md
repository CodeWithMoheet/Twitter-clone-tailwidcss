Tailwind CSS

1.	npm init -y
2.	npm install -D tailwindcss postcss autoprefixer vite
3.	npx tailwindcss init –p
4.	In package.json file add 
 "scripts": {
    "start": "vite"
  },
5.	In (Tailwind.config.js)add [*] beside content as shown
/** @type {import('tailwindcss').Config} */
module.exports = {
  content: ["*"],
  theme: {
    extend: {},
  },
  plugins: [],
}
6.	For generating css file automatically in tailwind file called (“Output.css”) we use 
"scripts": {
    "start": "vite",
    "build": "npx tailwindcss -i ./src/input.css -o ./src/output.css --watch"
      },
7.	In build put the file path of css file
8.	npm run start
 

