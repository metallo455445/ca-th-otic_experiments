# Installation guide (fedora edition)

## Pre-requisites
- git installed on pc

## 1. Repo cloning
![image](sprites/screen1.png)
1. Go to the main screen of the repo
2. Press the green <code>Code</code> button
3. Select Local -> clone -> HTTPS and copy the link using the appropriate button
4. On your PC, open the terminal and navigate to any folder EX:<code>/.../Documents/</code>

<code>!!WARNING!!</code> you do **not** need to create a folder called *ca-th-otic_experiments*, it will be created automatically during the cloning phase

5. Run the command:

        git clone <<*copied_link*>>

## 2. Create a new Branch
Once you have chosen the ticket you want to complete, you will open a Branch that implements that feature. First of all, it is always advisable to do a 

    git pull

in general every time before starting to work (good practice :D).
After that, you can create the actual Branch with the command:

    git checkout -b <<*branch_name*>>

This creates a local Branch that allows you to comfortably work on your code (without creating it in the cloud!)

## 3. Upload changes
After working on **THAT SPECIFIC BRANCH**, the time comes to upload the changes made to the common cloud. 

1. prepare the files to upload

        git add <<*stuff*>

    allows you to select the file path of the files you want to upload. If you want to upload everything without leaving any file behind, you can use more conveniently:

        git add .

2. commit creation <br>
    The commit is simply a comment added to the files you uploaded that briefly describes what you did. Common examples can be:

        "fix-ticket-6" or "updated with new data"

    the command to commit is:

        git commit -m "<<*message*>>"

3. PUSH <br>
    At this point, you have to press the last intoxicating Enter before launching our files onto the cloud. This is done via a sensational command (because pressing Enter fills you with energy):

        git push -u origin <<*branch_name*>>

## Authentication <br>
The first time you do a push of this kind, you will be asked to authenticate <br>

1. username: your github name, email is fine too
2. password/token: this can cause confusion because it's not the github account password but rather a token

## Generate a token <br>  
1. Click on your profile icon (top right) -> settings -> scroll down to *Developer settings*
![image](sprites/dev_set.png)

2. .
![image](sprites/token_classic.png)

3. .
![image](sprites/gent_token.png)

4. At this point it will ask you to authenticate, log in normally, then this screen will open
![image](sprites/costomize_token.png) 
check all the boxes, in the notes write whatever you like (like pc fedora) and then generate the token

5. copy the token and insert it where required

## Merge Conflicts
Bad stuff, ask gemini...
