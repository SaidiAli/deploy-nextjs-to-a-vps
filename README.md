# Deploy Nextjs Project to a VPS
This file has instructions to deploy a nextjs project to a VPS. The VPS can be acquired from any vendor (Contabo, Digital ocean, hostinger ...)
## Instructions
1. After puchasing the VPS, connect to it using SSH by ``` ssh root@<ip-address> ```
2. Create a new user (if needed): ``` adduser <user-name>```
3. Add new user to super user do(sudo) group: ```usermod -aG sudo <new-user>```
4. Swith current user from root to the newly created user: ```sudo su - <new-user>```
5. Update packages: ```sudo apt update```
6. Upgrade packages: ```sudo apt upgrade```
7. Intall latest NodeJs: Follow instructions at [Link](https://www.digitalocean.com/community/tutorials/how-to-install-node-js-with-nvm-node-version-manager-on-a-vps)
8. Install pm2 for running process: ```npm install pm2 -g```
9. Install github action runners for CI/CD (Setup CI/CD)
10. git clone the project onto the VPS
