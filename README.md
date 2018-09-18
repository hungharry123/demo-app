# demo-app


# WEEK 2

## Set up development environment

1. nvm install node
2. curl -o- https://raw.githubusercontent.com/creationix/nvm/v0.33.11/install.sh | bash
3. export NVM_DIR="${XDG_CONFIG_HOME/:-$HOME/.}nvm"
4. [ -s "$NVM_DIR/nvm.sh" ] && \. "$NVM_DIR/nvm.sh"
5. command -v nvm
6. -v nvm
7. [ -s "$NVM_DIR/bash_completion" ] && \. "$NVM_DIR/bash_completion"
8. export NVM_DIR="$HOME/.nvm" && (   git clone https://github.com/creationix/nvm.git "$NVM_DIR";   cd "$NVM_DIR";   git checkout `git describe --abbrev=0 --tags --match "v[0-9]*" $(git rev-list --tags --max-count=1)`; ) && \. "$NVM_DIR/nvm.sh"
9. nvm install 6.14.4(version: 10.10.0, 8.1.0, ... )
10. node -v
11. nvm use node
12. nvm run node --version

## Create React application using Facebook create-react-app

1. npm install create-react-app -g
2. cd *folder to create app* 
3. npm init react-app __*my-app*__ *(name of app)*

### *if fail try this and do 14 - 15 again:*
 
- chmod -R 777 ~/.npm/ OR sudo chmod -R 777 ~/.npm/

4. npm install yarn -g 
5. cd __*my-app*__
6. yarn start

### *if you want to run:*
 
 7. yarn build 

 ### *if you want to run with local port:*

 8. npm install -g __*serve*__ (name of server)
 9. yarn global add serve
 10. sudo serve -s build __OR__ serve -s build

 ### *if you want to debug:*


11. yarn test

 ### *if you want to build:*

 12. yarn eject
