Personal Portfolio Website

A personal portfolio website showcasing my background, technical interests, projects, and learning journey in IT infrastructure, cloud technologies, and automation.

* Live Website: danieldebra.com
* GitHub Repository: personal-portfolio-website

Overview

This repository contains the source code for my personal portfolio website. I implemented a Continuous Integration (CI) workflow using GitHub Actions and integrated it with Netlify’s deployment workflow.

The project demonstrates practical experience with version control, automated HTML validation, pull request workflows, branch protection, and automated website deployments.

Technologies Used

Technology	Purpose
HTML5	Website structure and content
CSS3	Website styling and layout
Git	Version control
GitHub	Source code hosting and collaboration workflow
GitHub Actions	Automated validation through CI
Netlify	Website hosting, preview deployments, and production deployments

CI/CD Workflow

GitHub Actions validates changes before they are merged into the production branch. Netlify manages preview and production deployments.

Workflow

1. Development: Website changes are made locally using Git and VS Code.
2. Feature branches: Changes are developed on separate branches rather than directly on main.
3. Pull requests: A pull request proposes merging changes into main.
4. Automated validation: GitHub Actions checks that required website files exist and validates HTML markup.
5. Branch protection: The main branch requires pull requests and successful CI status checks before merging.
6. Preview deployment: Netlify generates a preview deployment so changes can be reviewed before release.
7. Production deployment: After changes are merged into main, Netlify automatically deploys the updated website.

GitHub Actions Checks

The CI workflow is defined in .github/workflows/ci.yml.

It runs on pushes to main and feature branches matching feature/**, as well as pull requests targeting main.

The workflow performs the following checks:

* Confirms that index.html exists.
* Confirms that css/style.css exists.
* Runs automated HTML validation.

These checks help identify issues before changes reach the production branch.

Repository Structure

personal-portfolio-website/
├── .github/
│   └── workflows/
│       └── ci.yml
├── css/
│   └── style.css
├── index.html
└── README.md

Local Development

1. Clone the repository

git clone https://github.com/danielodebra/personal-portfolio-website.git
cd personal-portfolio-website

2. Create a feature branch

git switch -c feature/your-change

Replace your-change with a short description of your work.

3. Make and test your changes

Edit the relevant files in your preferred code editor and check the website in a browser.

4. Commit and push your changes

git add README.md
git commit -m "Add project README"
git push -u origin docs/add-project-readme

These commands illustrate the documentation change. For future work, stage the files you have actually changed.

5. Open a pull request

On GitHub, open a pull request from your documentation branch into main.

Wait for the required CI checks to pass, review the changes, and merge when everything looks correct.

After merging, verify that the production deployment completes successfully.

Project Goals

This project was developed to:

* Apply Git and GitHub version control practices.
* Implement automated validation using GitHub Actions.
* Understand CI workflows and required status checks.
* Practise pull request-based development and branch protection.
* Integrate source control with Netlify preview and production deployments.
* Build practical experience relevant to cloud infrastructure and DevOps engineering.

Future Improvements

Potential enhancements include:

* Automated link checking.
* Accessibility testing.
* Additional automated quality and security checks where appropriate.
* Further improvements to the development and deployment workflow.

Author

Daniel

IT Support Engineer developing practical skills in cloud infrastructure, Windows infrastructure, automation, and DevOps.

* Portfolio: danieldebra.com
* GitHub: danielodebra