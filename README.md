# 이미지 생성해보자!

---

## 🚀 기능 요구 사항

---

사용자의 요청에 따라 이미지를 생성, 저장, 조회 기능을 제공하는 서비스를 구현합니다.

* 사용자 이메일, 패스워드를 통해 로그인을 할 수 있다.
    * 로그인 시 사용자 정보 관리를 쿠기&세션, JWT 중 무엇을 사용하더라도 문제 없다.
* 사용자 가입 시 저장하는 정보는 다음과 같다.
    * 이름
    * 이메일
    * 비밀번호
* 로그인한 사용자의 정보를 조회할 수 있는 API를 제공한다.
    * 조회시 이름, 이메일을 조회할 수 있다.
* 이미지 생성 API를 제공한다.
    * 이미지 생성 시 사용자에게 제시어를 입력 받아 해당 문자열을 통해 이미지를 생성한다.
    * 이미지 생성 시 사용할 API는 카카오에서 제공하는 karlo를 사용한다.
        * https://developers.kakao.com/product/karlo
    * 이미지가 생성이 완료되면 이미지 url을 데이터베이스에 저장해 사용자가 언제든지 조회할 수 있게 한다.
* 사용자가 생성한 이미지를 전체, 단건 조회할 수 있는 API가 제공된다.
    * 전체 이미지를 조회할때는 이미지 url과 생성 시간을 조회할 수 있다.
    * 하나의 이미지 정보를 조회할 때는 사용자가 입력한 제시어, url, 생성 시간을 조회할 수 있다.
* 사용자가 생성한 이미지를 삭제할 수 있는 API를 제공한다.
    * 사용자가 생성한 이미지를 삭제할 때 물리적으로 삭제하는 것이 아닌 논리적으로 삭제하여 복구할 수 있도록 한다.
* 앞선 모든 API들을 문서화해서 확인할 수 있다.

## 🎯 프로그래밍 요구 사항

---

* 자바 17버전을 기준으로 진행해야 합니다.
* build.gradle 의존성 설정은 자유롭게 진행하면 됩니다.

## ✏️ 과제 진행 요구 사항

---

* 해당 레포지토리를 fork&clone 해 진행하면 됩니다.
* 과제 기한은 과제 시작일 일주일 뒤까지 진행합니다.
* 과제 평가 시 과제 기한까지 진행한 커밋으로 평가합니다.