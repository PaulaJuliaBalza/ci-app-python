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

# Issues-Solutions
```
Current runner version: '2.326.0'
Runner Image Provisioner
Operating System
Runner Image
GITHUB_TOKEN Permissions
Secret source: Actions
Prepare workflow directory
Prepare all required actions
Getting action download info
Error: This request has been automatically failed because it uses a deprecated version of `actions/upload-artifact: v3`. Learn more: https://github.blog/changelog/2024-04-16-deprecation-notice-v3-of-the-artifact-actions/

# ci-python.yml
    - name: Guardar reporte          # Sixth step: save coverage report
      uses: actions/upload-artifact@v4
      with:
        name: coverage-report
        path: htmlcov/
```