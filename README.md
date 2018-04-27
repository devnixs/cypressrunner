# Cypress Runner

Simple image to run cypress tests

## How to use

`docker run --name="cypressrunner" -e CYPRESS_KEY=XXXX -e CYPRESS_BASE_URL="http://.../" -v ./cypress.json:/runner/cypress.json -v ./cypress:/runner/cypress raphaelareya/cypressrunner`

To check the result

`docker inspect cypressrunner --format='{{.State.ExitCode}}'`