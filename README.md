# vite-configure

- Install vite With Yarn:
    $ yarn create vite
    write project name
    select language
    select framework

- yarn install
- yarn dev <!-- for run project -->

- Configure file structure

- Configure route
  On tsconfig.json file : 

  "baseUrl": "./src/",
    "paths" : {
      "#components/*" : ["./components/*"],
    }

  On vite.config.ts file :

  import { defineConfig } from "vite";
  <!-- into defineConfig function -->
  resolve: {
    alias: {
      "#assets": resolve(__dirname, "./src/assets/"),
    },
  },

