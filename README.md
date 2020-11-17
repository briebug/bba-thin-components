# Thin Components Example

This is an example demonstrating how we can use proper abstractions to manipulate space and time with thin components.


![image](https://user-images.githubusercontent.com/1544557/38834610-cbb84af6-417d-11e8-9cb6-64c3a364af6b.png)


## Prerequisites

- [Git](https://git-scm.com/book/en/v2/Getting-Started-Installing-Git)
- Node.js and NPM – we recommend using [NVM (Linux/Mac)](https://github.com/creationix/nvm) or [NVM-Windows (Windows)](https://github.com/coreybutler/nvm-windows)
- Install Angular CLI via `npm i -g @angular/cli`

## Web: Getting Started

```
git clone https://github.com/onehungrymind/bba-thin-components.git
cd bba-thin-components
yarn
yarn serve:all
```
The client application will open to [http://localhost:4200](http://localhost:4200) in your browser.

The `serve:all` command is a convenience methods that runs multiple commands concurrently. You can run each command separately if you need to.

```
"start": "ng serve",
"serve:socketio": "node ./server/server.js",
"serve:json": "json-server server/db.json --port 3100 --watch",
"serve:api": "nx run api:serve",
"serve:client": "nx run client:serve --open",
"serve:all": "concurrently \"npm run serve:socketio\" \"npm run serve:api\" \"npm run serve:client\"",
```

> Note: the above terminal commands are for Mac. Remember to substitute the appropriate commands for your OS.
