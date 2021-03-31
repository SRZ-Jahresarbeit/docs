## Tailwind CSS
Tailwind CSS is a utility-first CSS framework.
It requires **Node.js 12.13.0 or higher.**
<br>
The documentation can be found here:
```
https://tailwindcss.com/docs
```
We are using Tailwind 2.0.4 as a PostCSS Plugin.
<br>
We install Tailwindcss, PostCSS and autoprefixer with this command:
```
npm install -D tailwindcss@latest postcss@latest autoprefixer@latest
```

With this command we installed and built the **tailwind.css** file:
```
npx tailwindcss-cli@latest build -o src/tailwind.css
```

With the command 
```
npx tailwindcss-cli@latest build src/styles.css -o src/tailwind.css
```
the changes are automatically transferred from the styles.css file to the tailwind.css file.
<br>
This is useful if you want to have another stylesheet in addition to the Tailwind CSS file.
<br>
The changes in the files **postcss.config.js** and **tailwind.config.js** are also adopted in Tailwind when this command is executed
<br>
This is not done before!
