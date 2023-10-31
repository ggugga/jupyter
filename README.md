<!-- markdownlint-disable first-line-heading -->
<p align="center">
  <img src=".github/assets/logo.svg" alt="Vulhub" height="300" />
  <p align="center">
    <a href="https://github.com/vulhub/vulhub/blob/master/LICENSE">
      <img src="https://img.shields.io/github/license/vulhub/vulhub.svg" alt="GitHub">
    </a>
    <a href="https://www.wangan.com/vulhub">
      <img src="https://img.shields.io/badge/Official-Community-blue.svg" alt="Official Community">
    </a>
    <a href="https://discord.gg/bQCpZEK">
      <img src="https://img.shields.io/discord/485505185167179778.svg" alt="Discord">
    </a>
@@ -26,7 +23,7 @@ Vulhub는 사전 구축된 취약한 Docker 환경의 오픈 소스 모음입니다.

## 설치

Ubuntu 20.04에 Docker를 설치합니다.
Ubuntu 22.04에 Docker를 설치합니다.

```bash
# 최신 버전의 docker 설치
@@ -36,7 +33,7 @@ curl -s https://get.docker.com/ | .sh
systemctl 시작 도커
```

참고 : 이미 (더 이상 사용되지 않는) Docker Compose v1 (일명  'docker-compose')이 설치되어있는 경우 Compose v2로 업그레이드해야합니다.
 2022년 2월부터  'docker compose'는 [Docker Compose V2](https://www.docker.com/blog/announcing-compose-v2023-general-availability/)와 같은 하위 명령으로  Docker  에 병합되며, docker-compose의 Python 버전은 <>년 <>월 이후 더 이상 사용되지 않습니다. 따라서 Vulhub는 더 이상 추가  'docker-compose'를 설치할 필요가 없으며 모든 문서는  대신 'docker compose'를 사용하도록  수정됩니다.

다른 운영 체제의 경우 Docker와 Docker Compose의 설치 단계가 약간 다를 수 있으므로 자세한 내용은 [docker documentation](https://docs.docker.com/)을 참조하세요.

@@ -72,16 +69,15 @@ 취약점을 구축하기 위해 최소 1GB 메모리의 VPS를 사용하는 것이 좋습니다.

## 통지

1. 권한 오류를 방지하려면 루트 사용자를 사용하여 'docker' 명령을 실행하는 것이 가장 좋습니다.
2.  일부 Docker 이미지는 ARM 머신에서 실행을 지원하지 않습니다.
1. 권한 오류를 방지하려면 docker 컨테이너에 현재 디렉터리의 모든 파일에 액세스할 수 있는 권한이 있는지 확인하세요.
2.  Vulhub는 현재 ARM과 같은 비 x86 아키텍처를 사용하는 시스템에서의 실행을 지원하지 않습니다.

## 기부

이 프로젝트는 도커(docker)에 의존합니다. 따라서 컴파일 및 실행 중에 발생하는 모든 오류는 도커 및 관련 프로그램에서 발생합니다. 먼저 오류의 원인을 직접 찾아보십시오. 도커 파일이 잘못 작성되었거나 vulhub에서 코드가 잘못 작성된 것으로 판단되면 문제를 제출하십시오. 더 자세한 내용은 부탁드립니다 👉[Common reasons for compilation failure](https://github.com/phith0n/vulhub/wiki/%E7%BC%96%E8%AF%91%E5%A4%B1%E8%B4%A5%E7%9A%84%E5%8E%9F%E5%9B%A0)

