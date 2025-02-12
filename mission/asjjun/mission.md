# 사전 미션

## 1. 컨테이너 기술이란 무엇입니까?
컨테이너 기술은 다양한 컴퓨팅 환경에서 이식 가능하고 일관된 방식으로 애플리케이션을 패키징, 배포 및 실행하는 방법입니다. 컨테이너는 종속성, 라이브러리 및 구성 파일과 함께 애플리케이션을 캡슐화하는 방법을 제공하여 Docker 또는 Kubernetes와 같은 컨테이너 플랫폼을 지원하는 모든 시스템에서 안정적이고 일관되게 실행할 수 있도록 합니다.

컨테이너는 다음과 같은 몇 가지 주요 이점을 제공합니다.

이식성: 컨테이너는 개발자의 노트북, 온프레미스 서버, 클라우드 기반 환경 등 컨테이너 런타임을 지원하는 모든 플랫폼에서 실행될 수 있습니다.
격리: 컨테이너는 일정 수준의 격리를 제공하여 애플리케이션과 해당 종속성이 동일한 호스트 시스템에서 실행되는 다른 애플리케이션과 분리되도록 합니다. 이러한 격리는 보안을 강화하고 서로 다른 애플리케이션 간의 충돌을 방지합니다.
효율성: 컨테이너는 호스트 시스템의 운영 체제 커널을 공유하므로 기존 가상 머신에 비해 가볍고 리소스 효율성이 높습니다.
확장성: 컨테이너화된 애플리케이션은 동일한 컨테이너의 여러 인스턴스를 생성하여 쉽게 수평으로 확장할 수 있으므로 효율적인 리소스 활용과 향상된 성능이 가능합니다.

Docker와 같은 널리 사용되는 컨테이너화 플랫폼을 통해 개발자는 애플리케이션을 컨테이너로 구축, 패키징 및 배포할 수 있습니다. Kubernetes와 같은 오케스트레이션 도구는 머신 클러스터 전체에서 컨테이너화된 애플리케이션의 배포, 확장 및 관리를 관리하고 자동화합니다.

전반적으로 컨테이너 기술은 애플리케이션을 패키징, 배포 및 실행하는 일관되고 효율적인 방법을 제공함으로써 소프트웨어 개발 및 배포에 혁명을 일으켰습니다.

## 2. 도커란 무엇입니까?
Docker는 컨테이너 내에서 애플리케이션을 개발, 배포 및 관리하기 위한 도구와 프레임워크를 제공하는 널리 사용되는 플랫폼입니다. 컨테이너화 세계의 주요 업체로서 애플리케이션을 컨테이너로 구축, 배송 및 실행하는 프로세스를 간소화하는 제품 및 서비스 제품군을 제공합니다.

Docker의 주요 구성 요소는 다음과 같습니다.

Docker Engine: Docker의 핵심 구성요소입니다. 호스트 시스템에서 컨테이너를 생성하고 관리할 수 있는 경량 런타임 및 패키징 도구입니다. Docker 엔진에는 컨테이너 관리를 위한 Docker 데몬과 데몬과 상호 작용하기 위한 Docker CLI(명령줄 인터페이스)가 포함되어 있습니다.
Docker 이미지: Docker는 이미지를 컨테이너의 구성 요소로 사용합니다. 이미지는 애플리케이션 코드, 라이브러리, 종속성 및 애플리케이션을 실행하는 데 필요한 기타 파일을 포함하는 읽기 전용 템플릿입니다. 이미지는 컨테이너를 만드는 데 사용됩니다.
컨테이너: 컨테이너는 격리된 프로세스로 실행되는 Docker 이미지의 인스턴스입니다. 애플리케이션을 해당 종속성과 함께 캡슐화하여 다양한 환경에서 일관되게 실행할 수 있습니다.
Docker Hub: Docker Hub는 Docker에서 제공하는 클라우드 기반 레지스트리 서비스로, 방대한 Docker 이미지 컬렉션을 호스팅합니다. 이를 통해 개발자는 Docker 이미지를 저장, 공유 및 협업할 수 있으므로 애플리케이션을 더 쉽게 배포할 수 있습니다.
Docker Compose: Docker Compose는 다중 컨테이너 Docker 애플리케이션을 정의하고 관리하기 위한 도구입니다. YAML 파일을 사용하여 복잡한 애플리케이션에 필요한 서비스, 네트워크 및 볼륨을 구성합니다.

