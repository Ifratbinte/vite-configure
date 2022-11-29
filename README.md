# vite-configure

- Install vite With Yarn:
    $ yarn create vite <br>
    write project name <br>
    select language <br>
    select framework <br> <br>

- yarn install <br>
- yarn dev <br> 

- Configure file structure <br> 

- Configure route <br>
  On tsconfig.json file :  <br>

  "baseUrl": "./src/", <br>
    "paths" : { <br>
      "#components/*" : ["./components/*"], <br>
    } <br> 

  On vite.config.ts file : <br>

  import { defineConfig } from "vite"; <br>
  resolve: { <br>
    alias: { <br>
      "#assets": resolve(__dirname, "./src/assets/"), <br>
    }, <br>
  }, <br>

