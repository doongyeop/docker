# 1. Docker 기본 개념

## Why Docker?

### ㄱ. 이식성 (Portability)
#### 1. 복잡한 설치 과정 생략
> 필요한 프로그램을 설치할 때, 복잡한 의존성이나 환경 설정을 직접 처리하지 않아도 됨. Docker 이미지를 통해 손쉽게 동일한 환경을 복제할 수 있음.
#### 2. 일관된 환경 보장
> 개발, 테스트, 운영 환경이 동일한 Docker 이미지를 기반으로 실행되기 때문에, 버전 차이나 설정 오류로 인한 문제가 줄어듬. (예: OS, 라이브러리 버전, 설정 파일 등)
#### 3. 충돌 방지
> 각 애플리케이션이 독립적인 컨테이너에서 실행되므로, 서로 다른 프로그램 간의 충돌이나 간섭 없이 안정적으로 운용할 수 있음

### ㄴ. 경량성 (Lightweight)
1. 전통적인 가상 머신(VM)보다 훨씬 가벼움.
2. OS 전체를 올리지 않고 필요한 애플리케이션과 의존성만 포함하므로 빠르게 실행됨

### ㄷ. 빠른 배포 및 실행 속도
1. 컨테이너는 몇 초 만에 실행될 수 있어, 배포 속도가 빨라짐.
2. CI/CD 파이프라인에 최적화 되어있음.

### ㄹ. 버전 관리 및 롤백 용이
1. Docker 이미지는 버전 관리가 가능하여 특정 버전으로 쉽게 롤백할 수 있음.
2. 이미지에 태그를 붙여 상태를 명확히 구분 가능.