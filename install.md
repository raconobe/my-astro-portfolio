Let’s wipe the slate clean and start fresh with **Astrofy**. It combines your blog, projects, roadmap notes, and CV into one clean layout.

---

### Step 1: Clean Up & Clone Astrofy

Run these commands sequentially in your Debian terminal to remove any previous test folders and set up Astrofy fresh:

```bash
# Move to your projects base directory
cd ~/Desktop/projects-vault-raco

# Clean up any leftover folders from earlier attempts
rm -rf my-starlight-vault molecular-moon

# Clone Astrofy directly into your target directory
git clone https://github.com/manuelernestog/astrofy.git web-dev-roadmap

# Enter the project folder
cd web-dev-roadmap

# Install all project dependencies
npm install

# Start the local development server
npm run dev

```

Once the server starts, open `http://localhost:4321` in your browser to view your live Astrofy dashboard.

---

### Step 2: Key Files to Personalize Astrofy

#### 1. Site Metadata (`src/config.ts`)

Open `src/config.ts` to set global defaults:

```typescript
export const SITE_TITLE = 'Raul | Dev Roadmap & Vault';
export const SITE_DESCRIPTION = 'Software Engineering, Web Development & System Notes';
export const GENERATE_SLUG_FROM_TITLE = true;
export const TRANSITION_API = true;

```

#### 2. Sidebar Profile & Links (`src/components/SideBar.astro`)

* **Avatar Image:** Replace `public/profile.webp` with your preferred image.
* **Navigation Links:** Edit `src/components/SideBar.astro` to add or modify menu items (e.g., Home, Roadmaps, CV, Blog).

#### 3. Main Landing Page (`src/pages/index.astro`)

Open `src/pages/index.astro` to customize your welcome header, personal bio, recent projects, and featured blog posts.

#### 4. Adding Roadmap Articles (`src/content/blog/`)

Articles inside Astrofy use Markdown files located in `src/content/blog/`. Create a file like `src/content/blog/frontend-roadmap.md`:

```markdown
---
title: "Frontend Development Roadmap"
description: "Core topics: HTML5, CSS Grid/Flexbox, JavaScript ES6+, and Vue/React."
pubDate: "2026-10-11"
heroImage: "/post_img.webp"
badge: "Frontend"
---

# 🎨 Frontend Roadmap

Welcome to the frontend vault! Here are the core topics and resources...

```

#### 5. Customizing Your Resume (`src/pages/cv.astro`)

Edit `src/pages/cv.astro` to update your work experience, education history, and technical skill badges using the built-in `<TimeLineElement/>` components.

---

### Step 3: Link to GitHub

If you want to push this fresh Astrofy vault to your `web-dev-roadmap` GitHub repository:

```bash
# Re-initialize git for your personal repository
rm -rf .git
git init

# Stage and commit initial Astrofy setup
git add .
git commit -m "Initialize web-dev-roadmap with Astrofy template"

# Link to your remote GitHub repository
git branch -M main
git remote add origin git@github.com-raco:raconobe/web-dev-roadmap.git

# Push to GitHub
git push -u origin main --force

```




---


Let’s wipe the slate clean and start fresh with **Astrofy**. It combines your blog, projects, roadmap notes, and CV into one clean layout.

---

### Step 1: Clean Up & Clone Astrofy

Run these commands sequentially in your Debian terminal to remove any previous test folders and set up Astrofy fresh:

```bash
# Move to your projects base directory
cd ~/Desktop/projects-vault-raco

# Clean up any leftover folders from earlier attempts
rm -rf my-starlight-vault molecular-moon

# Clone Astrofy directly into your target directory
git clone https://github.com/manuelernestog/astrofy.git web-dev-roadmap

# Enter the project folder
cd web-dev-roadmap

# Install all project dependencies
npm install

# Start the local development server
npm run dev

```

Once the server starts, open `http://localhost:4321` in your browser to view your live Astrofy dashboard.

---

### Step 2: Key Files to Personalize Astrofy

#### 1. Site Metadata (`src/config.ts`)

Open `src/config.ts` to set global defaults:

```typescript
export const SITE_TITLE = 'Raul | Dev Roadmap & Vault';
export const SITE_DESCRIPTION = 'Software Engineering, Web Development & System Notes';
export const GENERATE_SLUG_FROM_TITLE = true;
export const TRANSITION_API = true;

```

#### 2. Sidebar Profile & Links (`src/components/SideBar.astro`)

* **Avatar Image:** Replace `public/profile.webp` with your preferred image.
* **Navigation Links:** Edit `src/components/SideBar.astro` to add or modify menu items (e.g., Home, Roadmaps, CV, Blog).

#### 3. Main Landing Page (`src/pages/index.astro`)

Open `src/pages/index.astro` to customize your welcome header, personal bio, recent projects, and featured blog posts.

#### 4. Adding Roadmap Articles (`src/content/blog/`)

Articles inside Astrofy use Markdown files located in `src/content/blog/`. Create a file like `src/content/blog/frontend-roadmap.md`:

```markdown
---
title: "Frontend Development Roadmap"
description: "Core topics: HTML5, CSS Grid/Flexbox, JavaScript ES6+, and Vue/React."
pubDate: "2026-10-11"
heroImage: "/post_img.webp"
badge: "Frontend"
---

# 🎨 Frontend Roadmap

Welcome to the frontend vault! Here are the core topics and resources...

```

#### 5. Customizing Your Resume (`src/pages/cv.astro`)

Edit `src/pages/cv.astro` to update your work experience, education history, and technical skill badges using the built-in `<TimeLineElement/>` components.

---

### Step 3: Link to GitHub

If you want to push this fresh Astrofy vault to your `web-dev-roadmap` GitHub repository:

```bash
# Re-initialize git for your personal repository
rm -rf .git
git init

# Stage and commit initial Astrofy setup
git add .
git commit -m "Initialize web-dev-roadmap with Astrofy template"

# Link to your remote GitHub repository
git branch -M main
git remote add origin git@github.com-raco:raconobe/web-dev-roadmap.git

# Push to GitHub
git push -u origin main --force

```
