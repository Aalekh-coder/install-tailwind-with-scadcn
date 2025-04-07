how to install the shadcn with vite js

1. npm create vite@latest
2. npm i -D tailwindcss@3 postcss autoprefixer 
3. npx tailwindcss init -p
4. @tailwind base; @tailwind components; @tailwind utilities;
5. in tailwind.config.js    
/** @type {import('tailwindcss').Config} */
export default {
  content: [
    "./index.html",
    "./src/**/*.{js,ts,jsx,tsx}",
  ],
  theme: {
    extend: {},
  },
  plugins: [],
}
6. create jsconfig.js
{
    "compilerOptions": {
      "baseUrl": ".",
      "paths": {
        "@/*": ["./src/*"]
      }
    }
  }

7. npm install -D @types/node
8. In vite.config.js
import { defineConfig } from 'vite'
import react from '@vitejs/plugin-react'
import path from "path"

// https://vite.dev/config/
export default defineConfig({
  plugins: [react()],
  resolve: {
    alias: {
      "@": path.resolve(__dirname, "./src"),
    },
  },
})

9. npx shadcn@latest init
# install-tailwind-with-scadcn
