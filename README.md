# moodle-styleguide


## Moodle coding style

Moodle has some very specific styling that should be followed, check out the coding style guide at:

  [www.moodledev.io](https://moodledev.io/general/development/policies/codingstyle)


## Setting up your linter


The linter recommended for moodle development is PHP Codesniffer. PHP Sniffer is a tool used to analyse PHP code using a set of rules. In many cases these rules can be used to automatically fix the errors they identify.


### The following are the steps to set up PHP Codesniffer:


  1. Start by installing composer, the steps are provided in the link below:

     [www.digitalocean.com](https://www.digitalocean.com/community/tutorials/how-to-install-composer-on-ubuntu-20-04-quickstart)
    
 
  2. Install composer dependencies:
 
      ```shell   
      composer global require "squizlabs/php_codesniffer=*"
  
      composer global require moodlehq/moodle-cs
      ```  
   
  3. Add composer's path to your bashrc:

      ```shell
      export PATH="$PATH:$HOME/.config/composer/vendor/bin"
      ```
      

  4. Install PHP Sniffer in VS Code:
 
        
      - Press Ctrl+P on Linux/Windows or Cmd+P on Mac to open the Quick Open dialog.
      
      - Type ext install phpcs to find the extension.
    
      - Press Enter or click the cloud icon to install it.

      - Restart Visual Studio Code when prompted.
 
  
  5. Test that PHP Sniffer is working:
  
    
     - Open any php file.

     - Add a variable in camel case.
    
     - Save changes and check that an error pops up for the incorrect case used.

