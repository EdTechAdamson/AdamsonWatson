<h1 align="center" style="border-bottom: none;">🚀 Web UI w/ Watson Assistant API Sample Application</h1>
<h3 align="center">This Web app demonstrates the usage of the Watson Assistant service in a simple interface with a subject selected.</h3>
<p align="center">
  <a href="http://travis-ci.org/watson-developer-cloud/assistant-simple">
    <img alt="Travis" src="https://travis-ci.org/watson-developer-cloud/assistant-simple.svg?branch=master">
  </a>
  <a href="#badge">
    <img alt="Github contributors" src="https://img.shields.io/github/all-contributors/all-contributors/all-contributors">
  </a>
  <br>
  <img width="500" src="https://www.dallasisd.org/cms/lib/TX01001475/Centricity/Domain/16974/New%20Banner.jpg">
  <br>
  <img width="250" src="https://media.giphy.com/media/hTATwczg9Sy7l66C6Q/giphy.gif">
  <img width="440" src="https://media.giphy.com/media/l0HlMldqhAt3QYEh2/giphy.gif">
</p>
</p>




## Prerequisites

1. Sign up for an [IBM Cloud account](https://cloud.ibm.com/registration/).
1. Download the [IBM Cloud CLI](https://cloud.ibm.com/docs/cli/index.html#overview).
1. Create an instance of the Watson Assistant service and get API script:


## Install and setup your environment

### Download and install [VSCode](https://code.visualstudio.com/Download)
1. If you are having trouble look through the this [setup guide](https://code.visualstudio.com/docs/setup/setup-overview)

### Install [Git](https://git-scm.com/downloads)- this tracks changes so you can recall or recover your work.
1. After installation navigate to the command line.
1. In windows 10 , navigate to the CLI using one of the following methods.
     - Start menu > Windows System > Command Prompt
     - Start menu > Windows PowerShell > Windows PowerShell
     - Windows Logo Key+X

1. For macOS, you can find the CLI using one of the following methods.
    - In Finder menu bar, navigate to Go > Utilities > Terminal
    - Or in Finder, navigate to Applications > Utilities > Terminal
    - Or use the shortcut Command+Shift+U and select Terminal to open.
    
### Setup your Git identity
1. Type ```git --version``` into the CLI to see that Git installed.
1. Type ..... replacing ```your name``` and ```you@email.com``` with your github username and github email
    ```
    git config --global user.name "Your Name"
    git config --global user.email you@example.com
    ```
    
> ####

> #  Instructions on how to use this repository as a basis to start your project

### Create a local clone of this fork
1. On the right top corner of this repo, click ```
1. Above the list of files, click  ```Code```.
1. To clone the repository using HTTPS, under "Clone with HTTPS", click .
1. Open Git Bash.
1. ``` $ git config --global credential.helper wincred ```
1. Type ``` cd documents```
1. Create a project folder by typing ``` mkdir Admason```
1. Navigate into the folder by typing ``` cd Adamson ```
1. Type git clone, and then paste the URL you copied earlier. It will look like this, with your GitHub username instead of YOUR-USERNAME:
  ```
  $ git clone https://github.com/YOUR-USERNAME/Spoon-Knife
  ```
1. Press Enter. Your local clone will be created.
  ```
  $ git clone https://github.com/YOUR-USERNAME/Spoon-Knife
> Cloning into `Spoon-Knife`...
> remote: Counting objects: 10, done.
> remote: Compressing objects: 100% (8/8), done.
> remove: Total 10 (delta 1), reused 10 (delta 1)
> Unpacking objects: 100% (10/10), done.
  ```
### Configure git to sync with original repository
1. On GitHub, navigate to the original repository.
1. Above the list of files, click  ```Code```, and clone with HTTPS
1. Open Git Bash
1. Change directories to the location of the fork you cloned in above.
    - To go to your home directory, type just cd with no other text.
    - To go into one of your listed directories, type cd your_listed_directory.
1. Type git remote -v and press Enter. You'll see the current configured remote repository for your fork.
  ```
  $ git remote -v
> origin  https://github.com/YOUR_USERNAME/YOUR_FORK.git (fetch)
> origin  https://github.com/YOUR_USERNAME/YOUR_FORK.git (push)
  ```
  
1. Type git remote add upstream, and then paste the URL you copied earlier and press Enter. It will look like this:
  ```
  $ git remote add upstream https://github.com/octocat/Spoon-Knife.git
  ```
1. To verify the new upstream repository you've specified for your fork, type git remote -v again. You should see the URL for your fork as origin, and the URL for the original repository as upstream.
  ```
  $ git remote -v
> origin    https://github.com/YOUR_USERNAME/YOUR_FORK.git (fetch)
> origin    https://github.com/YOUR_USERNAME/YOUR_FORK.git (push)
> upstream  https://github.com/ORIGINAL_OWNER/ORIGINAL_REPOSITORY.git (fetch)
> upstream  https://github.com/ORIGINAL_OWNER/ORIGINAL_REPOSITORY.git (push)
  ```
 
### Open up this repository with VSCode
1. Open VSCode and click on ```Terminal``` in the top navigation bar.
1. Type ``` cd documents ```
1. Type ``` cd Adamson ```
1. Type ``` code . ```
1. Navigate to the icons on the left, click the boxes icon, type in ``` open in broswer```. This is an extension that will allow you to view your code in the broswer. Install the one by TechER.
1. Navigate back to the ```index.html``` file. Hover over the file, right click and select ```Open in Default Browser``` or use the keyboard shortcut Alt+B.

> ####

> # Instructions on how to create your own project
    
## Set up the structure of your web app
### Opening with Visual Studio Code
1. Upon opening VSCode , a welcome page opens.
1. At the top, click terminal, new terminal.
    - type ``` cd documents```
    - Create a project folder by typing ``` mkdir Admason```
    - Navigate into the folder by typing ``` cd Adamson ```
    - We must then initialize our project as a git repo, type ``` git init ```
    - Lets create some files to get us started, type...
    ```
    code index.html main.css app.js
    ```
    - Lets see what we made, this next command will open a new window into the prject directory
    ```
    code .
    ```

## Lets add some text to our web app
1. In VSCode, lets open ```index.html``` on the left hand side, type ```html:5```, and hit enter.
    - Lets rename our title to ```Adamson```
    - Lets add some body
    ```
    <body>
      <h1>Task Timeline</h1>
      <p id="date"></p>
      <ul>
        <li class="list">Edit the head</li>
        <li class="list">Edit the body</li>
        <li>Link to JavaScript</li>
      </ul>
    </body>
    ```
    - Lets link to the JavaScript file, type ``` script: src``` right before the last body tag. Your code should look like this.
    ```
    <!DOCTYPE html>
    <html lang="en" dir="ltr">
      <head>
        <meta charset="utf-8">
        <title>Task Timeline</title>
        <link rel="stylesheet" href="main.css">
      </head>
      <body>
        <h1>Task Timeline</h1>
        <p id="date"></p>
        <ul>
          <li class="list">Edit the head</li>
          <li class="list">Edit the body</li>
          <li>Link to JavaScript</li>
        </ul>
        <script src="app.js"></script>
      </body>
    </html>
    ```
    - Navigate to the icons on the left, click the boxes icon, type in ``` open in broswer```. This is an extension that will allow you to view your code in the broswer. Install the one by TechER.
    - Navigate back to the ```index.html``` file. Hover over the file, right click and select ```Open in Default Browser``` or use the keyboard shortcut Alt+B.

## Lets add some styling to our web app
1. Open the ```main.css``` file and type...
  ```
  body {
  font-family: helvetica;
}

ul {
  font-family: monospace;
}

li {
  list-style: circle;
}

.list {
  list-style: square;
}

#date {
  font-size: 12px;
  font-style: italic;
  font-weight: bold;
}
  ```
1. Save all work, right click on ```index.html``` and select ```Open In Default Browser``` 

## Lets add some JavaScript
### Implementing strict mode
1. Strict reduces silent errors, improves performance, provides more warnings, and fewer unsafe features when beginning with JavaScript.
1. Type ```'use strict'```

1. Add todays date 
    - First, you'll retrieve a new date from the built-in JavaScript object. It looks like this new Date(). 
    - Next, you can transform the date format by using toDateString().
    - The HTML needs to know where you want to add this information on the page or document, so retrieve an element using getElementById('date').
    - The final step is to insert the date string inside the selected element with innerHTML.
    ```
    let today = new Date();
    let formatDate = today.toDateString();
    let selectElement = document.getElementById('date');
    selectElement.innerHTML = formatDate;
    ```

    - Here we're using the word let to create a variable named today, which holds the date and time. It's a convention to use camel case for variable names with more than one word—for example, the variable formatDate.

    - When you declare a variable, it holds a reference to the value you assign. Variables are a useful way of storing information temporarily so you can reuse the values. In the selectElement variable, you're saving the result of reformatting the date. In that step, you remove the time and timezone from using toDateString().
    
    - Save all work, right click on ```index.html``` and select ```Open In Default Browser``` 
    
## Lets Track our changes with Git
### Open Terminal on VSCode
1. Type ``` git add . ```
    
1. Type ``` git commit -m "Initial commit"```
    
1. Type ``` git push```






## Contributing

See [CONTRIBUTING](CONTRIBUTING.md).

## Open Source @ IBM

Find more open source projects on the
[IBM Github Page](http://ibm.github.io/).


[doc_intents]: https://cloud.ibm.com/docs/services/conversation/intents-entities.html#planning-your-entities
[docs]: https://cloud.ibm.com/docs/services/assistant/index.html#index
[docs_landing]: (https://cloud.ibm.com/docs/services/assistant/index.html#index)
[sign_up]: https://cloud.ibm.com/registration
