# git-cli
A tutorial on how to maintain repo with local repo aka how to push files with cli.

# Contains 

 * Authentication
     * [**Create a personal token**](#step-1)
     
     * [**Creating `SSH`key**](#step-2) 
     
     * [**Installing `git` and `gh`**](#step-3)
 
     * [**Git setup**](#step-4)

     * [**Authentication to github with `gh`**](#step-5)
 * Clonning
     * [**Clone repository with `SSH`**](#step-6) 
  
 


  
  
  
# Step 1)

  ## Creating a Personal token

create a **Public Access Token** from
[here](https://github.com/settings/tokens) or go to **Settings** > **Developer** **Settings** > **Personal** **Access** **Token**

and create a **token** with a minimum of full **repo** and full **admin:org** and full **admin:public_key** permission.

![pa Token](https://raw.githubusercontent.com/thelearn-tech/img/main/IMG_20220413_102222.jpg)
![read org](https://raw.githubusercontent.com/thelearn-tech/img/main/IMG_20220413_102249.jpg)



#  Step 2)
  
## Creating a `SSH` key

 ![ssh Keygen](https://raw.githubusercontent.com/thelearn-tech/img/main/IMG_20220408_081622.jpg)
 [Make sure to use your GitHub  public email]

`ssh-keygen -t rsa -b 4096 -C "your public email"`





# Step 3)

  ## Installing ***git*** and **gh**
  
  Installation guide for git [here](https://github.com/git-guides/install-git#:~:text=To%20install%20Git%2C%20run%20the,installation%20by%20typing%3A%20git%20version%20.)

  Installation guide for gh [here](https://github.com/cli/cli/blob/trunk/docs/install_linux.md)
  
  Installation on termux
  <br>
  `pkg install git gh -y` or 
  <br>
  `apt install git gh -y`


  **verify install of git and gh**


type   `git --version` 
<br> 
type    `gh --version`
<br>

to verify installation of **git** and **gh**.

![gh and git](https://raw.githubusercontent.com/thelearn-tech/img/main/IMG_20220101_161325.jpg)

# Step 4)
  ## GIT setup

get your email from [here](https://github.com/settings/emails) or **Settings** > **Emails**

If you have private email then your email will look some thing like this ![email](https://raw.githubusercontent.com/thelearn-tech/img/main/IMG_20220101_163547.jpg)


<br>
now type   `git config --global user.name "youUserName"`

and type `git config --global user.email "yourEmail"`

like this 
![git auth](https://raw.githubusercontent.com/thelearn-tech/img/main/IMG_20220101_162613.jpg)

change ***youUserName*** to your github user name like `git config --global user.name "thelearn-tech"` and do same for your email. 


# Step 6)

  ## Authentication to github with gh
  
type  `gh auth login --with-token "yourToken"`

replace **yourToken** with the token you created in [Step 1](#step-1)



## Now **git** and **gh** is setted up.

# Step 7) 

## cloning the Repository 

`git clone https://github.com/yourUserName/yourRepo`

and `cd` in to it.
 <br>

![clone repo](https://raw.githubusercontent.com/thelearn-tech/img/main/IMG_20220101_202020.jpg)

# Step 8)

 # pulling and commiting and pushing
 

 <br>

![setup img](https://raw.githubusercontent.com/thelearn-tech/img/main/IMG_20220102_105927.jpg)
 
<br>
 <br>

 `git init`
 
<br>

then `git pull`
 
<br>
 <br>

 `git pull` before adding or changing any files. It's very important!!
 
<br>

 now add file or change existing one as a update.
 
<br>

 I added a file called `example.txt`
 
<br>

 now if you do `git status` then you will see `untracked file`
 
<br>

 adding the file `git add example.txt` 
 
<br>

 here `example.txt` is file name to be added . 

 <br>
 <br>
 
To add all files use `git add .`
 
<br>

 `.` means all files in that directory.
 
 <br>
 
 if you do `git status` now then it will show **new file:**
 
<br>

 now commit with `git commit -m "pushing file in cli"`

<br>

 here `-m` in `git commit -m` stands for **comment** like `git commit -m "comment"`
 

simple do `git push`

And done.
