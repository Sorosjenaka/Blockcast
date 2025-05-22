# Blockcast 

Blockcast Depin Run with Vps

Please Follow my X : https://x.com/0xsoros

Thanks you for support me

## Step 1 
```bash
sudo apt update && sudo apt upgrade -y
```
## Step 2 Install Docker and Docker Compose
```
sudo apt install docker.io docker-compose -y
sudo systemctl enable docker
sudo systemctl start docker
```
## Step 3 Check version your docker
```
docker --version
docker compose version
```
## Step 4 Run Blockcast BEACON
```
git clone https://github.com/Blockcast/beacon-docker-compose.git
cd beacon-docker-compose
docker compose up -d
```
## Check your Docker
```
docker compose ps
```
## Allow port
```
sudo ufw allow 8443
sudo ufw allow 9190
```
## Restart and Run Docker
```
docker compose down
docker compose up -d
```
## Step 5 Regist your Node
```
docker compose exec blockcastd blockcastd init
```
## Out put will show up like this 
```
Hardware ID: c6ff0e6f-bc4d-4151-47c3-07df0e3cf53f
Challenge Key: MCowBQYDK2VwAyEAXP49l4pBK1V5qy7vbRJYv3etRdEr7ycsQAvrgS+hQY0=
Register URL: https://app.blockcast.network/register?hwid=...&challenge-key=...
```
## Copy your Hardware ID and Challenge Key
Go to website to register and put your Hardware ID and Challenge Key

Website : https://app.blockcast.network/dashboard

Wait Your node to online

## Check Your Logs
```
docker compose logs -f blockcastd
```


