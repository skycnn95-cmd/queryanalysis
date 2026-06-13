# Query Analysis 배포 패키지

이 디렉토리는 GitHub 배포를 위해 생성된 실행 가능한 빌드 패키지입니다.

## 파일 구성 안내
1. **`query_analysis.jar`**: 실행 가능한 웹 어플리케이션 프로그램 (Spring Boot 빌드 결과물)
2. **`query_analysis.db`**: 기본으로 제공되는 내장 SQLite 데이터베이스 파일 (사전 초기화된 테이블 및 샘플 데이터 포함)
3. **`db_config.json`**: 데이터베이스 접속 정보 환경설정 파일 (기본값 SQLite 세팅)
4. **`run.bat`**: Windows 환경에서 원클릭으로 어플리케이션을 구동하기 위한 스크립트
5. **`run.sh`**: Linux / macOS 환경에서 어플리케이션을 구동하기 위한 스크립트

## 구동 방법
### 1. 사전 요구사항
- 시스템에 **Java 17 이상**(JDK 또는 JRE 17)이 설치되어 있어야 합니다.
- 설치 여부 확인: 터미널에서 `java -version` 실행

### 2. 실행
- **Windows**: `run.bat` 파일 더블클릭 또는 실행
- **Linux/macOS**: 터미널에서 `chmod +x run.sh` 실행 후 `./run.sh` 실행

### 3. 웹 접속
- 브라우저를 열고 다음 주소로 이동합니다:
  - 로그인 및 메인 화면: `http://localhost:8080/`
  - 데이터베이스 접속 설정 변경 화면: `http://localhost:8080/dbenv`

## 로그인 정보
- **최초 관리자 아이디**: `admin`
- **최초 관리자 비밀번호**: `admin`

## 데이터베이스 연동 정보 변경
- 웹으로 접속하여 `/dbenv` 환경설정 페이지에서 MYSQL, ORACLE, MARIADB 등으로 언제든 동적 데이터베이스 접속 환경을 전환하실 수 있습니다.
