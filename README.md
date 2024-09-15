# TITANS GAME

## OVERVIEW
Parent repository for Titans Game project, intagreates the frontend and backend repos as git submodules (client, server)
I use rust for the backend and svelteKit framework for the frontend in order to increase efficiency by using lightweight framework, avoiding virtual DOM.
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
- **PostgreSQL**

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



