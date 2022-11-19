1. project init
npm int -y

2. install postCSS
npm i -D postcss postcss-cli

2.1. install PostCSS Language Support
VS json >

  "emmet.includeLanguages": {
    "postcss": "css"
  }

3. create folder: src > input.css, dist > index.html

4. create script
"watch:css": "postcss src/input.css -o dist/style.css -w",
"build:css": "postcss src/input.css -o dist/style.css"

5. add prefixer
npm i -D autoprefixer

6. create postcss.config.js
module.exports = {
  plugins: [require('autoprefixer')],
};

7. add postcss preset-env
npm i -D postcss-preset-env

require('postcss-preset-env')({
      stage: 1,})

8. add preCSS (=SASS syntax)
npm i -D precss

9. add postcss IMPORT
npm i -D postcss-import

10. add postcss ASSETS
npm i -D postcss-assets

    require('postcss-assets')({
        loadPaths: ['dist/img'],
    }),

  11. add CSSNANO
  npm i -D cssnano

    require('cssnano')({
        preset: 'default'
    }),
