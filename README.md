# GVM

- [x] get vue cli and setup front end
- [x] wire it up to the backend with gorilla mux
- [ ] maybe get 'fresh' setup to rebuild js and go code on change for frontend/backend hot code reloading
- [ ] get the database and go-migrate setup
- [ ] figure out authentication
- [ ] add CRUD for the resources
- [ ] add front end testing (maybe cypress?)

## Project setup
This project was built with go 1.14.3 , @vue/cli 4.5.9 , mysql and golang-migrate

On a mac, you can use homebrew to install most of the requirements, if not get these required packages:
- [golang](https://golang.org/dl/) 
- [mysql](https://dev.mysql.com/downloads/mysql/)
- [node & npm](https://nodejs.org/en/download/)
- [golang-migrate](https://github.com/golang-migrate/migrate/tree/master/cmd/migrate)

create a database to use for the project

```
$ git clone https://github.com/sliceking/gvm.git
$ npm install
$ npm run build
$ go get
$ migrate -database 'mysql://user:password@tcp(localhost)/database'  -path db/migrations up
$ go run main.go
```

### Compiles and hot-reloads for js development
```
npm run serve
```

### Compiles and minifies js for production
```
npm run build
```

### Lints and fixes files
```
npm run lint
```

### Customize configuration
See [Configuration Reference](https://cli.vuejs.org/config/).
