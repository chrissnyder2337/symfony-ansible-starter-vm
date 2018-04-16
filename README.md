# SYMFONY ANSIBLE STARTER VM (TBD)

This is a anisble vm for local development with symfony 4. 

Review the variables in `./provisioning/vars/vars.yml` and `./Vagrantfile` and replace `site-name` with your project name.

## Local Installation (With Vagrant)

The following are basic local installation steps.

#### Prerequisites:

The following should be installed on your local machine.
 
 - PHP 7.2
 - Composer [Install Composer Globally](https://getcomposer.org/doc/00-intro.md#globally)
 - NodeJS >= 6.x 
 - Yarn [Install Yarn](https://yarnpkg.com/lang/en/docs/install/)
 - Vagrant [Download Vagrant](https://www.vagrantup.com/downloads.html)
 - Vagrant hostsupdater plugin (`vagrant plugin install vagrant-hostsupdater`)
 - Vagrant bindfs plugin (`vagrant plugin install vagrant-bindfs`)
 

#### Steps:

1. Install Dependencies:

    ``` 
    composer install
    ``` 

2. Install frontend assets:

    ``` 
    yarn install
    ``` 

3. Compile frontend assets:

    ``` 
    yarn run encore dev
    ```
    
4. Start the vagrant machine. You may be asked for your password.

    ```
    vagrant up
    ```
    or
    ``` 
    vagrant up --provision
    ```
    
5. Visit the site:

- Visit (http://site-name.test) in your browser.

    

    
## Troubleshooting


https://github.com/symfony/webpack-encore/issues/121