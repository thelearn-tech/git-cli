# git-cli
A tutorial on how to maintain repo with local repo aka how to push files with cli.

## Contains  

#  step 1)

 ## Creating a Repository.


  First create a **Public** or **Private** **Repository** without adding **.gitignore** file, you can add **README.md** and **LICENCE** .
  
  ![repo img](https://raw.githubusercontent.com/thelearn-tech/img/main/IMG_20220101_131716.jpg)
  
  
  
  
# step 2)

  ## Creating a Personal token

create a **Public Access Token** from
[here](https://github.com/settings/tokens) or go to **Settings** > **Developer** **Settings** > **Personal** **Access** **Token**

and create a **token**.

![pa Token](https://raw.githubusercontent.com/thelearn-tech/img/main/IMG_20220101_132744.jpg)

I just gave **repo** permission but you can change according to your needs.


# step 3)

  ## Installing ***git*** and **gh**
  
  Installation guide [here](https://github.com/git-guides/install-git#:~:text=To%20install%20Git%2C%20run%20the,installation%20by%20typing%3A%20git%20version%20.)

  
  Installation on termux
  <br>
  `pkg install git gh -y` or 
  <br>
  `apt install git gh -y`

# step 4) 

  ## Authenticating to github with gh

I am using **Termux**. u can use **linux, mac or windows**.

open **Terminal** or **CMD**

type   `git --version` 
<br> 
type    `gh --version`
<br>

to verify installation of **git** and **gh**.


![gh and git](https://raw.githubusercontent.com/thelearn-tech/img/main/IMG_20220101_161325.jpg)

now type   `git config --global user.name "youUserName"`

change ***youUserName*** to your github user name like `git config --global user.name "thelearn-tech"`