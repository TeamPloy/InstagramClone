### Instagram 클론코딩

주제 : Instagram 메인페이지 클론코딩

컨벤션에 꼭 한 가지도 빠짐없이 알맞게 코드를 작성해야 하며,  
깃허브를 사용하여 주기적으로 코드를 커밋할 수 있도록 합니다.

### GITHUB

- 위 링크에서 레포지토리를 포크후, 포크된 본인의 레포지토리를 클론하여 개발을 시작합니다.
- 커밋은 주기적으로 이루어져야 하며, 최소 한 섹션을 개발할 때마다 커밋합니다.
- 정해진 기한 내에 자신의 깃허브 아이디로 된 브랜치를 생성하여 insertcourse/frontend-beginner-instagram 레포지토리에 풀 리퀘스트(이하 PR)를 생성합니다.  
  PR은 "[인스타그램 클론코딩] 박우빈 미션 제출합니다."와 같은 형식으로 생성되어야 합니다.  
  PR에 코드를 작성하며 자신이 느꼈던 점이나 어려웠던 점, 흥미있었던 점, 또는 궁금한 점 등을 작성할 수 있습니다.
- 커밋을 할 때에 정해진 커밋 규칙을 통해서 커밋하도록 합니다.
- 제출기한을 꼭 엄수할 수 있도록 합니다.

### COMMIT RULE

ADD, UPDATE : 특정 기능이나 섹션, 컴포넌트(이하 부분) 등을 추가하였을 때  
FIX : 특정 부분 중 잘못된 부분을 수정하였을 때  
DELETE : 특정 부분을 삭제하였을 때  
REFACTOR : 기존에 있던 부분에서 코드를 리팩토링하였을 때

커밋은 다음의 예시들과 같이 진행합니다.

```
git commit -m "FIX : 팔로우 버튼에 마우스 hover시 글자색이 바뀌지 않는 오류 수정"

git commit -m "ADD : 인스타그램 스토리 스크롤 컴포넌트 추가"
```

### 코드 컨벤션

1. 템플릿의 형식에 따라 코드를 작성해야 합니다. index.html, style.css, script.js 파일을 모두 이용할 수 있도록 합니다.
2. section, aside, div, span, img 태그를 한 번 이상 필수적으로 사용해야합니다.
3. 각 섹션은 총 세 개로 나누며, 고유한 id값 외에 다른 값을 가질 수 없습니다.
4. 자식 컴포넌트들은 부모 컴포넌트의 id나 class값을 기준으로 대쉬바 두 개를 사용하여 네이밍하도록 합니다.

```html
<div id="name">
  <div class="name--box">
    <input class="name--box--input" />
  </div>
  <div class="name--container">
    <span class="name--container--text"></span>
  </div>
</div>
```

5. 인라인 스타일은 절대 사용하지 않도록 합니다.
6. 섹션은 아래와 같이 크게 세 개의 섹션으로 나누도록 합니다.  
   너비는 다음과 같이 viewport 단위로 작업해야하며, 왼쪽의 사이드바는  
   위/아래로 스크롤해도 고정되어 있어야 합니다.
7. 인스타그램 스토리 목록의 프로필 컴포넌트는 최소 12개여야하며,  
   스크롤을 하지 않았을 때 기본으로 8개의 컴포넌트만이 보여야합니다.  
   또한 좌/우로 스크롤할 수 있어야하며, 스크롤바는 보이지 않게 설정하도록 합니다.

8. 오른쪽 사이드바의 "회원님을 위한 추천" 탭에서 "팔로우" 버튼 위 마우스를  
   올렸을 때 글자색이 검은색으로 바뀌어야하며, 마우스 커서는 "포인터"가 되도록 합니다.

9. 오른쪽 사이드바의 "전환" 버튼을 눌렀을 때, 사용자에게 변경할 인스타 아이디를 입력받아 프로필에 있는 이름을 바꿀 수 있도록 합니다.  
   만약 사용자가 아무 것도 입력하지 않았다면, 사용자에게 "값이 입력되지 않았습니다!"를 띄우고 이름을 변경하지 않습니다.
10. 사용자의 이름은 자율적으로 정할 수 있으며, 기본적으로는 "instagramer"를 사용합니다.
11. 추가적으로 제공되지 않는 아이콘은 직접 구하여 구현해야 합니다.