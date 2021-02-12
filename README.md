# directorio-talento


Administración de directorio de talento
# Config JS

```javascript
  module.exports = {
  /**
   * Ref：https://v1.vuepress.vuejs.org/config/#title
   */
  title: 'Portal de Procesos Demo',
  /**
   * Configuration GH-PAGE
   */
  base: "/directorio-talento/",
  ..
  }
```

# abort on errors
```sh
set -e
npm run docs:build
cd docs/.vuepress/dist
git init
git add -A
git commit -m "deploy"
git push -f https://github.com/hmvsoluciones/directorio-talento.git master:gh-pages
cd -
```