1. project init
npm int -y

2. install postCSS
npm i -D postcss postcss-cli

3. create folder: src > input.css, dist > index.html

4. create script
"watch:css": "postcss src/input.css -o dist/style.css -w",
"build:css": "postcss src/input.css -o dist/style.css"

5. add prefixer
npm i -D autoprefixer

6. create postcss.config.js