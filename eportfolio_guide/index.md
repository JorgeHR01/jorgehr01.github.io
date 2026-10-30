---
layout: default
---

# How I Built My GitHub Pages E-Portfolio

## Introduction

I created this e-portfolio as part of OM 620, Tools and Technologies for Analytics, at CSUSM. The goal was to have a website where I could share my background, skills, and projects as I work through the MS in Supply Chain Analytics program and any future career endeavors. I used GitHub Pages to host the website and the Minimal theme as the starting design. This guide covers the main steps I followed for creating my first portfolio, along with the files I changed to make the site my own.

## 1. Setting Up GitHub Pages

### Creating the Repository

I started with my GitHub account, `jorgehr01`, and a repository named `jorgehr01.github.io`. The repository name matters because GitHub Pages uses the username followed by `.github.io` for a personal site. My website address is [jorgehr01.github.io](https://jorgehr01.github.io/).

### Working With the Files Locally

I worked with a local copy of the repository so I could edit the files on my computer. GitHub Desktop and Visual Studio Code are two ways to manage the repository and its files. Once the changes are saved locally via Visual Studio, they still need to be committed and pushed through GitHub Desktop before they appear on GitHub. Saving a file on my computer by itself does not update the website.

## 2. Adding the Minimal Theme

For the design, I used the [Minimal theme for GitHub Pages](https://github.com/pages-themes/minimal). The theme gives the site a simple layout. I downloaded the theme's files from its GitHub repository and placed them into my portfolio repository.

I kept the overall layout because it was straightforward and worked well for a resume-style portfolio. The theme also includes a README file that explains its usage and configuration options.

![Minimal theme files in my repository](/assets/img/eportfolio_guide/theme_files.png)

*The original Minimal theme files are included in my portfolio repository.*

## 3. Configuring the Site

### Editing `_config.yml`

One of the most important files was `_config.yml`, which controls several settings for the site. I changed the title to **Jorge's Portfolio** and added a short description about the projects and work I want to showcase. I also set `show_downloads` to `false`.

The same file includes `remote_theme: pages-themes/minimal@v0.2.0` and the `jekyll-remote-theme` plugin. These settings tell Jekyll which theme to use when building the site.

![My portfolio configuration file](/assets/img/eportfolio_guide/config_settings.png)

### Adding My Picture

The original theme included a stock `logo.png` image. For my portfolio, I added a graduation picture named `Graduation.png` to the `assets/img` folder. Then I pointed the `logo` setting in `_config.yml` to `/assets/img/Graduation.png`.

I did not rename my picture to `logo.png`; I changed the image path to my Graduation.png file instead.

![My profile picture being added](/assets/img/eportfolio_guide/added_profile_pic.png)

## 4. Writing the Homepage

### Updating `index.md`

The root `index.md` file contains the main page of the portfolio. I replaced the sample theme content with information about my education, work experience, and skills. I organized the page similarly to a resume, starting with my name and summary, followed by work experience, education, projects, and skills.

For work experience, I included my role helping manage my family's landscaping business, as well as my sales and retail experience. Under education, I included my studies at CSUSM and UC Berkeley. 

![Markdown used for my homepage](/assets/img/eportfolio_guide/homepage_markdown.png)

### Using Markdown

Markdown let me format the page without writing all the HTML myself. Some formatting I used included:

- `#`, `##`, and `###` to organize headings and subheadings.
- `**bold text**` to emphasize details.
- `*italic text*` for supporting information, including dates and school details.
- Bulleted lists for work responsibilities and an ordered list for developing technical skills.
- A Markdown link to my LinkedIn profile.

The structure helped make the information easier to read while keeping the source file fairly simple. I could edit the Markdown in VS Code and check how it looked before publishing.

## 5. Updating the README

I also edited `README.md` so someone visiting the GitHub repository would know it was my personal website. I included a short introduction and a reference to the original Minimal theme. The README explains the repository, while `index.md` contains the content people see on the website.

![README for my GitHub Pages repository](/assets/img/eportfolio_guide/readme_excerpt.png)

## 6. Committing and Publishing the Changes

After editing the files, the last step was publishing them. The workflow was to review the local changes, write a commit message, commit those changes, and push them to GitHub. A commit records a version of the project; pushing sends those commits from my computer to the GitHub repository.

GitHub Pages then builds and publishes the website. I can check the repository's **Actions** tab for a successful **pages build and deployment** and visit the site itself to confirm the changes appear as expected.

For this second milestone, I also created the `eportfolio_guide` folder with its own `index.md` file and added a link to it under **Projects** on the homepage. This makes the guide a separate page without creating a different website.

## 7. Final Portfolio

The result is a personal website with my graduation photo, background, education, work experience, and skills. It also has a Projects section that links to this guide. The site can continue to grow as I complete more coursework and develop new projects to share.

![My completed e-portfolio](/assets/img/eportfolio_guide/final_portfolio.png)

## Resources
- [GitHub Pages](https://pages.github.com/)
- [Minimal theme source and documentation](https://github.com/pages-themes/minimal)

[Back to my portfolio](/)
