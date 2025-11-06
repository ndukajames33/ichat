# 1. Initialize a Git repo (if not already done)
git init

# 2. Add all files and make the first commit
git add .
git commit -m "Initial commit: project setup"

# 3. Update README
echo "## Project Overview" >> README.md
git add README.md
git commit -m "Add project overview to README"

# 4. Add main code file
echo "print('Hello, world!')" > main.py
git add main.py
git commit -m "Add main script with hello world"

# 5. Add .gitignore
echo "__pycache__/" > .gitignore
git add .gitignore
git commit -m "Add .gitignore to exclude Python cache files"

# 6. Create requirements file
echo "flask" > requirements.txt
git add requirements.txt
git commit -m "Add Flask dependency"

# 7. Add config file
echo "DEBUG=True" > config.env
git add config.env
git commit -m "Add basic config file"

# 8. Modify main.py with a function
echo "def greet(name):\n    return f'Hello, {name}!'" >> main.py
git add main.py
git commit -m "Add greet function to main.py"

# 9. Update README with usage section
echo "### How to Run\nRun \`python main.py\` to start the script." >> README.md
git add README.md
git commit -m "Add usage instructions to README"

# 10. Final cleanup
git add .
git commit -m "Final cleanup and formatting"
