# Gitbook Template

> A Gitbook seed project

## What is this ?

This is a template project for creating books using Gitbook.

## What is the software required to install it ?

You must have installed [node.js](https://nodejs.org), [Git]((https://git-scm.com/downloads)) and the [Gitbook Command Line tools](https://github.com/GitbookIO/gitbook-cli)

- For node.js
  - To check if the node.js is installed, you may execute:
  
    ```
    $ npm -v
    ```
    
  - if it is not installed, you must download and install the software from [the official node.js website](https://nodejs.org/en/download/)

- For Git
  - To check if Git is installed, you may execute:
  
    ```
    $ git --version
    ```
    
  - if it is not installed, you must download and install the software from [the official Git website](https://git-scm.com/downloads)

- For Gitbook Cli (command line tools)
  - To check if Gitbook-Cli is installed, you may execute:
    ```
    $ gitbook -V
    ```

  - If it is not installed, you must install the package using ``npm`` as an administrator
  
    ```
    $ npm install -g gitbook-cli
    ```
    
  - In linux or mac, you may use ``sudo``to set the user and the path for the ``.npm`` folder and install the package
  
    ```
    $ export PATH=$PATH:$HOME/.npm-packages/bin
    $ sudo chown -R $USER:$GROUP ~/.npm
    $ sudo npm install -g gitbook-cli
    ```


## How to install it ?

If you want to edit the book using the [Gitbook Editor](https://www.gitbook.com/editor), you only need to clone the repository. 
You may create a new book in the editor using the resulting Git repository.

To deploy the book in a [Github-Pages website](https://pages.github.com/), you must change the URL for the repository in the ``package.json`` file.

- Check the URL of the repository in the Github.
- Replace the URL of the repository. By default, it is "noname/noname.git"

## How to run it ?

The project includes a set of commands that can be used to automate part of the process.

- **To install or update the Gitbook plugins**

  ```
  $ npm run book:prepare
  ```

- **To preview the book.** It runs a webserver where you can review the book while you are writing. Any change in the book is displayed immediately.

  ```
  $ npm run book:watch
  ```

- **To create the book** (in Windows)

  ```
  $ npm run book:build
  ```

- **To publish the book in a Github-Pages website** (in Windows)

  ```
  $ npm run book:publish
  ```

- **To create the book** (in Linux)

  ```
  $ npm run book:build-linux
  ```

- **To publish the book in a Github-Pages website** (in Linux)

  ```
  $ npm run book:publish-linux
  ```

