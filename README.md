# DevEnv-Smarty

A GitHub Codespaces **Dev**eloper **Env**ironment as a service (DEaaS), replicating the environment that you were given at the Introduction to Web Development module.

## How it was created

1. a blank codespace was created from a blank repository. The following are installed by default:

a. PHP
b. Node.js (via nvm), yarn and pnpm

2. the following plugins were installed to the devcontainer.json via bottom left "Codespaces" button, then "Add Dev Container Configuration files" > "Modify your current configuration" then searching for the following packages and ensuring the boc on the left is ticked:

a. Composer (via Github Releases) - from devcontainers-contrib
b. Lighthouse CLI (via npm) - from devcontainers-contrib

I also tried installying this, but threw errors:

MySQL (via Homebrew)
