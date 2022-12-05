# Fivem wiki 

## Prerequisites

* Docker (https://www.docker.com/)
* npm (https://www.npmjs.com/)

## Installation

Clone repository
```bash
mkdir /Fivem
cd /Fivem

git clone https://github.com/AlanDizaster/fivem.git
```

Configure environment
```bash
cp .env.examle .env
```

Run the Docker containers
```bash
docker compose up -d
```

Install the Composer dependencies (inside  the Docker `fivem_app` container)
```bash
composer install
```

Install the npm dependencies (outside the Docker container) and compile the assets
```bash
npm install
npm run build
```
