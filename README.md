# TITANS GAME

## OVERVIEW
Parent repository for Titans Game project, integrates the frontend and backend repos as git submodules (client, server) <br />
I use rust for the backend and svelteKit framework for the frontend in order to increase efficiency by using lightweight framework, avoiding virtual DOM. <br />
Project will be a web-based game, developed following TDD rules both on backend and frontend.
WORK IN PROGRESS.

## TECH STACK
### Client
- **Programming Language:** TypeScript
- **Framework:** SvelteKit
- **Testing:** Vitest, Playwright, Svelte Testing Library

### Server
- **Programming Language:** Rust
- **Framework:** Actix Web
- **Testing:** Rust's built-in testing framework

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
docker pull mysql:latest
docker run --name mysql_titansgame -e MYSQL_ROOT_PASSWORD=root -e MYSQL_USER=titans_game -e MYSQL_PASSWORD=titans_game -e MYSQL_DATABASE=titans_game_db -p 3306:3306 -v mysql_data:/var/lib/mysql -d mysql:latest

cd server

## ensure that rustup is installed
rustup -v

## ensure all tests pass
cargo test

## start the server
cargo run

## server is available on port 8000
```

3. Setup Frontend
```
cd client

## install dependencies
npm install

## ensure all tests pass
npm run test:unit
npm run test:e2e

## run the dev server
npm run dev

## client is available on port 5173
```



