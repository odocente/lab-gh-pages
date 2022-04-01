```bash
git init
git remote add origin git@github.com:odocente/lab-gh-pages.git
npm install

git add .
git commit -m "initial commit"
git push -u origin main

npm run build
```

- Creamos rama `gh-pages`:

	```bash
	git branch gh-pages
	git checkout gh-pages
	```

	

- Eliminamos tódolos ficheiros agás a pasta `dist` . Movemos o contido de `dist` ao directorio `root` que debe ficar co seguinte contido:  

```
|- images
|- js
|- index.html
```

- Subimos modificacións:

```bash
git add .
git commit -m "upload files"
git push -u origin gh-pages
```

- Comprobamos o resultado: 
	- https://github.com/odocente/lab-gh-pages
	- https://odocente.github.io/lab-gh-pages/
