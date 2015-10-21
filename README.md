# sublime-react-configuration
##Step by step installation
1. Define user settings
  
  - Copy the content of Preferences => Settings - Default into Preferences => Settings - User.
  - Remove font face.
  - set "font_size": 13.
  - set "tab_size": 2.
  - set "translate_tabs_to_spaces": false.
  

2. [Install Package Control](https://packagecontrol.io/installation)
  
  - Copy the code in the link.
  - Open the sublime console, View => Show Console.
  - Paste the code and run the script
  - Restart Sublime
  
3. [Install Emmet](http://emmet.io/)

  - ctrl + shift + p => Install package => Emmet.
  - Restart Sublime
  
4. [Install Package Resource Viewer](https://github.com/skuroda/PackageResourceViewer)

  - ctrl + shift + p => Install package => Package Resource Viewer.
  
5. [Install ColorPicker](https://github.com/weslly/ColorPicker)

  - ctrl + shift + p => Install package => ColorPicker.

6. [Install HTML5 Snippet](https://packagecontrol.io/packages/HTML5)

  - ctrl + shift + p => Install package => HTML5.
  
7. [Install JavaScript & NodeJS Snippets](https://packagecontrol.io/packages/JavaScript%20%26%20NodeJS%20Snippets)

  - ctrl + shift + p => Install package => JavaScript & NodeJS Snippets.

8. [Install Babel plugin](https://packagecontrol.io/packages/Babel)
  
  - ctrl + shift + p => Install package => Babel.
  - Open a .js file.
  - View => Syntax => Open all with the current extension as... => Babel => Javascript(Babel)
  - Open a .jsx file.
  - View => Syntax => Open all with the current extension as... => Babel => Javascript(Babel)
  
9. [Install Babel Snippets](https://packagecontrol.io/packages/Babel%20Snippets)

  - ctrl + shift + p => Install package => Babel Snippets.
  
10. [Install ESLint](http://eslint.org/)
  
  - Open the Terminal and run:
  
    ```
    $ npm install -g eslint
    ```

11. [Instal SublimeLinter](http://www.sublimelinter.com/en/latest/installation.html)

  - ctrl + shift + p => Install package => SublimeLinter.
  - ctrl + shift + p => Install package => SublimeLinter-eslint.
  
12. [Configure the linting](http://eslint.org/docs/user-guide/getting-started)

  - Create a .eslintrc in the project folder.<br/>*ESLint will search upwards from the directory of the file being linted all the way to drive’s root directory.*
  - Add the rules that you want to the file, below there is an example, you can check [the documentation](http://eslint.org/docs/rules/)
  
  ```Javascript
  {
    "ecmaFeatures": {
      "modules": true,
      "jsx": true
    },
  
    "env": {
      "es6": true,
      "browser": true,
      "node": true,   
      "jquery": true
    },
  
    "rules": {
      
      "no-extra-semi": 2,           // disallow unnecessary semicolons
      "no-func-assign": 2,          // disallow overwriting functions written as function declarations
      "no-irregular-whitespace": 1, // disallow irregular whitespace outside of strings and comments
      "no-sparse-arrays": 1,        // disallow sparse arrays
      "no-unreachable": 2,          // disallow unreachable statements after a return, throw, continue, or break statement
      "use-isnan": 2,               // disallow comparisons with the value NaN
      "valid-typeof": 2,            // Ensure that the results of typeof are compared against a valid string
  
  
      ////////// Best Practices //////////
  
      "eqeqeq": 2,                // require the use of === and !==
      "no-alert": 1,              // disallow the use of alert, confirm, and prompt
      
      ////////// Variables //////////
  
      "no-delete-var": 1,               // disallow deletion of variables
      "no-undef": 2,                    // disallow use of undeclared variables unless mentioned in a /*global */ block
      "no-undef-init": 1,               // disallow use of undefined when initializing variables
      "no-unused-vars": 1,              // disallow declaration of variables that are not used in the code
      "no-use-before-define": 2,        // disallow use of variables before they are defined
  
      ////////// Stylistic Issues //////////
  
      "camelcase": 1,                 // require camel case names
      "comma-spacing": 1,             // enforce spacing before and after comma
      "eol-last": 2,                  // enforce newline at the end of file, with no multiple empty lines
      "new-cap": 2,                   // require a capital letter for constructors
      "no-array-constructor": 1,      // disallow use of the Array constructor
      "no-mixed-spaces-and-tabs": 1,  // disallow mixed spaces and tabs for indentation
      "no-multiple-empty-lines": 1,   // disallow multiple empty lines (off by default)
      "no-trailing-spaces": 2,        // disallow trailing whitespace at the end of lines
      "semi": 2,                      // require or disallow use of semicolons instead of ASI
      "space-after-keywords": 1,      // require a space after certain keywords (off by default)
      "space-infix-ops": 1,           // require spaces around operators
      
  
      ////////// ECMAScript 6 //////////
  
      "no-var": 2,          // require let or const instead of var (off by default) 
  
    }
  }
