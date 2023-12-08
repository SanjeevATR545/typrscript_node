# typrscript_node
1. create a dir
2. npm init -y
3. install typescript
4. npx tsc --init    //create tsconfig file
5. npm i express mongodb mongoose cors dotenv cookie-parser
6. npm i -D typescript nodemon @types/node @types/express @types/mongodb @types/mongoose @types/cors @types/dotenv @types/cookie-parser //fordev dependencies

# changes in  tsconfig.json
"target": "ES2022"
"module": "NodeNext",  
 "outDir": "dist",     //change the compiled file folder
"sourceMap": true,    //uncomment it
       #add in last after the skipLibCheck #
"include": ["src/**/*"]   // add the source code dir in .ts

# package.json changes
    "build": "npx tsc",
    "start": "node server/dist/app.mjs",    //your build file
    "dev": "npx tsc -w & nodemon server/dist/app.mjs"  //your 
