# upgraded 폴더 구조 설명

`upgraded` 폴더는 레거시 프로젝트의 전체 파일과 폴더를 복사하여 최신화 작업을 진행하는 공간입니다. 주요 구조는 다음과 같습니다:

- MANIFEST.in: 패키징에 필요한 파일 목록
- README.rst: 프로젝트 설명 파일
- distribute-0.6.10.tar.gz: 레거시 Python 패키지 배포 파일
- distribute_setup.py: 레거시 배포 스크립트
- setup.py: 프로젝트 설치 및 설정 스크립트
- docs/: 프로젝트 문서 폴더
  - Makefile: 문서 빌드용 Makefile
  - build/: 빌드된 문서 결과물
  - source/: 문서 소스 및 설정 파일
    - _static/: 문서용 정적 파일
    - changelog.rst, conf.py, example_usage.rst, getting_started.rst, index.rst, other_uses.rst: 문서 원본
- guachi/: 주요 Python 모듈 및 테스트 코드
  - __init__.py, config.py, database.py: 핵심 모듈 파일
  - tests/: 테스트 코드
    - test_configmapper.py, test_configurations.py, test_database.py, test_integration.py
- guachi.egg-info/: 패키지 정보 및 메타데이터
  - PKG-INFO, SOURCES.txt, dependency_links.txt, top_level.txt

이 폴더는 레거시 코드를 최신 Python 환경에 맞게 업그레이드하고 테스트하는 작업 공간입니다.