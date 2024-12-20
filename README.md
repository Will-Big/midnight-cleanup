# Midnight Cleanup

## 게임 실행 사진 및 영상

### Animatool 실행 화면
<img src="./images/tool_image.png" alt="툴 실행 화면" width="600">

### Launcher 실행 화면
<img src="./images/launcher_image.png" alt="런처 실행 화면" width="600">

### 실행 영상
[![게임 실행 영상](https://img.youtube.com/vi/WkjI6ZwUVwU/0.jpg)](https://www.youtube.com/watch?v=WkjI6ZwUVwU&ab_channel=%EC%97%94%EC%A0%A4%EC%B0%BD)

**설명**  
이 프로젝트는 C++20과 DirectX 11을 사용하여 개발된 3D 그래픽스 애플리케이션입니다.
게임인재원 졸업 프로젝트로 2024년 4월부터 2024년 11월까지 진행되었으며, 팀원 간 협업과 그래픽스 기술을 활용한 학습 및 연구를 목적으로 제작되었습니다.

프로젝트는 툴(Animatool)과 게임 런처(launcher)로 구성되어 있으며, 다음과 같은 주요 목표를 가지고 개발되었습니다:

- DirectX 11을 활용한 고품질 3D 렌더링 구현
- 효율적인 애니메이션 제작 및 관리 툴 개발
- 실시간 게임 플레이 환경에서 성능 최적화
- 그래픽스 프로그래밍을 학습하며 실무 역량 강화

---

## 프로젝트 구조

| 폴더 이름            | 설명                              |
|----------------------|------------------------------------|
| **Animacore/**       | 게임 엔진 내부 코드               |
| **Animatool/**       | 툴 코드                            |
| **Animavision/**     | 그래픽스 엔진 내부 코드           |
| **launcher/**        | 게임 런처 코드                     |
| **midnight_cleanup/**| 게임 플레이 코드                   |
| **Shaders/**         | 쉐이더 코드                        |
| **Resources/**       | 리소스 파일 (예: 텍스처, 모델)     |
| **lib/**             | 외부 라이브러리 (예: DLL, LIB 파일) |
---

## 외부 파일 다운로드

프로젝트 실행 및 빌드를 위해 필요한 외부 파일(DLL, LIB, 리소스)은 저장소에 포함되어 있지 않습니다. 아래 링크를 통해 다운로드한 후 적절한 경로에 배치해 주세요.

🔗 [외부 파일 다운로드 링크](http://naver.me/xhzusCaQ)

### 파일 배치 가이드
1. **DLL 파일**: 빌드된 실행 파일과 동일한 디렉토리에 배치 (lib 폴더 내부에서 복사)
2. **LIB 폴더**: `midnight-cleanup/` 디렉토리에 배치 (**솔루션(.sln) 파일과 동일한 위치**)
3. **리소스 폴더**: `midnight-cleanup/` 디렉토리에 배치 (**솔루션(.sln) 파일과 동일한 위치**)

---

## 빌드 방법

### 요구 사항
- **운영 체제**: Windows 10 이상
- **툴체인**: Visual Studio 2022 이상
- **언어 표준**: C++20
- **필수 SDK**: [DirectX SDK](https://www.microsoft.com/en-US/download/details.aspx?id=6812&msockid=3062152011ea654904ea003210c36437), Windows SDK
- **패키지 매니저**: [vcpkg](https://github.com/microsoft/vcpkg)

### 빌드 단계
1. 외부 파일 다운로드 링크를 통해 `외부 파일.zip`을 다운로드합니다.

2. 다운로드한 외부 파일(`lib`, `Resources`)을 클론한 저장소 폴더 안에 넣습니다. ([파일 배치 가이드](#파일-배치-가이드))
   - `lib` -> `midnight-cleanup/lib`
   - `Resources` -> `midnight-cleanup/Resources`

3. `vcpkg_list.txt` 파일을 참조하여 프로젝트가 요구하는 외부 헤더 파일을 추가합니다.  
   - 예: `vcpkg install 패키지명` 명령어를 사용하여 의존성을 설치

4. 빌드 대상 선택
   - **툴 빌드**: `Animatool` 프로젝트를 우클릭 한 후 `시작 프로젝트로 설정`을 선택합니다.  
   - **게임 빌드**: `launcher` 프로젝트를 우클릭 한 후 `시작 프로젝트로 설정`을 선택합니다.  
   - Visual Studio에서 `빌드 > 솔루션 빌드`를 실행합니다.

5. DLL 파일 추가
   -  빌드된 실행 파일과 동일한 디렉토리에 lib 파일에 포함된 dll 파일 배치

   

---

## 툴 및 게임 실행 방법

### 실행 파일 다운로드
1. 외부 파일 다운로드 링크를 통해 `실행 파일.zip`을 다운로드합니다.

2. 다운로드한 파일을 원하는 경로에 압축 해제합니다.

### 실행
1. **툴 실행**  
   - `Animatool.exe` 파일을 실행합니다.

2. **게임 실행**  
   - `launcher.exe` 파일을 실행합니다.
