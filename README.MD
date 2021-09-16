


Node env with modern JS

npm init

npm install --save-dev @babel/cli @babel/core @babel/preset-env
touch .babelrc
{
  "presets": ["@babel/preset-env"]
}
touch index.js and move it to src

"build": "babel index.js -d dist"
"start": "npm run build && node dist/index.js" -- strike
"start": "npm run build && nodemon dist/index.js"
"serve": "node dist/index.js" -- production 
"build": "babel src -d dist",
"serve": "node dist/index.js"