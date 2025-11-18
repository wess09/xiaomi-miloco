# Notes for Deploying Miloco on Windows Subsystem for Linux (WSL)
## Before Deployment
1. Please install Docker directly in the WSL environment, do not use Docker Desktop
2. Ensure your Windows version is at least Windows 11 22H2, otherwise mirrored mode network cannot be used
3. Please deploy Miloco directly using the deployment script, manual installation is not required
## During Deployment
1. Please ensure Docker is installed. Note: Docker Compose V2 is required
2. The script will automatically install NVIDIA CUDA Toolkit, no manual installation needed
## After Deployment
1. Please set WSL network to mirrored mode network, otherwise the camera cannot be called normally
2. Turn off Windows Firewall or set inbound rules, otherwise the camera cannot be called normally
3. It is recommended to use cloud models for planning models, please do not set it to miloco-vl-7b