# Jholok

## Run on a New Machine

# 1. Clone the project
cd ~/Documents
git clone git@github.com:shamirtowsif/jholok.git
cd jholok

# 2. Update system
sudo pacman -Syu
reboot

# 3. Install Docker & Docker Compose
sudo pacman -S docker docker-compose

# 4. Enable and start Docker
sudo systemctl enable docker
sudo systemctl start docker

# 5. Allow Docker without sudo
sudo usermod -aG docker $USER
reboot

# 6. Build containers
docker compose build

# 7. Run the project
docker compose up

# Stop
# Ctrl + C
