# Website Maintenance Documentation
## Web Designer: Kevin Jang (k1jang@ucsd.edu)

---
## Table of Contents
1. Prerequisites
   1. Bare minimum guide on Markdown and HTML/CSS
2. <a href="">Getting Started with GitHub and Jekyll</a>
   1. GitHub
   2. VS Code
   3. Jekyll
3. Organizational flow of GitHub
4. Creating the next issue
   1. Creating the issue page
   2. Creating the folder for issue posts
      1. Creating a text only post
      2. Creating an artwork post
      3. Creating custom posts (rare)
5. Checking the new page
6. Updating Forms, Links
7. Updating Editorial Team and Alumni
8. FAQ
---
# Getting Started with GitHub and Jekyll
**Alchemy the Journal** is managed through GitHub and deployed on GitHub Pages using Jekyll. GitHub is a collaborative development platform used throughout the CSE Department's courses. GitHub Pages is a deployment platform for client-side websites, so this is perfect for hosting a fully-customizable literary magazine. Using GitHub, GH Pages, and Jekyll is completely free (except for owning the domain), so this is a very cost-effective option. I recommend applying for a GitHub Pro account using an **@ucsd.edu** email because UCSD has this plan and it keeps this repository private so people can't see the internal code behind Alchemy. Jekyll is an open-source static-site generator that makes it easy to write blog posts using templated pages.

## GitHub
The repository is located at (https://github.com/Kevin-Jjang/Alchemy-UCSD). In order to make updates to the Alchemy website, I highly recommend using a code editor such as Microsoft VS Code because you should preview how the posts look once you write them. 

## VS Code

Install VS Code here. 

You will then open the Explorer as seen above. Then click on ```Clone Repository```. This will open the command palette where you will then copy the link to the GitHub repo at (https://github.com/Kevin-Jjang/Alchemy-UCSD) and paste it in that area. Press enter and select a destination on your local device to keep a local version of the website's code. Afterwards, you should see this screen. You have successfully created a local version of Alchemy and remotely connected it to the GitHub repository!!! 

## Jekyll 
Jekyll is an open source static-site generator that makes it easy to write blog posts using templated pages. To get started, follow the [jekyll installation guide](https://jekyllrb.com/docs/installation/). You will want to install Ruby so you can locally run Jekyll. You do not need to run the commands ```gem install jekyll bundler``` and ``` jekyll new blog``` because this blog is already established.

# Organizational Design

```
/ (root)
| 
|-- _data
|-- _includes
|-- _issues
|   |-- _issuesCoverPage (cover pages)
|   |-- _term## (where all posts for the term## should be stored)
|
|-- _layouts
|-- _posts
|-- assets
| 
```

