# cloud-travel-document

본 문서는 Cloud Travel 앱을 테스터가 자신의 아이폰에서 실행시킬 수 있는 방법을 설명합니다. 

Apple 기기에서 실행되는 App은 Apple App Store에서 심사를 받지 않고는 원칙적으로 아무기기에서나 설치할 수 없습니다. 
그리하여 사전에 테스트할 기기의 UDID를 App개발자가 배포용 인증서와 함께 배포프로필에 포함시켜 App을 빌드하여 배포합니다. 
사전에 등록된 기기에서만 App을 실행시킬 수 있다는 말입니다. 

```
테스트할 기기의 UDID를 알기위해 App개발자가 Firebase를 통해 테스터에게 메일을 보낸다. 
메일을 수신받은 테스터는 메일의 절차대로 진행한다. 
UDID가 App 개발자에게 전달된다. 
테스터의 UDID를 등록하여 App Rebuild 후 Firebase를 통해 테스터에게 설치메일을 보낸다.
수신받은 메일 절차대로 진행하여 테스트 App을 실행한다. 
```


아래의 방법이 Google Firebase를 통해 테스트 배포하여 설치할수 있는 방법을 제공합니다. 
1. App 개발자가 테스터들의 Email을 사전에 알아야 진행 가능합니다. 아래 메일로 메일주소를 보내주시면 Cloud Travel을 실행절차를 진행할 수 있는 메일을 보내드립니다.
>mctlmk@gmail.com

2. 수신받은 메일(UDID 수신용)
![스크린샷, 2022-11-24 00 10 54](https://user-images.githubusercontent.com/59984223/203667908-80fce9f7-061b-4707-b39a-009c256c95a0.jpeg)
3. Get Started 버튼 클릭
![스크린샷, 2022-11-24 00 11 33](https://user-images.githubusercontent.com/59984223/203667860-d01ba64a-d47b-4f35-8abd-70dc709e8c2f.jpeg)
4. Safari App을 통해 실행 
![스크린샷, 2022-11-24 00 11 55](https://user-images.githubusercontent.com/59984223/203667938-734b1f09-47af-46bf-94c5-45f28ee8aae1.jpeg)
5. 내용확인 후 동의 체크박스 체크 후 초대수락 버튼클릭
![스크린샷, 2022-11-24 00 13 46](https://user-images.githubusercontent.com/59984223/203678833-4ed1adfb-4a32-4f42-8489-5fba6f33a39a.jpeg)
![스크린샷, 2022-11-24 00 14 10](https://user-images.githubusercontent.com/59984223/203678883-d52873f5-08fd-45ba-bff7-13aa0694f51e.jpeg)
6. 기기등록버튼 클릭
![스크린샷, 2022-11-24 00 14 26](https://user-images.githubusercontent.com/59984223/203667963-74f85983-1244-4b52-9890-a35e22a7c725.jpeg)
7. 프로필 다운로드
![스크린샷, 2022-11-24 00 15 02](https://user-images.githubusercontent.com/59984223/203667970-92330994-70a5-4064-bc1a-8ffa0d049e45.jpeg)
8. 설정에서 다운받은 프로필을 설치
![스크린샷, 2022-11-24 00 15 56](https://user-images.githubusercontent.com/59984223/203667976-7ad102c4-c547-4c92-8089-82d8548320fe.jpeg)
![스크린샷, 2022-11-24 00 16 12](https://user-images.githubusercontent.com/59984223/203667979-dac752ab-67a4-462e-ad45-f7b771b6df68.jpeg)
![스크린샷, 2022-11-24 00 16 45](https://user-images.githubusercontent.com/59984223/203667985-dc4a50e0-277a-4d3c-8171-fc4e56e0e67b.jpeg)
9. Safari로 돌아와 완료 버튼 클릭
![스크린샷, 2022-11-24 00 17 08](https://user-images.githubusercontent.com/59984223/203667996-53248bba-1fce-4c6f-8a59-da00810addf7.jpeg)
10. 완료화면 / 이후 개발자에게 UDID가 전달됨.
![스크린샷, 2022-11-24 00 17 28](https://user-images.githubusercontent.com/59984223/203668002-1fd66ba9-f1dc-4550-8b1e-e7949e3779f6.jpeg)
11. 두번째 메일 수신
![스크린샷, 2022-11-24 00 23 49](https://user-images.githubusercontent.com/59984223/203668009-e3fa8023-0c09-49f0-acdf-161c31295b87.jpeg)
12. Safari App을 통해 실행
![스크린샷, 2022-11-24 00 24 31](https://user-images.githubusercontent.com/59984223/203668015-00b77d97-3ae6-41c9-b27f-6ec38c83a7a7.jpeg)
13. App 다운로드 실행
![스크린샷, 2022-11-24 00 24 49](https://user-images.githubusercontent.com/59984223/203668020-13329e6e-9ff3-4d45-86c6-4f94d031727a.jpeg)
![스크린샷, 2022-11-24 00 25 19](https://user-images.githubusercontent.com/59984223/203668023-a4fcf2eb-45e0-411c-adf9-116ee1ab5357.jpeg)
14. 설치된 App 확인
![스크린샷, 2022-11-24 00 25 47](https://user-images.githubusercontent.com/59984223/203668033-8f752bdc-9840-457a-a094-56d25d13d3a9.jpeg)
15. App 실행시 개발자모드 Alert 확인
![스크린샷, 2022-11-24 00 27 24](https://user-images.githubusercontent.com/59984223/203668040-ec3d58cc-7043-4670-9096-33bf28d01b2b.jpeg)
16. 설정 > 개인정보 보호 및 보안 > 개발자 모드 Enable
![스크린샷, 2022-11-24 00 27 38](https://user-images.githubusercontent.com/59984223/203668046-1bfa686d-11bd-492d-bbdd-ea66b796dd76.jpeg)
![스크린샷, 2022-11-24 00 27 51](https://user-images.githubusercontent.com/59984223/203668050-7ace5064-2969-4a00-8ee9-c25911cee723.jpeg)
![스크린샷, 2022-11-24 00 28 08](https://user-images.githubusercontent.com/59984223/203668061-cb85e7fb-396a-4832-ad1d-f1e3df10c9bb.jpeg)
17. App실행 후 App에서 보내는 알람을 수신받을 수 있도록 허용 선택
![스크린샷, 2022-11-24 00 30 12](https://user-images.githubusercontent.com/59984223/203668065-a07d819d-ca4d-4066-adfd-6f4297c44644.jpeg)
