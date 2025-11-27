# GitHub
👉 "Hands-on Git &amp; GitHub practice repository covering essentials, advanced commands, workflows, and real DevOps use cases."

Setting Up Code Repository in GITHUB:
---------------------------------------
1. Goto www.github.com & Create an Account.
2. Create New Repository as "CentralGit"
3. Description : Centralized Repository
4. Choose Public.
5. Create Repository

Install & Configure Git:
------------------------
sudo su
yum update -y
yum install git -y
git --version

git config --global user.name "<region_specific_username>"
git config --global user.email "<your_email@example.com>"
git config --list

Workflow of Git:
------------------------

<img width="800" height="568" alt="image" src="https://github.com/user-attachments/assets/ea01b82f-47f3-40da-ac04-2ee8d36aa305" />


Git Lifecycle Explanation
-------------------------
Working Directory → (git add) → Staging Area 
Staging Area → (git commit) → Local Repository 
Local Repository → (git push) → Remote Repository (GitHub)



