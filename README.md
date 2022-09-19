# 📌 I. Front End 
### ✅ Step 1: Install Dependency Packages
- [x] cd /front
>  npm install **or** npm i 

### ✅ Step 2: Update Environment Variables
- [x] Update env.production and env.development with IP Address of your Backend server

#### ⛔ Example for production  file:
```
VUE_APP_MODE=production
VUE_APP_API_URL=http://localhost:8000/api
```

#### ⛔ Example for developement file:
```
VUE_APP_MODE=development
VUE_APP_API_URL=http://localhost:8000/api
```
### ✅ Step 3: Running Application
- [x] If you are in the development environment (Compiles and hot-reloads for development)
> npm run serve  (Normal Vue JS)

> npm run dev  (Vue + Vite)
- [x] If you are in the production environment (Compiles and minifies for production)
  
📍 Normal Vue JS:
> npm run build 

📍📍 Vue + Vite: 
> npm run build 

>  npm run preview 

📍📍📍 Both after build
  
> npm install --global serve 

>  serve -s dist 


# 📌 II. Backend 
### ✅ Step 1: Install the Packages
- [x] cd /back
>  composer install **or** composer i 

### ✅ Step 2: Update the Environment Variables
- [x] copy **.env.example**  file **to** the **.env**  file
  
```
DB_DATABASE= YOUR_DB_NAME  ✏️
DB_USERNAME= YOUR_DB_USERNAME ✏️
DB_PASSWORD= YOUR_DB_PASSWORD ✏️
```
### ✅ Step 3: Generate Application Key
>  php artisan key:generate 

### ✅ Step 4: Migrate migrateion table to database
>  php artisan migrate 

### ✅ Step 5: Migrate default admin user to database with seeder
>  php artisan db:seed 

### ✅ Step 6: Running Application
- [x] If you are in local development environments
>  php artisan serve  --port=YOUR_PORT (port is optional) 

- [x] If you are in production environments

>  http:://YOUR_IP_ADDRESS/PROJECT/back/public 

- [x] If you are configured VHOST  environment variable  with Apache configuration point to public folder in project so you can type:
>  http:://YOUR_IP_ADDRESS 

