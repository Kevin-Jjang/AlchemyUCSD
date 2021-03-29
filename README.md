# Website Maintenance Documentation
## Current site: https://kevin-jjang.github.io/AlchemyUCSD/
## Web Designer: Kevin Jang (k1jang@ucsd.edu)

---
## Table of Contents
1. Prerequisites
   1. Markdown (~1 hour to learn)
   2. HTML (~30-60 min to learn basics if Markdown is known)
   3. CSS (~3 hours to be proficient in, recommended to learn)
      1. Google Inspect Tool (DevOps) 
2. Getting Started with GitHub and Jekyll
   1. GitHub
   2. VS Code
   3. Jekyll
3. Organizational Design
4. Creating the next issue
   1. Creating the issue page
   2. Creating the folder for issue posts
      1. Creating a text only post
      2. Creating an artwork post
      3. Creating custom posts (use .html extension)
5. Reviewing the new pages
6. Pull Request to the deployment branch
7. Updating Forms, Links (submissions.html)
8. Updating Editorial Team and Alumni (_data, team.html)
9. FAQ
---
# Getting Started with GitHub and Jekyll
**Alchemy the Journal** is managed through GitHub and deployed on GitHub Pages using Jekyll. GitHub is a collaborative development platform used throughout the CSE Department's courses. GitHub Pages is a deployment platform for client-side websites, so this is perfect for hosting a fully-customizable literary magazine. Using GitHub, GH Pages, and Jekyll is completely free (except for owning the domain), so this is a very cost-effective option. I recommend applying for a GitHub Pro account using an **@ucsd.edu** email because UCSD has this plan and it keeps this repository private so people can't see the internal code behind Alchemy. Jekyll is an open-source static-site generator that makes it easy to write blog posts using templated pages.

## GitHub
The repository is located at (https://github.com/Kevin-Jjang/AlchemyUCSD). The GitHub Pages where the website is viewed is located at (https://kevin-jjang.github.io/AlchemyUCSD/) In order to make updates to the Alchemy website, I highly recommend using a code editor such as Microsoft VS Code because you should preview how the posts look once you write them. 

## VS Code

Install VS Code here. 

[insert image with circle around file explorer, clone repo, and pasted url]

You'll then open the Explorer as seen above. Then click on `Clone Repository`. This will open the command palette where you will then copy the link to the GitHub repo at (https://github.com/Kevin-Jjang/AlchemyUCSD) and paste it in that area. Press enter and select a destination on your local device to keep a local version of the website's code. Afterwards, you should see this screen. You have successfully created a local version of Alchemy and remotely connected it to the GitHub repository!!! 

## Jekyll 
Jekyll is an open source static-site generator that makes it easy to write blog posts using templated pages. To get started, follow the [jekyll installation guide](https://jekyllrb.com/docs/installation/). You will want to install Ruby so you can locally run Jekyll. You do not need to run the commands ```gem install jekyll bundler``` and ``` jekyll new blog``` because this blog is already established.

# Organizational Design

```
AlchemyUCSD (root)
| 
├── _data               # Update .yml files as editors and issues are updated
├── _includes           # (Ignore) Header/footer templates
├── _layouts            # Match a layout to a post, or create a custom post in HTML
├── assets              # Upload images, pdfs, etc. in here
|   └──+ 
|      ├── css
|      ├── font
|      ├── img          
|      ├── js           # (Ignore) email me animation designs and I'll make them
|      ├── pdf
├── _issuesCoverPage
|   └── term##.html     # The cover page for the term##
├── _term##             # Where all posts for the term## should be stored
|
├── .github             # (Ignore) For CI/CD Pipeline 
├── index.html          # Homepage https://kevin-jjang.github.io/AlchemyUCSD/
├── issues.html         # Issues Page
├── submissions.html    # Submissions Page
├── team.html           # Meet the Team Page
├── about.html          # Contact Us Page
├── _config.yml         # 
├── Gemfile             # 
```
## Creating the Next Issue
The folder `_term##` should not be modified and instead duplicated as a new folder. It contains an HTML page for the cover art and the Letter from the Editor for easy setup.