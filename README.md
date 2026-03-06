# ShiningStars Early Learning Center - Static Website Template

A fast, pre-generated HTML website built using the [Eleventy](https://www.11ty.dev/) static site generator. 

This repository serves as a beautiful, modern starting point for a Daycare, Preschool, or Early Childhood Education center. It includes pre-built layouts for Home, Programs, About, Gallery, and Contact pages.

## Features

* **Lightning Fast:** Scores 100/100/100/100 in Lighthouse performance tests 🔥
* **No Javascript Frameworks:** 100% lightweight HTML and CSS.
* **Modern CSS Design:** Built with CSS Variables, Flexbox, and CSS Grid.
* **Responsive Layouts:** Looks great on mobile, tablet, and desktop.
* **Automatic Navigation:** Powered by the [Eleventy Navigation](https://www.11ty.dev/docs/plugins/navigation/) plugin.
* **Working Contact Form:** Designed to integrate seamlessly with Netlify Forms.
* **Markdown Content:** Easy to edit page content using standard Markdown.

---

## 🚀 Getting Started

Follow these steps to customize and run the ShiningStars site on your own machine.

### 1. Requirements

Ensure you have the following installed on your machine:
* [Node.js](https://nodejs.org/) (v14 or higher is recommended)
* `npm` (Node Package Manager - comes with Node.js)
* Git

### 2. Clone the Repository

Clone this project to your local machine and switch into the directory.

```bash
git clone https://github.com/danurbanowicz/eleventy-netlify-boilerplate.git sunshine-daycare
cd sunshine-daycare
```

### 3. Install Dependencies

Install the project modules required by Eleventy.

```bash
npm install
```

### 4. Customizing Your Daycare Information

The core site information is stored in the `_data/metadata.json` file. 

Open `_data/metadata.json` and change the title, URL, email, and description to match your Daycare.

```json
{
  "title": "Your Daycare Center Name",
  "url": "https://your-daycare-url.com/",
  "language": "en",
  "description": "Your daycare description.",
  "author": {
    "name": "Director Name",
    "email": "info@your-daycare-url.com"
  }
}
```

You can edit the content on the individual pages (Home, About, Programs, Contact) by modifying the `.md` files located in the `/pages/` directory.

### 5. Running the Site Locally

To preview your site as you make changes:

```bash
npm run serve
```
This will compile the CSS and HTML and start a local server, usually at `http://localhost:8080`. The site will automatically refresh when you save changes.

To perform a production build (without the local server):

```bash
npm run build
```

---

## 🌐 Deployment to Netlify

This project is optimized for deployment on Netlify. It includes a working Contact Form (`pages/contact.md`) that Netlify will automatically process.

### Step 1: Push Your Code to GitHub (or GitLab/Bitbucket)

1. Create a new repository on your GitHub account.
2. Link your local project to your new remote repository:
   ```bash
   git remote remove origin
   git remote add origin https://github.com/yourusername/your-new-repo.git
   git push -u origin main
   ```

### Step 2: Connect to Netlify

1. Log in to [Netlify](https://app.netlify.com/).
2. Click **"Add new site"** and choose **"Import an existing project"**.
3. Select your Git provider (e.g., GitHub).
4. Authorize Netlify and choose the repository you just created.
5. In the build settings, Netlify should automatically detect the settings:
   - **Build Command:** `npm run build`
   - **Publish directory:** `_site`
6. Click **"Deploy site"**.

Your Daycare website is now live! Netlify will automatically rebuild and publish your site every time you push new changes to the `main` branch.
