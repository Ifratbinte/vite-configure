# vite-configure

- Install vite With Yarn: <br>
    $ yarn create vite <br>
    write project name <br>
    select language <br>
    select framework <br> <br>

- yarn install <br>
- yarn dev <br> 
- Configure file structure <br> 
- Configure route <br>
  On <b>tsconfig.json</b> file :  <br>

  "baseUrl": "./src/", <br>
    "paths" : { <br>
      "#components/*" : ["./components/*"], <br>
    } <br> 

  On <b>vite.config.ts</b> file : <br />

  import { defineConfig } from "vite"; <br>
  resolve: { <br>
    alias: { <br>
      "#components": resolve(__dirname, "./src/components/"), <br>
    }, <br>
  }, <br>

