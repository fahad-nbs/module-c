# module-c

##link module-c (checkout component) to module-a (shop-rework/broadcast)
1. install `npm install -g @vue/cli`
2. then in module-c console type `vue-cli-service build --target lib --name module-c ./src/components/index.js`
3. created index.js file in src/components where I have exported all components
4. then type `npm link`
5. then in module-a type `npm link module-c`
6. in module-a type npm i module-c
7. it will install package in node-modules
8. and you can import components from there
9. now run your main project `npm run serve`
10. now if you will change something in module-c component and save it then changes will be appeared in module-a

We can start both projects seperatly too. 
or even start main project only it will work due to our installed module-c package in node-modules

module-a link: https://github.com/fahad-nbs/module-a

reference: https://javascript.plainenglish.io/how-to-create-test-bundle-vue-components-library-8c4828ab7b00

## Project setup
```
npm install
```

### Compiles and hot-reloads for development
```
npm run serve
```

### Compiles and minifies for production
```
npm run build
```

### Customize configuration
See [Configuration Reference](https://cli.vuejs.org/config/).
