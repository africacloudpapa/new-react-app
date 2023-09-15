# Deploy React App to Server

This project teaches how to deploy a react application to server (AWS, GCP, AZURE, DIGITAL OCEAN, VPS)

## Node and npm installation

```

sudo apt-get update
sudo apt-get install -y ca-certificates curl gnupg
sudo mkdir -p /etc/apt/keyrings
curl -fsSL https://deb.nodesource.com/gpgkey/nodesource-repo.gpg.key | sudo gpg --dearmor -o /etc/apt/keyrings/nodesource.gpg
NODE_MAJOR=20
echo "deb [signed-by=/etc/apt/keyrings/nodesource.gpg] https://deb.nodesource.com/node_$NODE_MAJOR.x nodistro main" | sudo tee /etc/apt/sources.list.d/nodesource.list
sudo apt-get update
sudo apt-get install nodejs -y

```

## Clone the repository

```
git clone https://github.com/africacloudpapa/new-react-app.git

```

## Change to new-react-app folder

```
cd new-react-app

```

## Install packages

```
npm install

```

## Build the application

```
npm run build

```

## install nginx

```
sudo apt install nginx -y

```

## Copy the build file to nginx html folder

```
sudo cp -r build/* /var/www/html

```
