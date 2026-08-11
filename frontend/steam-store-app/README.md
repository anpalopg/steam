# ⚡ Incident Management — Frontend ⚡

<div align="center">
  
![React](https://img.shields.io/badge/Version-Version?style=for-the-badge&logo=react&logoColor=blue&label=React&labelColor=Violet&color=Green)
  
![Docker](https://img.shields.io/badge/docker-%230db7ed.svg?style=for-the-badge&logo=docker&logoColor=white)

![TypeScript](https://img.shields.io/badge/Typescript-logo?style=for-the-badge&logo=typescript&logoColor=black&color=blue)

![Redux](https://img.shields.io/badge/Redux-logo?style=for-the-badge&logo=redux&logoColor=white&color=purple)

![npm](https://img.shields.io/badge/Version-Version?style=for-the-badge&logo=npm&logoColor=red&color=gold)



</div>

---

## 📋 Table of Contents

- 🎯 Description  
- ✨ Features  
- 🏗️ Architecture  
- 🛠️ Technologies  
- 📦 Requirements  
- 🚀 Installation and Execution  
- 🐳 Docker  
- ⚙️ Configuration  
- 📂 Project Structure  
- 🔌 API Communication  
- 🤝 Contributing  

---

## 🎯 Description


---

## ✨ Features

- Unified deployment as a single monolithic application
- Multiple functional modules integrated within the same codebase
- Shared global UI state managed with Redux
- API communication handled through Axios
- Extensible and scalable internal architecture
- Centralized routing and module organization
- Reusable and modular UI components
---

## 🏗️ Architecture




---

## 🛠️ Technologies

- **[React](https://react.dev/)** – Modern UI framework  
- **[Vite](https://vitejs.dev/)** – Lightning-fast bundler  
- **[Redux](https://redux.js.org/)** – Global state management  
- **[TypeScript](https://www.typescriptlang.org/)** – Typed JavaScript  
- **[Axios](https://axios-http.com/)** – HTTP client  
- **[Docker](https://www.docker.com/)** – Containerization  

---

## 📦 Requirements

- Node.js @latest  
- npm  
- Podman or Docker (optional)  

---

## 🌟 Installation and Execution

### 🔧 Method 1: Local Development

#### 1️⃣ Clone the repository
```bash

```

#### 2️⃣ Install dependencies

```bash
npm install
```

#### 3️⃣ Configure the backend URL

```bash
cp .env.example .env   # then edit VITE_API_URL if needed
```

#### 4️⃣ Run the dev server

```bash
npm run dev
```

🎉 **Done!** The frontend runs at `http://localhost:5173`

Other scripts:

```bash
npm run build            # production build -> dist/
npm run build:typecheck  # type-check then build
npm run lint             # ESLint
npm run preview          # preview the production build
```

---

### 🐳 Method 2: Docker / Podman

The image is multi-stage (node build → nginx serving on port 80). The backend
URL is baked in at build time via the `VITE_API_URL` build arg.

```bash

```

To run the whole stack (front + BFF + backend) use the compose file in the back
repo: `../incident-management-back/compose.yml`.

---

## ⚙️ Configuration

### Environment Variables

Copy `.env.example` to `.env` in `incident-management-app/`. The SPA reads a
single variable:

| Variable | Description | Default |
|----------|-------------|---------|
| `VITE_API_URL` | Base URL of the BFF service | `http://localhost:8080` |

`.env` file:

```
VITE_API_URL=http://localhost:8080
```

### Axios Setup

```

### Local Development



---

## 📂 Project Structure


---

## 🔌 API Communication


---

## 🤝 Contributing

Contributions are welcome! 🎉

1. 🍴 Fork the project
2. 🌿 Create a branch for your feature (`git checkout -b feature/AmazingFeature`)
3. 💾 Commit your changes (`git commit -m 'Add some AmazingFeature'`)
4. 📤 Push to the branch (`git push origin feature/AmazingFeature`)
5. 🔃 Open a Pull Request

---

## 📝 Code Conventions

- Use ESLint and Prettier
- Component names in PascalCase
- Hooks and functions in camelCase
- One component per file
- Keep components small and reusable
- Avoid inline CSS; prefer .css or styled-components
- Keep the order of coding

---

## 📄 License

This project is under the MIT License. See the `LICENSE` file for more details.

---

## 🙏 Acknowledgments
- **[React](https://react.dev/)**
- **[Vite](https://vitejs.dev/)**
- **[Axios](https://axios-http.com/)**
- **[TypeScript](https://www.typescriptlang.org/)**
- **[Redux](https://redux.js.org/)**
---
## 🔗 References
- [React Documentation](https://react.dev/)
- [Vite Documentation](https://vitejs.dev/)
- [Axios Documentation](https://axios-http.com/)
- [TypeScript Documentation](https://www.typescriptlang.org/)
- [Redux Documentation](https://redux.js.org/)
- [Markdown Live Preview](https://markdownlivepreview.com/)
---

<div align="center">

**⭐ If you like this project, give it a star on GitHub ⭐**

Made with ❤️ and ☕

</div>