Docker는 컨테이너에서 애플리케이션을 생성, 배포, 실행하는 프로세스를 단순화함으로써 컨테이너 기술 대중화에 중요한 역할을 해왔습니다. 사용 편의성, 이식성 및 효율성으로 인해 현대 소프트웨어 개발 및 배포 파이프라인의 표준 도구가 되었습니다.

## 3. 도커 파일, 도커 이미지, 도커 컨테이너의 개념은 무엇이고, 서로 어떤 관계입니까?
도커파일:
Dockerfile은 Docker 이미지를 빌드하는 데 필요한 지침과 명령이 포함된 텍스트 파일입니다. 이는 애플리케이션에 필요한 환경과 종속성을 조립하는 데 필요한 단계를 지정하여 Docker 이미지를 생성하기 위한 청사진 역할을 합니다. 이러한 지침에는 사용할 기본 이미지, 설치할 패키지, 추가할 파일, 실행할 명령 등이 포함됩니다.

도커 이미지:
Docker 이미지는 소프트웨어를 실행하는 데 필요한 모든 것(코드, 런타임, 라이브러리, 환경 변수 및 구성 파일)이 포함된 독립 실행형 실행 패키지입니다. docker build 명령을 사용하여 Dockerfile에서 생성됩니다. 컨테이너의 스냅샷이나 템플릿으로 생각하면 됩니다. 이미지는 변경할 수 없으며 공유, 저장 및 여러 컨테이너를 만드는 데 사용할 수 있습니다.

도커 컨테이너:
Docker 컨테이너는 Docker 이미지의 실행 가능한 인스턴스입니다. 애플리케이션과 해당 종속성을 캡슐화하는 가볍고 격리된 실행 가능한 환경입니다. 컨테이너는 docker run 명령을 사용하여 Docker 이미지에서 생성됩니다. 호스트 시스템에서 격리된 프로세스로 실행되지만 커널을 다른 컨테이너와 공유합니다. 컨테이너는 독립적으로 시작, 중지, 삭제 및 관리될 수 있습니다.

관계:
Dockerfile은 Docker 이미지를 생성합니다. Dockerfile은 이미지를 빌드하는 데 필요한 단계를 정의합니다. Dockerfile이 포함된 디렉터리에서 docker build -t image_name .을 실행하면 Dockerfile의 지침을 실행하고 이미지가 생성됩니다.
이미지는 Docker 컨테이너를 생성합니다. 이미지가 있으면 docker run 명령을 사용하여 이미지에서 하나 이상의 컨테이너를 생성할 수 있습니다. 각 컨테이너는 해당 이미지의 인스턴스이며 정의된 환경 내에서 애플리케이션을 실행하면서 독립적으로 작동합니다.
이미지는 변경할 수 없습니다. 컨테이너는 실행 가능한 인스턴스입니다. 이미지는 읽기 전용 템플릿인 반면, 컨테이너는 해당 이미지에서 생성된 쓰기 가능한 활성 인스턴스입니다. 컨테이너는 시작, 중지, 삭제, 수정될 수 있지만 이미지는 변경되지 않습니다.
Dockerfiles, Docker 이미지 및 Docker 컨테이너는 Docker 컨테이너화 기술의 핵심을 형성하여 개발자가 애플리케이션을 위한 일관되고 이동 가능하며 격리된 환경을 만들고 개발, 배포 및 관리 프로세스를 간소화할 수 있도록 해줍니다.