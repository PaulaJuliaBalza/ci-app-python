# Create project
```
mkdir ci-app-python
cd ci-app-python
git init 
nano README.md
git add .
git commit -m "initial commit"
```
# Create the structure
```
mkdir -p .github/workflows
```

# Upload the repository
Create repository in Github.
```
git remote add origin https://github.com/PaulaJuliaBalza/ci-app-python.git
git branch -M main
git push -u origin main
```

📌 En GitHub → pestaña “Actions” vas a ver tu workflow ejecutándose automáticamente.