# directorio-talento


Administración de directorio de talento


# abort on errors
#!/usr/bin/env sh
set -e
npm run docs:build
cd docs/.vuepress/dist
git init
git add -A
git commit -m 'deploy'
git push -f https://github.com/hmvsoluciones/directorio-talento.git master:gh-pages
cd -