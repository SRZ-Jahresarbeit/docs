## Tailwind CSS
Tailwind CSS is a CSS framework.
It requires **Node.js 12.13.0 or higher.**
<br>
The documentation can be found here:
```
https://tailwindcss.com/docs
```
We are using Tailwind without PostCSS.
<br>
With this command you can install the **tailwind.css** file:
```
npx tailwindcss-cli@latest build -o src/tailwind.css
```
With the command 
```
npx tailwindcss-cli@latest build src/styles.css -o src/tailwind.css
```
the changes are automatically transferred from the styles.css file to the tailwind.css file.
<br>
This is useful if you want to have another stylesheet in addition to the Tailwind CSS file
