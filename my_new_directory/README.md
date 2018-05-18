This is my new readme file.

So this is kind of confusing but I think I am starting to get it. 

So far what I have done is:

1. created a new directory on my computer called my_new_directory.
  I did this by first going into the direcroty called Development
  then typing mkdir my_new_directory
2. I changed into the new directory by typing in cd my_new_directory
3. Within this new directory I created a new file called README.md 
  I did this by typing in touch README.md

note: you can add text to a file from the command line by doing the following:

echo "This is the text that's being added" > README.md (this is the filename which 
could also be different. in this case it so happens to be adding text to README.md)

4. Once the baove steps were completed I then went onto my GitHub account
  and made sure it was logged in. And created a new repository.
5. once the new repo was created I copied the link to my clipboard.
6. then I went to my terminal to finish setting up. Basically connecting the remote repo which lives on GitHub online to my local repo.
7. I ran a bunch of commands in my terminal to set this up.
  git init
  git add .
  git commit -m "initialize git"
  git remote add origin your-remote-repository-url

8. then I modified this readme with all the things I wrote above and am getting ready to push these changes to the remote repository. 
9. I will need to first track and commit all the changes that I've made so far. you cant just execute the command git push.
10. first you need to run the following commands:
  git add .
  git commit -m "add additional content to README"
11. Now I can use git push -u origin master
  the -u flag is short for --set-upstream and we only need to use this flag the first time we use git push. It tells the current local branch to track itself against the amster branch of origin, the remote repo I am pushing to. Once you set up this upstream link with -u you can then just simply execute the commang git push and git pull without specifying any arguments (such as target branch or repo)