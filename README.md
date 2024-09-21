# TITANS GAME

## OVERVIEW
Parent repository for Titans Game project, integrates the frontend and backend repos as git submodules (client, server) <br />
I use rust for the backend (for obvious efficiency reasons) and svelteKit framework for the frontend in order to increase efficiency by using lightweight framework, avoiding virtual DOM. <br />
WORK IN PROGRESS.

## TECH STACK
### Client
- **Programming Language:** TypeScript
- **Framework:** SvelteKit
- **Styling:** TailwindCSS

### Server
- **Programming Language:** Rust
- **Dependencies** Actix Web, sqlx, serde, bcrypt, jsonwebtoken, chrono

## GETTING STARTED
## Prerequisites
- **Node.js**
- **Rust**
- **Docker Desktop**

1. Clone the parent repo
```
git clone https://github.com/your-username/titansGame.git
cd titansGame

# Initialize and update submodules
git submodule init
git submodule update

```

2. Setup Backend
```
## create and run docker container with postgres db
sudo docker pull mysql:latest
sudo docker run --name mysql_titansgame -e MYSQL_ROOT_PASSWORD=root -e MYSQL_USER=titans_game -e MYSQL_PASSWORD=titans_game -e MYSQL_DATABASE=titans_game_db -p 3306:3306 -v mysql_data:/var/lib/mysql -d mysql:latest

cd server

## ensure that rustup is installed
rustup -v

## start the server
cargo run

## server is available on port 8000
```

3. Setup Frontend
```
cd client

## install dependencies
npm install

## run the dev server
npm run dev

## client is available on port 5173
```



