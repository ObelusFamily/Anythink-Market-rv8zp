# Welcome to the Anythink Market repo

To start the app use Docker. It will start both frontend and backend, including all the relevant dependencies, and the db.

Please find more info about each part in the relevant Readme file ([frontend](frontend/readme.md) and [backend](backend/README.md)).

## Development

When implementing a new feature or fixing a bug, please create a new pull request against `main` from a feature/bug branch and add `@vanessa-cooper` as reviewer.

## First setup

1. Install [Docker](https://docs.docker.com/get-docker/)
2. Verify Docker was installed running `docker -v` and `docker-compose -v`
3. `cd` into your project root directory and run `docker-compose up`
4. Test the backend by pointing your browser to [http://localhost:3000/api/ping](http://localhost:3000/api/ping)
5. Now test the frontend by registering a new user here [http://localhost:3001/register](http://localhost:3001/register)
6. You're all done. If you want to run any command on the running container use `docker exec`

### Troubleshooting first setup

If you get the following error when running `docker-compose up`
`fork/exec /usr/local/bin/docker-compose-v1: bad CPU type in executable`
Follow the next steps:

1. Go to Docker settings.
2. Go to the "General" section.
3. Scroll down until you find the option "Use Docker Compose V2" and enable it.
4. Apply & Restart changes.
5. Try running `docker-compose up` again.
