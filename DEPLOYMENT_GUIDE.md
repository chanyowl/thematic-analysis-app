# Deployment Guide: Uploading to GitHub & Hosting on GitHub Pages

Follow these simple steps to push this project to your GitHub account and make it live on the web so it can interact with your n8n workflow.

---

## Step 1: Create a New GitHub Repository
1. Go to [github.com/new](https://github.com/new) (make sure you are logged in).
2. Name your repository (for example: `thematic-analysis-app`).
3. Set the repository visibility to **Public** (this is required for free GitHub Pages hosting).
4. **Important**: Leave "Add a README file", "Add .gitignore", and "Choose a license" **UNCHECKED** (we have already created them locally).
5. Click **Create repository**.

---

## Step 2: Push your Local Code to GitHub
Copy and run the following commands in your terminal (make sure you are inside the `/Users/aipo/Desktop/Antigravity Thematic Analysis App` folder):

```bash
# 1. Add your new GitHub repository as the remote origin
git remote add origin https://github.com/<YOUR_GITHUB_USERNAME>/<YOUR_REPO_NAME>.git

# 2. Push your main branch to GitHub
git push -u origin main
```
*(Replace `<YOUR_GITHUB_USERNAME>` and `<YOUR_REPO_NAME>` with your actual GitHub username and the repository name you just created).*

---

## Step 3: Enable GitHub Pages (Free Hosting)
Once your code is pushed successfully:
1. Open your repository page on GitHub.
2. Click on the **Settings** tab at the top of the page.
3. In the left-hand menu, under the "Code and automation" section, click on **Pages**.
4. Under **Build and deployment**:
   * **Source**: Select `Deploy from a branch`.
   * **Branch**: Click the dropdown (currently saying `None`) and select **`main`**.
   * **Folder**: Keep it as **`/ (root)`**.
5. Click the **Save** button.

---

## Step 4: Access Your Live App
1. Wait about 30 to 60 seconds for GitHub to build and deploy your site.
2. Refresh the GitHub Pages settings page. You will see a banner at the top showing your live URL:
   `Your site is live at https://<your-username>.github.io/<your-repo-name>/`
3. Click the link to open your live web application!
4. Configure your persona, open the export modal, input your n8n Webhook URL and Google Spreadsheet details, and click **Trigger Automated n8n Pipeline** to start the analysis from anywhere on the web.
