# 🗂️ Project Management App

A fully functional and responsive **Project Management Application** built with **React**, **Vite**, and **Tailwind CSS**. It enables users to create and manage projects and associated tasks seamlessly. The application is deployed using **Azure Static Web Apps** with CI/CD powered by **GitHub Actions**.

---

## 🚀 Features

- 🔨 Create and delete projects
- ✅ Add, view, and manage tasks for each project
- 🎨 Modern UI built with Tailwind CSS
- ⚡ Lightning-fast dev experience via Vite
- ☁️ Deployed to Azure Static Web Apps
- 🔄 Automatic deployment via GitHub Actions

---

## 🛠️ Tech Stack

| Tech               | Purpose                    |
|--------------------|-----------------------------|
| **React**          | Frontend UI library         |
| **Vite**           | Fast bundler & dev server   |
| **Tailwind CSS**   | Utility-first CSS framework |
| **Azure SWA**      | Cloud hosting               |
| **GitHub Actions** | CI/CD for deployment        |

---

## 📁 Folder Structure

```
project-management-app/
├── dist/                   # Build output (after `npm run build`)
├── public/                 # Static assets
│   ├── Screenshot 2025-04-30 213926.png
│   ├── Screenshot 2025-04-30 214319.png
│   └── Screenshot 2025-04-30 214348.png
├── src/
│   ├── assets/             # Images like 'no-project.png'
│   ├── components/         # All UI components
│   │   ├── Button.jsx
│   │   ├── Input.jsx
│   │   ├── Modal.jsx
│   │   ├── NewProject.jsx
│   │   ├── NewTask.jsx
│   │   ├── NoProjectSelected.jsx
│   │   ├── ProjectSidebar.jsx
│   │   ├── SelectedProject.jsx
│   │   └── Tasks.jsx
│   ├── App.jsx             # Main application component
│   ├── main.jsx            # Entry point
│   └── index.css           # Tailwind and custom styles
├── .github/workflows/
│   └── azure-static-web-apps.yml # GitHub Actions for Azure
├── index.html
├── tailwind.config.js
├── vite.config.js
├── package.json
└── README.md
```

---

## 🧑‍💻 Local Development

### Prerequisites

- Node.js v16+
- Git

### Steps

1. **Clone the Repository**

```bash
git clone https://github.com/your-username/project-management-app.git
cd project-management-app
```

2. **Install Dependencies**

```bash
npm install
```

3. **Start Development Server**

```bash
npm run dev
```

Visit: [http://localhost:5173](http://localhost:5173)

---

## 🧱 Build for Production

```bash
npm run build
```

This will generate the optimized build in the `/dist` folder.

---

## ☁️ Azure Static Web Apps Deployment

### Step-by-Step Azure Setup

1. **Install VS Code Azure Tools Extension Pack**  
2. **Login to Azure inside VS Code**
3. Open the Command Palette and run:  
   `Azure Static Web Apps: Create Static Web App...`
4. **Fill details**:
   - App location: `/`
   - API location: *(leave blank)*
   - Build output location: `dist`
5. Azure creates a GitHub Actions workflow:  
   `.github/workflows/azure-static-web-apps.yml`
6. On every push to the repo, your app gets built and deployed automatically.

---

## 🌍 Live Demo

> Add your Azure Static Web Apps live link here  
> Example: [https://your-app-name.azurestaticapps.net](https://your-app-name.azurestaticapps.net)

---

## 📸 Screenshots

```md
![Project Overview](./public/Screenshot%202025-04-30%20213926.png)
![Task View](./public/Screenshot%202025-04-30%20214319.png)
![Add New Project](./public/Screenshot%202025-04-30%20214348.png)
```

---

## 📃 License

This project is licensed under the **MIT License**.  
Feel free to use and modify it as needed.

---

## 🙌 Credits

Thanks to the following tools:

- [React](https://reactjs.org/)
- [Vite](https://vitejs.dev/)
- [Tailwind CSS](https://tailwindcss.com/)
- [Azure Static Web Apps](https://learn.microsoft.com/en-us/azure/static-web-apps/overview)
- [GitHub Actions](https://docs.github.com/en/actions)

---

## 📌 To-Do / Roadmap

- [ ] Add authentication (Azure AD or Firebase for login)
- [ ] Add due dates and priorities to improve task organization
- [ ] Integrate a backend (e.g., Supabase or Firebase) for persistence
