# Final Assessment Projects

# Update system
sudo apt update && sudo apt upgrade -y

# Install common tools
sudo apt install -y curl wget git vim unzip htop net-tools software-properties-common

# Install Docker
curl -fsSL https://get.docker.com | sh
sudo usermod -aG docker $USER

# Install Docker Compose
sudo apt install -y docker-compose-plugin

# Install Nomad
curl -fsSL https://releases.hashicorp.com/nomad/1.8.0/nomad_1.8.0_linux_amd64.zip -o nomad.zip
unzip nomad.zip && sudo mv nomad /usr/local/bin/ && rm nomad.zip

# Install Loki + Promtail later via Docker
# Install Minikube + kubectl (optional if you want Kubernetes)
