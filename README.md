# 🐋 AWS CLI & Kubectl 이미지

> AWS CLI와 Kubectl이 통합된 Docker 이미지입니다.

---

## ✨ 주요 기능

- ☁️ **AWS CLI v2** 포함 (aws 명령어)
- ☁️ **Kubectl** 포함 (kubectl 명령어)
- 🖥️ `/bin/sh` 기본 쉘 환경  

---

## 🛠️ 설치 및 사용법

### 1. 이미지 풀 (Pull)
```
docker pull mupersei/awscli-kubectl:latest
```

### 2. 이미지 빌드 및 푸시
```
docker buildx build --platform linux/amd64,linux/arm64 --build-arg KUBECTL_VERSION=<Kubernetes Version> -t mupersei/awscli-kubectl:latest  --push .
```
