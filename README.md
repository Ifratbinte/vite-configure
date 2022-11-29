# vite-configure

- Install vite With Yarn:
<br>  
    $ yarn create vite <br>
    write project name <br>
    select language <br>
    select framework <br> <br>

- yarn install <br>
- yarn dev <!-- for run project --> <br> <br>

- Configure file structure <br> <br>

- Configure route <br>
  On tsconfig.json file :  <br>

  "baseUrl": "./src/", <br>
    "paths" : { <br>
      "#components/*" : ["./components/*"], <br>
    } <br> <br>

  On vite.config.ts file : <br> <br>

  import { defineConfig } from "vite"; <br>
  <!-- into defineConfig function --> <br>
  resolve: { <br>
    alias: { <br>
      "#assets": resolve(__dirname, "./src/assets/"), <br>
    }, <br>
  }, <br>

