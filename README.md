# This will have details of the project.

## start with understanding the folder structure

smartfarm/

backend/
frontend/
README.md



backend/
├── src/
│   ├── index.js          # Entry point
│   ├── db.js             # DB connection
│   ├── routes/
│   │   ├── auth.js
│   │   ├── fields.js
│   │   └── updates.js
│   ├── middleware/
│   │   └── auth.js       # JWT verification + role check
│   └── controllers/
│       ├── authController.js
│       ├── fieldController.js
│       └── updateController.js
├── .env
└── package.json



## process

- created the project 'smartfarm' on my github and cloned it on my local.
- created the backend folder
- couldn't install dependencies, npm not found, node not installed
- installed node (brew install node) v25.9.0
- installed dependencies (npm install express pg jsonwebtoken bcryptjs dotenv cors
npm install --save-dev nodemon)
Here's what each package does:
    express — web framework
    pg — PostgreSQL client
    jsonwebtoken — for JWT auth tokens
    bcryptjs — for hashing passwords
    dotenv — for environment variables
    cors — to allow the React frontend to talk to the backend
    nodemon — auto-restarts server on file changes during development

    --save-dev — this flag tells npm that nodemon is a development-only dependency. Meaning it's a tool you only need while building/developing the app, not when the app runs in production. npm saves it under "devDependencies" in your package.json instead of "dependencies".
    
- I forgot to initialize a node.js project in the backend folder (npm init -y). This is to be run before installing the dependices.



