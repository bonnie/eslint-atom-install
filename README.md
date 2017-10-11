# Installing ESLint for Atom

## Things to do once, at the beginning

### In Atom Config

* Install the ESLint package in Atom

* Configure the ESLint package:

  * Set the ".eslintrc Path" to `~/.eslintrc`

  * Set the "Show Rule ID in Messages" checkbox to *on*

  * Set all other checkboxes to *off*

### On your laptop

* Create a .eslint file in your home directory (`~/.eslintrc`) with these contents:

```
{
   "extends": "airbnb",
}
```

## Things to do for every new project

* After npm init, add this to your package.json file:

```
  "devDependencies": {
    "ajv": "^5.2.2",
    "eslint": "^4.6.1",
    "eslint-config-airbnb": "^15.1.0",
    "eslint-plugin-import": "^2.7.0",
    "eslint-plugin-jsx-a11y": "^5.1.1",
    "eslint-plugin-react": "^7.3.0"
  }
```

* Run `npm install`

## To see if eslint is working

* Try to make eslint mad by following these steps:

  * open a new file
  * save it as with a .js extension, in a project that has eslint installed as described above
  * add a line that has double-quotes, like: `const blah = "blah"`
  * save the file again

* Do you get angry red squiggles, and info when you mouse over or click on the text with the squiggles? If so, congratulations, eslint is installed!
