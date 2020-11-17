### Make sure you have [git bash](https://git-scm.com/downloads) installed:

1. Run `git --version` in the CMD/bash/terminal.

1. If some `git not recognized error message` is getting display on running the above command, then install [git bash](https://git-scm.com/downloads).

<hr>

### Make sure git is tracking your project.

1. Using your terminal/command line, get inside the folder where your project files are kept: 
  `cd /path/to/my/codebase`.
  <br>You can also do this simply by opening the folder using file explorer, and then right click and opening `git bash` in that project root directory.

1. Check if `git` is already initialized: `git status`
<br>If you get this error message: `fatal: Not a git repository (or any of the parent directories): .git`, that means the folder you are currently in is not being tracked by `git`. In that case, initialize `git` inside your project folder by typing `git init`, then going through the process of adding and committing your project. 
<br>If you get another error message, read carefully what it says. Is it saying `git` isn't installed on your computer by saying that the word 'git' is not recognized? Is it saying that you're already in a folder or sub-folder where `git` is initialized? Google your error and/or output to understand it, and to figure out how to fix it.

<hr>

### Create a remote, empty folder/repository on Github.

1. Login to your Github account. 

1. At the top right of any Github page, you should see a '+' icon. Click that, then select 'New Repository'. 

1. Give your repository a name--ideally the same name as your local project. If I'm building a authentication php project, its folder will be called 'auth-php-app' on my computer, and 'auth-php-app' will be the Github repository name as well.

1. Click 'Create Repository'. The next screen you see will be important, so don't close it.

<hr>

### Connect your local project folder to your empty folder/repository on Github.

The screen you should be seeing now on Github is titled **'Quick setup — if you’ve done this kind of thing before'**. 

Copy the link in the input right beneath the title, it should look something like this: 
`https://github.com/setupspiders/auth-php-app.git` 
This is the web address that your local folder will use to push its contents to the remote folder on Github.

1. Go back to your project in the terminal/command line. 

1. In your terminal/command line, type `git remote add origin [copied web address]`
<br> Example: `git remote add origin https://github.com/setupspiders/auth-php-app.git`

1. Push your branch to Github: `git push origin main` 

1. Go back to the folder/repository screen on Github that you just left, and refresh it. The title **'Quick setup — if you’ve done this kind of thing before'** should disappear, and you should see your files there. 
