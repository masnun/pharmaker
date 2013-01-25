# PHAR MAKER 

### Simple PHAR build tool to convert a directory into a PHAR archive 

#### Basic Concepts
__Source Directory:__ The directory that contains the source php files. <br/>
__PHAR Name:__ The name which identifies the Phar. The name is used to generate the phar archive as well as to refer to the archive in phar:// steam contexts. <br/>
__CLI Script:__ The script which is executed when the archive is run from the command line. index.php is assumed if not provided. <br/>
__Web Script:__ The script which is by default executed in the web environment. Defaults to CLI script value if not provided with.

#### Building Basics

    ./makephar <source dir> <phar name> [<cli script> <web script>]
    
Example: The following command will create a phar archive named mphar.phar with cli.php as cli script and web.php as the web script
   
    ./makephar src mphar.phar cli.php web.php

    ==========: STARTING PHAR BUILD PROCESS :==========
    Source Directory: src
    PHAR Name: mphar.phar
    CLI Script: cli.php
    Web Script: web.php
    DONE: Built mphar.phar

__Checkout the "src" directory for sample cli and web script__