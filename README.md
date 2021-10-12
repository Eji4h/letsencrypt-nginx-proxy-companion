<h3 align="center">Let's encrypt nginx proxy companion Docker Compose</h3>

---

<p align="center"> Docker Compose for letsencrypt nginx proxy companion.
    <br> 
</p>

## 📝 Table of Contents

- [About](#about)
- [Prerequisites](#prerequisites)
- [Usage](#usage)
- [Authors](#authors)

## 🧐 About <a name = "about"></a>

This project for easy create letsencrypt nginx proxy companion.

## Prerequisites <a name="prerequisites"></a>

- docker and docker-compose cli is already install.

## 🎈 Usage <a name="usage"></a>

1. Clone Lets'Encrypt Nginx Proxy Companion Docker Compose

   ```shell
   git clone https://github.com/Eji4h/letsencrypt-nginx-proxy-companion
   cd letsencrypt-nginx-proxy-companion/
   ```

2. Start Lets'Encrypt Nginx Proxy Companion Docker Compose

   ```shell
   . create-docker-nginx-proxy-network.sh
   docker-compose up -d
   cd ..
   ```

3. Run Docker need to use let's encrypt nginx proxy with environments

   Example with <a href="https://github.com/Eji4h/rancher-compose">Rancher Docker Compose</a>

   - Change environment to your domain and email

   ```yaml
     ...
     rancher:
       image: rancher/rancher:v2.6.1
       ...
       environment:
         - VIRTUAL_HOST=<example.com>
         - LETSENCRYPT_HOST=<example.com>
         - LETSENCRYPT_EMAIL=<example@gmail.com>
       ...
   ```

---

## ✍️ Authors <a name = "Yosapol Jitrak"></a>

- [@Eji4h](https://github.com/Eji4h) - Initial work
