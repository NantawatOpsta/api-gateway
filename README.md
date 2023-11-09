# Identity Provider Project

Test project learning how to use identity providers (keycloak) with microservices.

## start project

ตั้งค่า ENV ในไฟล์ .env ก่อน โดย

- สร้าง client บน keycloak แล้วใส่ค่า client_id และ client_secret ลงในไฟล์ .env

``` bash
# https://docs.docker.com/engine/install/
# run this command to start the project
KONG_DATABASE=postgres docker compose --profile database up -d
```

## All service

- Kong manager: <http://localhost:8002>
- UI: <http://localhost:8100>
- Service A: <http://localhost:8101>
- Serivce B: <http://localhost:8102>