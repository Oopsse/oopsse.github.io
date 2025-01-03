+++
date = '2025-01-03T17:17:26+01:00'
title = 'Set up Hugo and Github Pages'
+++

## Hugo 

+ https://gohugo.io/hosting-and-deployment/hosting-on-github/
+ https://selfscrum.medium.com/42-steps-from-zero-to-an-automated-github-website-built-with-hugo-2fa001827db1

git clone https://github.com/Oopsse/oopsse.github.io.git
cd oopsse.github.io
hugo new site . --force
git submodule add https://github.com/Oopsse/hugo-theme-mini.git themes/mini
mkdir -p .github/workflows
vi .github/workflows/hugo.yaml
git add -A
git commit -m "Hugo"
git push
hugo new posts/Hugo.md
