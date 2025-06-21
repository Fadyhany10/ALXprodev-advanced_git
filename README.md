# ALXprodev-advanced_git

#!/bin/bash

# Step 1: Install git-flow (for Debian/Ubuntu)
echo "Installing git-flow..."
sudo apt-get update
sudo apt-get install -y git-flow

# Step 2: Clone the empty repository
echo "Cloning remote repository..."
git clone https://github.com/YOUR_USERNAME/ALXprodev-advanced_git.git
cd ALXprodev-advanced_git || exit

# Step 3: Create and push develop branch
echo "Creating develop branch..."
git checkout -b develop
git push -u origin develop

# Step 4: Initialize git-flow with default settings
echo "Initializing git-flow..."
git flow init -d

# Step 5: Create an empty README file
echo "Creating README.md..."
touch README.md

# Step 6: Stage, commit and push the file
echo "Committing README.md..."
git add README.md
git commit -m "Add empty README.md"
git push

echo "GitFlow setup complete."
