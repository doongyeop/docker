# 1. Docker 기본 개념

## ✅ Docker란? 
> **컨테이너(Container)** 기술을 이용하여 각각의 프로그램을 **분리된 환경**에서 실행 및 관리할 수 있는 **오픈소스 플랫폼**.



## ✅ Container란?
> 애플리케이션과 그 실행에 필요한 모든 것을 포함하는 **격리된 실행 환경**

###  특징
-  **경량화**: 가상머신보다 훨씬 가볍고 빠름  
-  **격리성**: 각 컨테이너는 서로 영향을 주지 않음  
-  **이동성**: 환경에 구애받지 않고 어디서나 실행 가능  
-  **독립성**  
    - **파일 시스템**: 각 컨테이너는 독립된 저장 공간을 가짐  
    - **네트워크**: 컨테이너마다 고유한 IP와 Port 설정 가능  
    - **프로세스**: 외부에서 접근할 수 없는 내부 전용 프로세스 → **보안성↑**


## ✅ Host Computer

```
[호스트 컴퓨터 (Host OS)]
　　└─ Docker Engine
　　　　　├─ 컨테이너 1
　　　　　├─ 컨테이너 2
　　　　　└─ 컨테이너 3
```

-  **호스트 OS**: Docker가 설치된 운영체제 (ex. Ubuntu, macOS, Windows 등)  
-  **Docker Engine**: 컨테이너를 생성하고 관리하는 소프트웨어  
-  **컨테이너**: 각각의 독립된 실행 환경. 실제 자원은 호스트에서 빌려서 사용


## ✅ Image란?
> **컨테이너 실행을 위한 설정 파일 및 실행 파일이 포함된 템플릿**

### 📌 특징
- 컨테이너는 **이미지를 기반으로 생성**
- 한 번 만든 이미지는 **재사용 및 공유 가능** (ex. Docker Hub)
- 여러 계층(Layer)으로 구성되어 있어 변경된 부분만 저장 → **효율적인 버전 관리**

## 결론
>  이미지: 실행되지 않은 **정적 템플릿**  
>  컨테이너: 이미지를 기반으로 실행된 **동적 인스턴스**


