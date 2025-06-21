# 1. Switch to the develop branch
git checkout develop

# 2. Create and switch to a new feature branch
git checkout -b feature/implement-login

# 3. Create the login-page directory and add a README file with placeholder content
mkdir login-page
echo "Login Feature Coming soon" > login-page/README.md

# 4. Stage and commit the new files
git add login-page/README.md
git commit -m "feat: scaffolding login page"

# 5. Push the new branch to the remote repository
git push -u origin feature/implement-login
