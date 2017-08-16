# CakePHP Issue #11048

Steps to reproduce locally....

    #!/bin/bash
    git clone git@github.com:CakePHPKitchen/CakePHP-Issue-11048.git
    cd CakePHP-Issue-11048
    composer install
    mysql -u root < config/schema/basics.sql
    bin/cake migrations migrate
    mysql -u root issue11048 < config/schema/issue11048.sql
    bin/cake server -p 9001

Then navigate to 

    http://localhost:9001/issue11048
    
