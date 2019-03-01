# Programming Club Week 5

## Setup

There are four things that need to be installed. Simply using the defualt settings should suffice.
- [Python](https://www.python.org/downloads/) 3.7
- [VSCode](https://code.visualstudio.com/) or another IDE if you prefer (though this tutorial is for VSCode)
- [Python VSCode extension](https://marketplace.visualstudio.com/items?itemName=ms-python.python)
- [Git](https://git-scm.com/download)

An email and username is necessary to upload code with git.
First right click in any folder and select `Git Bash Here`, or open up a command prompt or terminal.

![](https://i.ibb.co/p2QLrFx/explorer-2019-03-01-13-15-44.png)

Next, set your email and username with the commands below.
```sh
git config --global user.name "John Doe"
git config --global user.email johndoe@example.com
```

## Cloning

Copying a repository of code to your local computer is called a **clone**.
To clone a GitHub repository, open up VSCode and press `Ctrl Shift P`

![](https://i.ibb.co/VYt25RH/Code-2019-03-01-13-27-13.png)

This shows a list of commands. Type `clone` and click the `Git: Clone` option.

![](https://i.ibb.co/XDF4VBP/Code-2019-03-01-13-29-15.png)

![](https://i.ibb.co/wMtgXVn/Code-2019-03-01-13-30-31.png)

It will ask you for the repository URL. To get this, go to the GitHub page you want to clone, click `Clone or download` and copy the URL.

![](https://i.ibb.co/hX55j5D/chrome-2019-03-01-13-24-58.png)

Paste in the URL, press `Enter`, and select a folder. Make sure to open the repository.

![](https://i.ibb.co/jrCF3Qq/Code-2019-03-01-13-34-11.png)

This is equivalent to executing `git clone <url> <folder>`.

To later access the code on your computer, go to `File` then `Open Folder...` and open the cloned folder.

![](https://i.ibb.co/WktXsbZ/Code-2019-03-01-13-44-51.png)

## Making changes

The first step is to **stage** the changes. After a file has been added, deleted, or modified, go to the `Source Control` tab and click the `+` icon on any files you want.

![](https://i.ibb.co/V9KqkDT/2019-03-01-13-58-13.png)

This is equivalent to `git add <file>`.

Next, type a descriptive message in the message box, and press `Ctrl Enter`. This will create a **commit**, the way Git internally stores changes.
The next step is to sync commits between your computer and the online repository.

![](https://i.ibb.co/yPpfNwW/Code-2019-03-01-14-03-01.png)

This is equivalent to `git commit -m "Message"`.

## Syncing

In the bottom left corner of VSCode, there is an icon that shows how many commits need to be downloaded (pulled) and uploaded (pushed).

![](https://i.ibb.co/LQSb0LN/2019-03-01-13-49-58.png)

Click the icon to sync changes between the remote repository and your computer.
This is roughly equivalent to `git push origin master` and `git pull origin master`.
