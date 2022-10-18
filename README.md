# MLH Prep Project

Over the next 2 weeks, you'll be building a React App that works with various APIs (Application Programming Interfaces) that talk to different data sources to do cool stuff.

We're using the [OpenWeather API](https://openweathermap.org/current) to get weather data on different cities. Your challenge over the next 2 weeks is to build out this website and add even more functionality to it. At the moment, it displays basic information about a location when you type it in. Check out [Issues](/issues) for some more ideas!

You'll need to get your own API Key from their website (for free) and add it as an environment variable in a `.env` file. We have a template available as `example.env`.

You'll be using React initially to build this. If you're new to React, check out the [website](https://reactjs.org) for some information on getting started! 

## Project Setup

Follow the steps below to setup the project on your local machine according to the operating system you are using.

### Windows
#### Using npm
- `Step 1`: Install Node.js and npm

_You can skip this step if you have node installed on your system._

Open the link below to install Node.js and npm on your system.

https://nodejs.org/en/download/

- `Step 2`: Install all the dependencies

```bash
npm install
```

- `Step 3`: Start the server.

```bash
npm start
```

You can view your project at `http://localhost:3000/`.

#### Using yarn
- `Step 1`: Install Node.js and npm

_You can skip this step if you have node installed on your system._

Open the link below to install Node.js and npm on your system.

https://nodejs.org/en/download/

- `Step 2`: Install yarn

_You can skip this if you have the yarn installed on your system. Make sure it is the latest stable version._

Run the following command in Powershell.

```bash
npm install --global yarn
```

- `Step 3`: Install the dependencies

```bash
yarn install
```
or simply

```bash
yarn 
```

_Note_: The **yarn.lock** may cause issues with the installation of dependencies. If you face this issue, try deleting the **yarn.lock** file and repeat the command above.

- `Step 4`: Start the server

```bash
yarn start
```
### Linux
#### Using npm

- `Step 1`: Install the Curl Command-Line Tool

_You can skip this step if you have curl installed on your system._

```bash
sudo apt install curl
```

- `Step 2`: Install Node.js and npm

_You can skip this step if you have node installed on your system. Make sure it is the latest stable version._

Open the link below to install Node.js and npm for your specific distribution.

https://github.com/nodesource/distributions/blob/master/README.md

- `Step 3`: Install all the dependencies

```bash
npm install
```

- `Step 4`: Start the server.

```bash
npm start
```

You can view your project at `http://localhost:3000/`.

#### Using yarn
- `Step 1`: Install the Curl Command-Line Tool

_You can skip this step if you have curl installed on your system._

```bash
sudo apt install curl
```

- `Step 2`: Install Node.js and npm

_You can skip this step if you have node installed on your system. Make sure it is the latest stable version._

Open the link below to install Node.js and npm for your specific distribution.

https://github.com/nodesource/distributions/blob/master/README.md

- `Step 3`: Install yarn

_You can skip this if you have the yarn installed on your system. Make sure it is the latest stable version._

```bash
npm install --global yarn
```

- `Step 4`: Install the dependencies

```bash
yarn install
```
or simply

```bash
yarn 
```

- `Step 5`: Start the server

```bash
yarn start
```
### Docker Development Environment

`!!! Have your environment file ready before running the container !!!` <br>


This project contains 2 Dockerfiles := `Dockerfile.dev` and `Dockerfile.prod` for development and production environment respectively.

These 2 enviroments are :-
1. <b>react-dev</b> := For running the app in development setting 
2. <b>react-prod</b> := For running on production ecosystem.

In order to run them simply choose from one of the above and replace them for `env-name`
  
```console
$ docker-compose up <env-name>
```
Both of these environment would be live at **localhost:3000**

#### Make Your Own Image
To make your own image, choose from any of the above mentioned Dockerfile and simply run 
```console
$ docker build -t <image_name> -f <dockerfile_name> .
```

## Environment Variables

Create a `.env` file to insert your api keys. _You can refer to the `example.env` format for more information._

#### Weather API

To generate an API key, follow the instructions below:

- Click on this [link](https://openweathermap.org/) to access the website.
- Sign in or Create a new account.
- Navigate to the user account and click on **API keys** or **My API keys**.

Copy the API key and paste it in your `.env` file and replace `Your_Api_Key` with the API key generated

```
REACT_APP_APIKEY=Your_Api_Key
```
