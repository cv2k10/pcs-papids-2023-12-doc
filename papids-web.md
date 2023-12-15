## Project Title
# LRT3-PAPIDS Web (Front End)

## Demo link:
Access the site publicly at: (http://dev.pa-pids.com)

## Table of Content:

- [About The App](#about-the-app)
- [Screenshots](#screenshots)
- [Technologies](#technologies)
- [React App Setup](#react-app-setup)
- [Github CI/CD Setup](#github-cicd-setup)
- [Docker Setup](#docker-setup)
- [Unit Testing](#unit-testing)
- [Approach](#approach)
- [Status](#status)
- [Available Scripts](#available-scripts)
- [Credits](#credits)
- [License](#license)
- [Learn More](#learn-more)

## About The App
LRT3-PAPIDS Front End System is a react app that act as a main human interface for the operator and
maintenance personnel to control and operates both PA and PIDS modules in the system from OCC to LRT3 line.

This project was bootstrapped with [Create React App](https://github.com/facebook/create-react-app).

## Screenshots
![Sample of Station Control Tab](/station_control.jpg)

## Technologies
`html`, `css`, `scss`, `react.js`, `react redux`, `javascript`, `docker`, ` github ci/cd pipeline`, `react testing library`

## React App Setup
To get started follow this steps:

1. Install [Node](https://nodejs.org/download/release/v14.21.3/) version 14 or [yarn](https://yarnpkg.com/getting-started/install)
2. Download or clone the repository.
3. Open the project and install packages by running: ```npm i``` or ```npm install``` or ```yarn```.
4. Start project locally: ```npm start``` or ```yarn start``` (running on port 3000).
5. Make necessary changes.

Build app for production: ```npm run build``` or ```yarn build```.

## Github CI/CD Setup
Setup the CI/CD pipeline for build deployment by following these steps:
1. Create a folder in `C:\` called `pcs-lrt3-release` in the client.
2. Install `OpenSSH Client` and `OpenSSH Server` in the client.(https://learn.microsoft.com/en-us/windows-server/administration/openssh/openssh_install_firstuse?tabs=gui)
3. Set the IP to be a public domain in the router.
4. Set the SECRET KEYS with the right credentials.
5. Navigate tp Actions tab in ASL_Web repository.
6. Run the `build-folder-transfer-to-all-stations` action.


## Docker Setup
Setup the docker by following these steps:
1. Install Docker Desktop in the client. 
2. Clone ASL_Web_withDocker repository: (https://github.com/PCS-GIS-PAPIDS-Control-Software/ASL_Web_withDocker).
3. If you already created `pcs-lrt3-release` folder in `C:\`, change the path for `web-server` and `ping-server`in `docker-compose.yml` to the one in `C:\pcs-lrt3-release\pappids-[STATION-NAME]`. So the docker can always monitor the changes from our CI/CD deployment.
4. Run the ```docker compose up -d``` to install the docker container.

## Unit Testing
All files for unit testing is located in the `\src\utils\unitTest`: 
1. paApi.
2. pidsApi.
3. signalR.

Run `npm run test` to run all the test scripts or `npm run test -- [filename].js.test` to run a single file.

## Approach
- Adopted the `camelCase` naming convention for variable initialization.
- Adopted the `functional component` for React component.
- Adopted the `ES6` style for array mapping, filtering and function.

## Status
LRT3-PAPIDS Front End System is still in progress. Currently in `Version 2`.

## Available Scripts
In the project directory, you can run:

### `yarn start || npm start`

Runs the app in the development mode.<br />
Open [http://localhost:3000](http://localhost:3000) to view it in the browser.

The page will reload if you make edits.<br />
You will also see any lint errors in the console.

### `yarn test || npm test`

Launches the test runner in the interactive watch mode.<br />
See the section about [running tests](https://facebook.github.io/create-react-app/docs/running-tests) for more information.

### `yarn build || npm run build`

Builds the app for production to the `build` folder.<br />
It correctly bundles React in production mode and optimizes the build for the best performance.

The build is minified and the filenames include the hashes.<br />
Your app is ready to be deployed!

See the section about [deployment](https://facebook.github.io/create-react-app/docs/deployment) for more information.

### `yarn eject || npm run eject`

**Note: this is a one-way operation. Once you `eject`, you can’t go back!**

If you aren’t satisfied with the build tool and configuration choices, you can `eject` at any time. This command will remove the single build dependency from your project.

Instead, it will copy all the configuration files and the transitive dependencies (webpack, Babel, ESLint, etc) right into your project so you have full control over them. All of the commands except `eject` will still work, but they will point to the copied scripts so you can tweak them. At this point you’re on your own.

You don’t have to ever use `eject`. The curated feature set is suitable for small and middle deployments, and you shouldn’t feel obligated to use this feature. However we understand that this tool wouldn’t be useful if you couldn’t customize it when you are ready for it.

## Credits
List of contriubutors:
- [Calvin](https://github.com/cv2k10)
- [Kimberly](https://github.com/Kimberry0722)
- [Umair](https://github.com/umair832)

## License
MIT license @ [author](author.com)

## Learn More
You can learn more in the [Create React App documentation](https://facebook.github.io/create-react-app/docs/getting-started).

To learn React, check out the [React documentation](https://reactjs.org/).

# Code Splitting
This section has moved here: https://facebook.github.io/create-react-app/docs/code-splitting

# Analyzing the Bundle Size
This section has moved here: https://facebook.github.io/create-react-app/docs/analyzing-the-bundle-size

# Making a Progressive Web App
This section has moved here: https://facebook.github.io/create-react-app/docs/making-a-progressive-web-app

# Advanced Configuration
This section has moved here: https://facebook.github.io/create-react-app/docs/advanced-configuration

# Deployment
This section has moved here: https://facebook.github.io/create-react-app/docs/deployment

# `yarn build` fails to minify
This section has moved here: https://facebook.github.io/create-react-app/docs/troubleshooting#npm-run-build-fails-to-minify






