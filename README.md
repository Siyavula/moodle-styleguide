# moodle-styleguide


## Moodle coding style

Moodle has some very specific styling that should be followed, check out the coding style guide at:

https://moodledev.io/general/development/policies/codingstyle


## Setting up your linter

The linter recommended for moodle development is PHP Codesniffer. PHP CodeSniffer is a tool used to analyse PHP code using a set of rules. In many cases these rules can be used to automatically fix the errors they identify.

The following are the steps to set up PHP Codesniffer:


  1. Start by installing composer, the steps are provided in the link below:

    https://www.digitalocean.com/community/tutorials/how-to-install-composer-on-ubuntu-20-04-quickstart
    
 
  2. Install composer dependencies:
   
    Type the following into your terminal:
  
      composer global require "squizlabs/php_codesniffer=*"
  
      composer global require moodlehq/moodle-cs
      
   
  3. If composer is still missing add it's path to your bashrc:

      export PATH="$PATH:$HOME/.config/composer/vendor/bin"
      

  4. Install PHP CodeSniffer in VS Code or your code editor:

      For VS Code:
      
        Open Visual Studio Code.
    
        Press Ctrl+P on Windows or Cmd+P on Mac to open the Quick Open dialog.
   
        Type ext install phpcs to find the extension.
    
        Press Enter or click the cloud icon to install it.

        Restart Visual Studio Code when prompted.
 
  
  5. Test that PHP CodeSniffer is working:
    
     Open any php file.

     Add a variable in camel case.
    
     Save changes and check that an error pops up for the incorrect case used.

