### <h1 align="center"  id="heading">Create Multiple Environments In React</h1>
## .env files
```
 .env.development
 .env.staging 
 .env.production 
```
## package.json
```json
"scripts": {
    "start": "env-cmd -f .env.development react-scripts start",
    "start:staging": "env-cmd -f .env.staging react-scripts start",
    "start:production": "env-cmd -f .env.production react-scripts start",
    "build": "env-cmd -f .env.development react-scripts build",
    "build:staging": "env-cmd -f .env.staging react-scripts build",
    "build:production": "env-cmd -f .env.production react-scripts build",
    "test": "react-scripts test",
    "eject": "react-scripts eject"
},
```
## development
```bash
npm start
npm build
```

## staging
```bash
npm run start:staging
npm run build:staging
```

## production
```bash
npm run start:production
npm run build:production
``` 