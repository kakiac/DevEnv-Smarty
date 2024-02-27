# DevEnv-Smarty

A GitHub Codespaces **Dev**eloper **Env**ironment as a service (DEaaS), replicating the environment that you were given at the Introduction to Web Development module.

## How it was created

1. a blank codespace was created from a blank repository. The following are installed by default:

a. PHP
b. Node.js (via nvm), yarn and pnpm

See the full list here: https://aka.ms/ghcs-default-image 

2. the following plugins were installed to the devcontainer.json via bottom left "Codespaces" button, then "Add Dev Container Configuration files" > "Modify your current configuration" then searching for the following packages and ensuring the boc on the left is ticked:

a. Composer (via Github Releases) - from devcontainers-contrib
b. Lighthouse CLI (via npm) - from devcontainers-contrib

I also tried installying this, but threw errors:

MySQL (via Homebrew)

3. Click on rebuild once it pops up. Your codespace will be recreated and install these packages. This will take some time, but you can click on the "View Log" link to view what is happening in the background.

4. Your codespace should restart.

5. Run `composer -v` to check that you are running composer and that it was successfully installed. You should be getting the composer logo and some usage commands.

6. If so, run the following command to install **Smarty**

`composer require smarty/smarty`

This should install Smarty. Smarty is a template engine for PHP, facilitating the separation of presentation (HTML/CSS) from application logic. You can find more information about it here: https://packagist.org/packages/smarty/smarty 

You should now see some additional files added (vendor folder, composer.json, composer.lock)

Commit and push your changes to the repository.
