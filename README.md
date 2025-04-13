1. npm create vite@latest
2. npm i -D tailwindcss@3 postcss autoprefixer
3. npx tailwind init -p
4. @tailwind base; @tailwind components; @tailwind utilites;
5. content: ["./index.html", "./src/**/.{js,ts,jsx,tsx}", ],
6. create jsonfig.json:  {
    "compilerOptions": {
      "baseUrl": ".",
      "paths": {
        "@/*": ["./src/*"]
      }
    }
  }

7. npm i -D @types/node
8. in viteConfig:
  resolve: {
    alias: {
      "@": path.resolve(__dirname, "./src"),
    },
  },

9. npx shadcn@latest init
