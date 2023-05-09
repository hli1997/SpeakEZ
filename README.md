# Instructions

## Download

Download the package from GitHub

```shell
git clone https://github.com/coderaidershaun/chatbot-conversation-jarvis.git chatbot
```

## Setup backend

Change directory into backend

```shell
cd backend
```

### Setup virtual environment

Create and activate a Virtual Environment

```shell
python3 -m venv venv
source venv/bin/activate
```

Upgrade PIP

```shell
pip3 install --upgrade pip
```

### Install Python packages

Install required Python packages

```shell
pip3 install openai python-decouple fastapi "uvicorn[standard]" python-multipart
```

### Create Environment Variables

Create your .env file

```shell
touch .env
```

Update your .env file with the following. You can see your .env by typing sudo nano .env or just by clicking on the file if you are in VS Code.

```plain
OPEN_AI_ORG=enter-you-key-here
OPEN_AI_KEY=enter-you-key-here
ELEVEN_LABS_API_KEY=enter-you-key-here
```

### Start your backend server

Start your backend server

```shell
uvicorn main:app
```

Alternatively, you can ensure your server resets every time you make a change by typing:

```shell
uvicorn main:app -- reload
```

## Setup frontend

Change directory into frontend

```shell
cd ..
cd frontend
```

Install packages

```shell
yarn --exact
```

Build application

```shell
yarn build
```

Start server in dev mode

```shell
yarn dev
```

or alternatively in live mode:

```shell
yarn start
```
