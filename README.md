5 GitHub Guide: Creating a Repository with Contributors and Requiring Owner Approval for Code Merges 

PART 1 Creating a Repository with Contributors and Rules 

1. Creating a GitHub Repository 

Go to GitHub and log in. 

Click on the "+" icon in the top right and select "New repository". 

Enter a repository name and select visibility (Public or Private). 

Check "Initialize this repository with a README" (optional). 

Click "Create repository".  

2. Adding Contributors to the Repository  

Go to your repository and click on the "Settings" tab. 

In the left sidebar, click "Collaborators and teams". 

Under "Manage access", click "Invite a collaborator". 

Enter the GitHub username or email of the contributor. 

Click "Add collaborator" and send an invite (people who you want to work with). 

The invited contributor must accept the invitation before they can contribute. 

3. Setting Up Branch Protection (Requiring Owner Approval) 

Go to your repository’s "Settings" tab. 

Click "Branches" in the left sidebar. 

Under "Branch protection rules", click "Add rule". 

In the "Branch name pattern" field, enter main (or your default branch name). 

Enable the following:  

"Require a pull request before merging". 

"Require approvals" (Set required approvals to at least 1). 

"Require review from code owners" (Ensures only the owner can approve changes). 

(Optional) Require status checks to pass before merging. 

Click "Save changes". 

4. Setting Up Code Ownership 

To ensure only the repository owner must approve code changes before merging: 

Create a .github/CODEOWNERS file in the root of the repository. 

Add the following content: * @ greentreegroup / @glynac 

This makes the repository owner the mandatory reviewer before merging any code. 

   

PART 2 Access to Repository and Make Modification 

1. How Contributors Can Access the Repository 

Once added as a collaborator: 

The contributor should accept the invitation sent to their GitHub account. 

Clone the repository locally using:  

git clone https://github.com/greentreegroup/glynac.ai-website.git 
  

Navigate into the project directory:  

cd your-repo 
  

2. How a Contributor Can Push Changes 

Create a new branch: git checkout -b feature-branch 
  

Make changes and commit: git add . 
git commit -m "Added new feature" 
  

Push to GitHub: git push origin feature-branch 
  

Create a Pull Request (PR):  

Go to the GitHub repository. 

Click "Pull Requests" → "New pull request". 

Select feature-branch as the source and main as the target. 

Click "Create pull request". 

3. How the Owner Can Review and Merge Code 

Go to "Pull Requests" in the GitHub repository. 

Open the new pull request. 

Review the changes and leave comments if needed. 

Click "Approve". 

Click "Merge pull request" to merge the changes into main. 

(Optional) Delete the feature-branch after merging. 

 

GLYNAC PRIVATE REPO   

4. How to access to the private repo 

1. How to access private access to the repo, Please watch this, https://youtu.be/Lhyu_2iLO8w?si=_hGtwn1Fx6Pp-ith 

2. as an intern you need to create your own branch when push, or you can ask your supervisor which branch to push 

5. file requirement to push the code 

1.	Before you push your code, you need to create a proper documentation and what is the requirement to install and run the code, like you working in the python, you can include requirement.txt or config file  

2. 	Include Proper readme, please follow this link for the structure  
 

Questions: 

You are working on an open-source Python project hosted on GitHub. The project is a simple web scraper that extracts data from a public website and stores it in a CSV file. You have written the core functionality, but now you need to create a comprehensive README file, how the Readme file look like  
