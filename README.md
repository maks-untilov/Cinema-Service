# 🎥cinema-app🎥
This is simple simulation of cinema service for reservation tickets for user and do some administration things for management. Also that supports registration, authentication and CRUD operations
## ✍️ Detailed description of the project
- CRUD operations for Movie, Cinema Hall, Movie Session, Order, Shopping Cart, User
- Control classes distributed by package (Dao, Service, Dto, Model etc.)
- Implemented authetication with registration and login operations
- Validation passwords and emails
- Relation between models(User -> Shopping cart)
- Roles for user
## 📝 Structure of the project
- Config. All configuration classes
- Controller. The conductor of operations for a request
- Dao. Relation between Project and DB
- Dto. Objects from requsts or for response
- Exception
- Lib. For annotations and validations
- Models
- Util
## 🎯 Features
- Login and registration
- Create and find movie
- Create and find available movie session
- Creating and clear shopping cart 
- Completing order and get order history
- Adding roles to user
- Validation during registration
- Dto to all models
## 🛠 Tools
- Spring WEB
- Spring Security
- Hibernate
- Javax Validation
- GlobalException
## ⚡️ Quickstart
Change to your db parametrs (In db properties)
```
db.driver=YOUR_DRIVER
db.url=YOUR_URL
db.user=YOUR_USERNAME
db.password=YOUR_PASSWORD
```
You can add your in-memory user
```
auth.inMemoryAuthentication()
                .passwordEncoder(passwordEncoder)
                .withUser("user@i.ua").password(passwordEncoder.encode("user123")).roles("USER")
```
