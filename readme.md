Node-Red + MongoDB in Docker

Quick Start:

- Install Docker using install for your OS
- Clone this repo
- Run `docker-compose up` in the repo root
- Access node-red admin dashboard at http://127.0.0.1:1880/admin

Default Configuration:

- The node-red admin dashboard is served from /admin by default
- Configuration files and flows are saved in the data folder
- Files added to the public folder are served from the root directory /
- Node Red Dashboard and MongoDB nodes are installed by default
- The MongoDB server is available on port 27017

Adding NPM Modules:

- Edit Dockerfile RUN command and append npm modules required
- Modify settings.js to enable global npm modules in red
- Run `docker-compose up --force-recreate --build`