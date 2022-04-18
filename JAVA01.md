# JAVA

* 객체지향 언어

  ## JAVA설치

* http://www.oracle.com/technetwork/java/index.html (오라클)에서 다운로드

* 설치시 환경변수 지정 해주어야함

  - 내PC -> 속성 -> 정보 -> 고급시스템 설정 -> 고급 -> 환경변수

    - JAVA_HOME : 자바설치 위치 주소 (ex.C:\Program Files\Java)

    - CLASSPATH : .;%JAVA_HOME%\lib\tools.jar(11버전 이상부터는 설정해줄 필요없음)
    - Path : %JAVA_HOME%\bin;기존패스
    - 설치 확인: cmd에서 명령어 4개 입력해본다 
      - JAVA -version
      - echo %JAVA_HOME%
      - echo %path&
      - JAVA(이거 입력시 관련명령어가 쫘악 뜨면 성공)

## Spring Tool Suite(STS)

- JAVA를 사용하기 위한 툴

- 새로운 WorkSpace 생성시 UTF-8 로 변경해주어야한다

  - STS - Window -Preference - General-Contents Types - Text - Default encording - UTF-8입력 - Update 클릭
  - STS - Window -Preference - General-Workspace- other - UTF-8 - Apply and close

- 기타 유용한 편집 환경 설정: Window --> Preferences 

  - 글꼴      : General - Apperance - Colors and Fonts - Basic - Text Font에서 수정(@글꼴은 세로로 출력, 12 이상 권장) 

  - 취소 버퍼 크기 : General - Editors - Text Editors - Undo history size: 20480, Display tab width: 2 

  - 라인 번호   : General - Editors - Text Editors - "Insert spaces for Tabs, Show Line Number" Check 

  - TAB의 공백 지정: Java - Code Style - Formatter - New... - Profile name: "java" 입력 후 확인 - Indentation - Tab policy를 "Spaces only"선택하고 확인  클릭 - Indentation size: 2, Tab size:2로 지정

