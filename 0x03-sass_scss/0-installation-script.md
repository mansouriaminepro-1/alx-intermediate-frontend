# 0-installation-script
# Purpose: Document the steps taken to install SASS for the alx-intermediate-frontend project
# Date: 2025-09-14

##########
# Option A - Ubuntu (using nvm) - Recommended
##########

# 1) Install nvm
curl -o- https://raw.githubusercontent.com/nvm-sh/nvm/v0.39.7/install.sh | bash

# 2) Exit the terminal and reopen it (or run the following lines to load nvm immediately)
export NVM_DIR="$HOME/.nvm"
[ -s "$NVM_DIR/nvm.sh" ] && \. "$NVM_DIR/nvm.sh"

# 3) Install Node.js v20.16.0
nvm install 20.16.0
nvm use 20.16.0

# 4) Verify Node & npm versions
node -v     # expected: v20.16.0
npm -v

# 5) Install SASS (project-local, dev dependency)
npm install --save-dev sass@3.7.4

# 6) Verify installation
npx sass --version

##########
# Option B - Install anywhere (if Node already installed) - Global install
##########

npm install -g sass@3.7.4
sass --version
