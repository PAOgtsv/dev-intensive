# dev-intensive
Dev-intensive. Learning hot to make Android apps

# TASK 1.
# Create an account on GitHub
# Status: DONE
## ISSUES: simple
## ADDIT INFO: -
## STEPS: 
### 1. Go to a github website and regeistrate new account. 
### 2 Reseive the message and click the 'prove' link


# TASK 2.
# Download Git on a computer
# Status: DONE
## ISSUES: simple
## ADDIT INFO: -
## STEPS: -


# TASK 3. 
# Install Git on the computer
# Status: DONE
## ISSUES:
## ADDIT INFO: make sure you set options you want. For I didn't know most of them I just get recomended options
## STEPS: 
### 1. follow instructions installing app
### 2. choose all options like Git Bash, Git GUI, Git CMD

# TASK 4.
# Instal SSH key on Github to avoid setting log-pas couple changing files on computer
# Status: DONE
## ISSUES: 
### 1. There was misunderstanding how to use GIT BASH
### 2. Also the found information confused me. I was forced to combine info from both two sources to get this task done
## ADDIT INFO:
### 1. https://htmlacademy.ru/blog/boost/tools/git-console
### 2. https://only-to-top.ru/blog/tools/2019-12-08-git-ssh-windows.html
## STEPS:
### 1. So, firstly we have to generate a key. We use followed command to make it
#### $ ssh-keygen -t rsa -b 4096 -C "sometext"
#### sometext is whatever you want. Pay attention on upper-case C before the "sometext".
### 2. Then, you are asked to generate passphrase (also you may keep it empty)
#### there might be problems with pass. 
### 3. Once you get a message you create the key (footprint, img and directory) we have to add the key to you ssh agent. And first step here is launching the agent
#### Use this command:
#### $ eval "$(ssh-agent -s)"
#### I had a problem with it, because before I found this solution i bump into $ eval 'ssh-agent -s'
#### Despite the last solution started the agent I couldn't add a key to it. It cause a problem. Then I found the right solution above
### 4. Add the key to agent
#### There was no problem using the command
#### $ ssh-add ~/.ssh/key_title
#### where key_name is a ypur key's title
### 5. Add a key to github account
#### in your GIT Bash type follow command - $ cat ~/.ssh/key_title.pub and copy the key
#### where key_name is a ypur key's title
#### Get to the "SSH and GPG keys" menu on an account
#### title the key (however you want)
#### paste the code and save options

