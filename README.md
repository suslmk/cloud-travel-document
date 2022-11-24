# Cloud Travel App 설치가이드

본 문서는 Cloud Travel 앱을 테스터가 자신의 아이폰에서 실행시킬 수 있는 방법을 설명합니다. <br>

Cloud Travel의 Client는 IOS 네이티브 언어인 SwiftUI로 개발되었습니다. <br>
오직 `IOS 16이상의 IPhone기기`에서만 테스트가 가능한 점 참고 부탁드립니다.

## App 테스트 유의점
Apple 기기에서 실행되는 App은 Apple App Store에서 심사를 받지 않고는 원칙적으로 아무기기에서나 설치할 수 없습니다. <br>
그리하여 사전에 테스트할 기기의 UDiD를 App개발자가 배포용 인증서와 함께 배포프로필에 포함시켜 App을 빌드하여 배포해야만 테스터(심사위원)가 App을 설치 후 사용해 볼 수 있습니다.<br>
사전에 등록된 기기에서만 App을 실행시킬 수 있다는 뜻 입니다.<br> 
><b>UDiD란</b><br>
모든 iPhone, iPod, iPad 및 ATV에는 해당 장치에 고유 한 숫자와 문자로 구성된 40 자 길이의 고유 식별자 (UDiD)가 있습니다. 기기 식별자입니다.

## App 테스트를 위한 상호 과정
```
1. 테스터(심사위원)는 App개발자에게 자신의 메일주소를 통보
2. 개발자는 테스터에게 UDiD 제공요청을 위한 메일 발송
3. 테스터는 1차 수신 받은 메일을 통해 UDID 제공 동의
4. 개발자는 제공받은 UDiD를 App 배포 프로필에 포함시켜 App Rebuilding 후 배포
5. 테스터는 2차 수신 받은 메일을 통해 App 설치 후 확인
```


## App 테스트를 위한 상세 절차
아래는 Google Firebase를 통해 테스트 배포하여 설치할수 있는 절차를 설명합니다.  
1. App 개발자가 테스터들의 Email을 사전에 알아야 진행 가능합니다. 아래 메일로 메일주소를 보내주시면 Cloud Travel을 실행절차를 진행할 수 있는 메일을 보내드립니다.
>mctlmk@gmail.com

2. 수신받은 메일(UDiD 수신용)</br>
<img src="https://user-images.githubusercontent.com/59984223/203667908-80fce9f7-061b-4707-b39a-009c256c95a0.jpeg" width="250" height="500"/>
3. Get Started 버튼 클릭</br>
<img src="https://user-images.githubusercontent.com/59984223/203667860-d01ba64a-d47b-4f35-8abd-70dc709e8c2f.jpeg" width="250" height="500"/>
4. Safari App을 통해 실행</br>
<img src="https://user-images.githubusercontent.com/59984223/203667938-734b1f09-47af-46bf-94c5-45f28ee8aae1.jpeg" width="250" height="500"/>
5. 내용확인 후 동의 체크박스 체크 후 초대수락 버튼클릭</br>
<img src="https://user-images.githubusercontent.com/59984223/203678833-4ed1adfb-4a32-4f42-8489-5fba6f33a39a.jpeg" width="250" height="500"/>
<img src="https://user-images.githubusercontent.com/59984223/203678883-d52873f5-08fd-45ba-bff7-13aa0694f51e.jpeg" width="250" height="500"/>
6. 기기등록버튼 클릭</br>
<img src="https://user-images.githubusercontent.com/59984223/203667963-74f85983-1244-4b52-9890-a35e22a7c725.jpeg" width="250" height="500"/>
7. 프로필 다운로드</br>
<img src="https://user-images.githubusercontent.com/59984223/203667970-92330994-70a5-4064-bc1a-8ffa0d049e45.jpeg" width="250" height="500"/>
8. 설정에서 다운받은 프로필을 설치</br>
<img src="https://user-images.githubusercontent.com/59984223/203667976-7ad102c4-c547-4c92-8089-82d8548320fe.jpeg" width="250" height="500"/>
<img src="https://user-images.githubusercontent.com/59984223/203667979-dac752ab-67a4-462e-ad45-f7b771b6df68.jpeg" width="250" height="500"/>
<img src="https://user-images.githubusercontent.com/59984223/203667985-dc4a50e0-277a-4d3c-8171-fc4e56e0e67b.jpeg" width="250" height="500"/>
9. Safari로 돌아와 완료 버튼 클릭</br>
<img src="https://user-images.githubusercontent.com/59984223/203667996-53248bba-1fce-4c6f-8a59-da00810addf7.jpeg" width="250" height="500"/>
10.  완료화면 / 이후 개발자에게 UDID가 전달됨.</br>
<img src="https://user-images.githubusercontent.com/59984223/203668002-1fd66ba9-f1dc-4550-8b1e-e7949e3779f6.jpeg" width="250" height="500"/>
</br>
</br>
</br>
</br>
===========================
1.   두번째 메일 수신</br>
<img src="https://user-images.githubusercontent.com/59984223/203668009-e3fa8023-0c09-49f0-acdf-161c31295b87.jpeg" width="250" height="500"/>
2.   Safari App을 통해 실행</br>
<img src="https://user-images.githubusercontent.com/59984223/203668015-00b77d97-3ae6-41c9-b27f-6ec38c83a7a7.jpeg" width="250" height="500"/>
3.   App 다운로드 실행</br>
<img src="https://user-images.githubusercontent.com/59984223/203668020-13329e6e-9ff3-4d45-86c6-4f94d031727a.jpeg" width="250" height="500"/>
<img src="https://user-images.githubusercontent.com/59984223/203668023-a4fcf2eb-45e0-411c-adf9-116ee1ab5357.jpeg" width="250" height="500"/>
4.   설치된 App 확인</br>
<img src="https://user-images.githubusercontent.com/59984223/203668033-8f752bdc-9840-457a-a094-56d25d13d3a9.jpeg" width="250" height="500"/>
5.   App 실행시 개발자모드 Alert 확인</br>
<img src="https://user-images.githubusercontent.com/59984223/203668040-ec3d58cc-7043-4670-9096-33bf28d01b2b.jpeg" width="250" height="500"/>
6.   설정 > 개인정보 보호 및 보안 > 개발자 모드 Enable</br>
<img src="https://user-images.githubusercontent.com/59984223/203668046-1bfa686d-11bd-492d-bbdd-ea66b796dd76.jpeg" width="250" height="500"/>
<img src="https://user-images.githubusercontent.com/59984223/203668050-7ace5064-2969-4a00-8ee9-c25911cee723.jpeg" width="250" height="500"/>
<img src="https://user-images.githubusercontent.com/59984223/203668061-cb85e7fb-396a-4832-ad1d-f1e3df10c9bb.jpeg" width="250" height="500"/>
7.   App실행 후 App에서 보내는 알람을 수신받을 수 있도록 허용 선택</br>
<img src="https://user-images.githubusercontent.com/59984223/203668065-a07d819d-ca4d-4066-adfd-6f4297c44644.jpeg" width="250" height="500"/>
