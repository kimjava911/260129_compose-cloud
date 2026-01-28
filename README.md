```sh
chmod 400 *.pem
ssh -i "*.pem" ubuntu@ec2-*-*-*-*.ap-northeast-2.compute.amazonaws.com
```

```sh
git clone <저장소 주소>
# git clone https://github.com/kimjava911/260129_compose-cloud.git
```

```sh
export CR_PAT=ghp_******
echo $CR_PAT | docker login ghcr.io -u <username> --password-stdin
```

```sh
docker pull ghcr.io/NAMESPACE/cloud-compose-spring:latest
docker tag ghcr.io/NAMESPACE/cloud-compose-spring:latest cloud-compose-spring:latest
vi .env # 환경변수 주입
docker compose up -d
```
