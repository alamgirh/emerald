---
layout: post
title: How to create a blog in GitHub using Jekyll Theme?
date: 2016-12-16
author: Alamgir Hossain
categories: Tutorial
tags: Jekyll GitHub HTML blog
published: true
---

<img src="http://timjames.me/img/jekyll/feature.jpg" class="fit image"> 

I will describe, step by step, how to build a blog  powered by Jekyll, a fantastic static website generator which is easily maintainable. I will also describe how to host your Jekyll site, for free, in a GitHub repository.

## Steps:

- Step 1: Create a [GitHub](https://github.com/) account
  - For example, your GitHub account name is **meghna**.
  - Create a repository, for example, your new repository name is **padma**. For little bit practice to know how GitHub works, you can create a [GitHub Pages](https://pages.github.com/). Write someting that you like in the README.md file. Go to Settings -> Options. Then you will find GitHub Pages paragraph where you can find a button (Choose a theme). Click the button Choose a theme and Select Theme. Finally, your README.md file will use as a content of your website. Your website address is http://**meghna**.github.io/**padma** . Yes, anyone can view your website and finally you created a website in GitHub!   
  - For writing README.md file you may learn Markdown which is super easy. You may see [Markdown-Cheatsheet](https://github.com/adam-p/markdown-here/wiki/Markdown-Cheatsheet).

- Step 2: Want to practice HTML - the key ingredient for creating a website?  
  - Create a repository **meghna**.github.io . Create an index.html file. If you are new HTML user you may find tutorial from [w3schools](http://www.w3schools.com/html/) 

- Step 3: Find a [Jekyll Theme](https://jekyllthemes.io/)

- Step 4: Find the repository in GitHub that theme you have chosen. Fork that repository.
  - Create the gh-pages branch if only master branch available. For convenience to maintain the website, you may set gh-pages as a default branch using settings > Branches > Default branch. 
  - Follow the instructions from the readme file provided by the theme developers.

- Step 5: Edit the file _config.yml according to your information. 
  - Specially edit the base hostname & protocol for your site (e.g. url: "https://username.github.io") and the subpath of your site (e.g. baseurl: "/repositoryname/" ) 

- Step 6: Write your first blog inside the folder _posts. For example, your new file name is 2016-12-16-My-First-Blog.md . You may use [http://prose.io](http://prose.io), which is more convenient that I found. You may change some other files inside the folder _includes to make your blog more personal from the original theme.

## During this process you need to know the following
- [GitHub for Beginners](https://guides.github.com/activities/hello-world/) 
- Basic HTML. I learn HTML 5 from YouTube [Tutorial](https://www.youtube.com/playlist?list=PL1A2CSdiySGIlme1vVXbXBZpK1aDb4TBG) and the Bangla tutorial [বেসিক ওয়েবসাইট ডিজাইন](http://shikkhok.com/%E0%A6%95%E0%A7%8B%E0%A6%B0%E0%A7%8D%E0%A6%B8-%E0%A6%A4%E0%A6%BE%E0%A6%B2%E0%A6%BF%E0%A6%95%E0%A6%BE/basic-website-design/). This Bangla tutorial is super interesting. If you only know how to on-off a computer you can even create a website!  
- Markdown, a lightweight markup language, is super easy to learn. If I forget anything, I see the [Markdown-Cheatsheet](https://github.com/adam-p/markdown-here/wiki/Markdown-Cheatsheet).
- Basic idea about [Jekyll](https://jekyllrb.com/). I learn Jekyll from YouTube [Tutorial](https://www.youtube.com/playlist?list=PLWjCJDeWfDdfVEcLGAfdJn_HXyM4Y7_k-). 
<br>
<br>

> Happy blogging! Hopefully your writing will help others not hurt others.
