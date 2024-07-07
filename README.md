# fullstack-repo-HW

Starting by creating front-end-HW repository and back-end-HW repository, creating client.py and server.py files.
Creating fullstack-repo-HW, adding front-end-HW and back-end-HW as submodules:

git submodule add https://github.com/amirhilal044/back-end-HW.git frontend-repo
git submodule add https://github.com/amirhilal044/front-end-HW.git backend-repo
              
![Screenshot (77)](https://github.com/amirhilal044/fullstack-repo-HW/assets/81297156/3c2bd527-9395-4862-8c1f-64e2ab57d419)

Creating config.yaml in the root fo fullstack-repo-HW

Commit and Push changes

Setup Auto-Update ofr Submodules using gitHub Actions

Creating .github/workflows/update-submodules.yml file in fullstack-repo-HW to automatically update submodules on push events

#How it Works
Front-end-HW and Back-end-HW are individual repositories, each repository contains its own Python class ('cliend.py and server.py.), These classes read the configuration from a config.yaml file located two directories up, which will be the root of fullstack-repo-HW
Full-stack-HW (unified repo) Contains config.yaml file and, front-end-HW and back-end-HW as submodules, config.yaml contains ServerIPAddress that can be accessed by client.py and server.py

then comes the auto update: The github actions workflow in fullstack-repo-HW can ensure that any changes pushed to front-end-HW or back-end-HW are automatically reflected in fullstack-repo-HW.
