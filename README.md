# 🚀 End-to-End DevOps CI/CD Pipeline Project

Bu proje; **Python (Flask)** tabanlı bir web uygulamasının **Docker** ile konteynerize edilmesini, **Nginx** reverse proxy arkasında çalıştırılmasını ve **GitHub Actions** kullanılarak otomatik test (`pytest`) ve imaj dağıtım (**GHCR**) süreçlerinin uçtan uca otomatize edilmesini içerir.

## 🏗️ Mimari Yapı

* **Uygulama Katmanı:** Python 3.12 & Flask
* **Reverse Proxy:** Nginx (`Port 80 -> 5000` yönlendirmesi)
* **Konteynerizasyon:** Docker & Docker Compose
* **CI/CD Otomasyonu:** GitHub Actions (`push -> pytest -> Docker Build -> GHCR Push`)

## 🛠️ Yerel Ortamda Çalıştırma

Projeyi kendi bilgisayarınızda ayağa kaldırmak için:

```bash
git clone [https://github.com/Emrullahuran/devops-cicd-project.git](https://github.com/Emrullahuran/devops-cicd-project.git)
cd devops-cicd-project
docker compose up --build -d