# Dockerized Jenkins

## Installation
[Before you start, Run step 1 to 3](https://www.jenkins.io/doc/book/installing/docker/#on-macos-and-linux).
Then continue below steps to install:

### 1. Build docker image
```bash
docker build -t myjenkins-blueocean:2.332.3-1 .
```

### 2. Run in Compose file
```bash
docker compose up -d
```

### 3. Run in browser
- For example open [`http://localhost:8080`](`http://localhost:8080`)
- Create your Jenkins account
- Choose recommended plugins
- You are done

## Runing CLI (Optional with http connection)
Change parameter to your configuration
```bash
java -jar jenkins-cli.jar -s <url> -auth <username>:<password> help
```

## Additional Tool
1. Ngrok (Forwarding port 8080)

# Jenkins Plugins
1. Generic Webhook Trigger
2. NodeJS