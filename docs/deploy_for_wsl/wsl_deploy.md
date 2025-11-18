# 在适用于 Linux 的 Windows 子系统（WSL）上部署 Miloco 的一些注意事项
## 部署前
1. 请直接使用 WSL 环境安装 Docker 不要使用 Docker Desktop
2. 请确保 Windows 版本大于等于 Windows 11 22H2 否则不能使用镜像模式网络
3. 请直接使用部署脚本部署 Miloco 不需要手动安装
## 部署中
1. 请确保已经安装了 Docker 注意：需要支持Docker Compose V2
2. 脚本会自动安装 NVIDIA CUDA Toolkit 不需要手动安装
## 部署后
1. 请设置 WSL 网络为 镜像模式网络 否则摄像头无法正常调用
2. 关闭 Windows 防火墙或设置入站规则 否则摄像头无法正常调用
3. 规划模型推荐使用 云端模型 请不要设置为 miloco-vl-7b