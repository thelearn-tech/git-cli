# git-cli
A tutorial on how to maintain repo with local repo aka how to push files with cli.

## Contains  


  
  
  
# Step 1)

  ## Creating a Personal token

create a **Public Access Token** from
[here](https://github.com/settings/tokens) or go to **Settings** > **Developer** **Settings** > **Personal** **Access** **Token**

and create a **token**.

![pa Token](https://raw.githubusercontent.com/thelearn-tech/img/main/IMG_20220101_132744.jpg)

I just gave **repo** permission but you can change according to your needs.


#  Step 2)

 ## Creating a Repository.


  First create a **Public** or **Private** **Repository** without adding **.gitignore** file, you can add **README.md** and **LICENCE** .
  
  ![repo img](https://raw.githubusercontent.com/thelearn-tech/img/main/IMG_20220101_131716.jpg)
  
  
# Step 3)

  ## Installing ***git*** and **gh**
  
  Installation guide [here](https://github.com/git-guides/install-git#:~:text=To%20install%20Git%2C%20run%20the,installation%20by%20typing%3A%20git%20version%20.)

  
  Installation on termux
  <br>
  `pkg install git gh -y` or 
  <br>
  `apt install git gh -y`

# Step 4) 

  ## git and verify install of git and gh

I am using **Termux**. u can use **linux, mac or windows**.

open **Terminal** or **CMD**

type   `git --version` 
<br> 
type    `gh --version`
<br>

to verify installation of **git** and **gh**.


![gh and git](https://raw.githubusercontent.com/thelearn-tech/img/main/IMG_20220101_161325.jpg)

get your email from [here](https://github.com/settings/emails) or **Settings** > **Emails**

If you have private email then your email will look some thing like this ![email](https://raw.githubusercontent.com/thelearn-tech/img/main/IMG_20220101_163547.jpg)


now type   `git config --global user.name "youUserName"`

and type `git config --global user.email "yourEmail"`

like this 
![git auth](https://raw.githubusercontent.com/thelearn-tech/img/main/IMG_20220101_162613.jpg)

change ***youUserName*** to your github user name like `git config --global user.name "thelearn-tech"` and do same for your email. 


# Step 5)

  ## Authentication to github with gh
  
type  `gh login --with-token "yourToken"`

replace **yourToken** with the token you created in [Step 1](#)