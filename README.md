ezin-exchange/
├─ package.json
├─ vite.config.js
├─ tailwind.config.js
├─ postcss.config.js
├─ src/
│   ├─ main.jsx
│   ├─ index.css
│   └─ EZINExchange.jsx
└─ public/
    └─ favicon.ico
    {
  "name": "ezin-exchange",
  "version": "1.0.0",
  "scripts": {
    "dev": "vite",
    "build": "vite build",
    "preview": "vite preview"
  },
  "dependencies": {
    "framer-motion": "^10.12.16",
    "react": "^18.2.0",
    "react-dom": "^18.2.0",
    "@radix-ui/react-select": "^1.0.0",
    "tailwindcss": "^3.3.3",
    "autoprefixer": "^10.4.14",
    "postcss": "^8.4.24"
  },
  "devDependencies": {
    "@vitejs/plugin-react": "^4.0.0",
    "vite": "^5.0.0"
  }
}
import { defineConfig } from 'vite';
import react from '@vitejs/plugin-react';
export default defineConfig({ plugins: [react()] });
export default {
  content: ["./index.html", "./src/**/*.{js,jsx}"],
  theme: { extend: {} },
  plugins: [],
}
export default { plugins: { tailwindcss: {}, autoprefixer: {}, }, }
import React from "react";
import ReactDOM from "react-dom/client";
import EZINExchange from "./EZINExchange";
import "./index.css";
ReactDOM.createRoot(document.getElementById("root")).render(<React.StrictMode><EZINExchange /></React.StrictMode>);
@tailwind base;
@tailwind components;
@tailwind utilities;
