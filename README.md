# GitHub Pages Demo Website

This is a small static website created for **Session 2: Static Website Hosting with GitHub Pages**.

The website is intentionally simple. Its purpose is to demonstrate GitHub Pages hosting and deployment, not advanced web design.

## Project structure

```text
demo-project/
|-- README.md
|-- index.html
|-- style.css
`-- images/
    `-- profile-placeholder.svg
```

## Run locally

Open this file in a browser:

```text
index.html
```

You can also open the folder in VS Code, right-click `index.html`, and open it in the browser.

## Push to GitHub

Create an empty public repository on GitHub. Do not add a README, `.gitignore`, or license from GitHub.

Then run these commands from inside this `demo-project` folder:

```bash
git init
git add .
git commit -m "Initial website"
git branch -M main
git remote add origin <repository-url>
git push -u origin main
```

Replace `<repository-url>` with your GitHub repository URL.

## Configure GitHub Pages

1. Open the repository on GitHub.
2. Go to **Settings**.
3. Open **Pages**.
4. Under **Build and deployment**, choose **Deploy from a branch**.
5. Select:

   ```text
   Branch: main
   Folder: /root
   ```

6. Save the settings.

After a short time, GitHub will show the live website URL.

## Update and redeploy

Make a small change in `index.html` or `style.css`, then run:

```bash
git add .
git commit -m "Update website content"
git push
```

GitHub Pages will redeploy the website automatically after the push.

## Expected GitHub Pages URL

For a project website, the URL usually looks like:

```text
https://username.github.io/repository-name/
```

