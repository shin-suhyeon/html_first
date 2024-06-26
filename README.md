# visual Studio code (VScode)
* vs code 실행 시 가장 먼저 확인해야할 것!
* 왼쪽 탐색기가 당일 작업폴더로 연결되어 있는지 확인하기!
* (위) 안되어있다면 -> 파일 -> 작업폴더닫기 후 -> 폴더열기 다시 진행!
# html 시작 
* git, gitHub 개념공부
* `<태그>` 웹페이지에서 의미적인 정보를 가지는 대상
## HTML5 버전선언
* `<!doctype html>`
## HTML 구조태그
* html : 웹의 시작과 끝. 문서 자체 의미.
* head : 웹 문서의 정보, 제목 포함
* meta : 웹 문서의 정보 기록
* title : 웹 문서의 제목(브라우저 상단 표시)
* body : 웹 문서 내용(실제 대부분의 서비스가 들어가는 본문)
## 구조 태그 속성
* `lang="ko"` html 문서 언어 설정
* `charset="uft-8"` 다국어 문자열 설정
* `description` 사이트 요약 설명
* `keywords` 사이트 검색 키워드 설정
## 속성 문법
`<태그 속성="값" 속성="값">`</태그>
* 태그와 속성 사이 공백
* 속성과 속성 사이 공백(속성 개수 제한없음)
* 속성은 시작태그에만 작성하기!
## 구조태그의 `title` 작성방법
* 메인페이지 -> 사이트명
* 메인페이지 -> 사이트명 - |  광고문구추가
* 서브페이지 -> 페이지명 | 사이트명
* ex) 책이름-저자명 | 서점명
* ex) 판매아이템명 | 사이트명
## h1~h6 제목태그(block tag)
* h1~h3 태그는 meta keywords와 동일한 검색키워드로 활용된다.(대제목일수록 높음)
* h4~h6 태그는 거의 사용하지 않는다.
* h1 대제목은 사이트의 로고 및, 서브 페이지 재목에서 주로 사용한다
* h 제목은 1~6레벨은 순서대로 작성해야 한다.
## 단락 p(block tag)
* 한 줄 또는 여러 줄 단락 묶을 때 사용하는 태그
* 제목(h) 태그 종류와는 형제 태그 관계로 사용해야 한다. 부모-자식(x)
## 인라인태그 br, em, strong, del, s, sup, sub
* `br` : 블록 내 줄바꿈 태그
* `strong` : 블록 내 경고용 강조 태그 (위와 특징 동일)
* `del` : 삭제 텍스트, 쇼핑몰의 할인 전 가격 등에 사용
* `s` : 교체 텍스트, 쇼핑몰의 할인 전 가격 등에 사용 (del 자주사용)
* `sup, sub` : 윗첨자 아래첨자 수학, 과학등의 기호에 사용
## 인용문 처리 blockquote, q
* `blockquote(block)` : 단락 자체가 인용문에 해당할 때 사용, p태그와 부모 -자식 관계로 사용해선 안된다!
* `q(inline)` " 단락(p) 내에서 일부가 인용문에 해당할 때 사용
* 공통 속성 `cite="url"` : `blockquote`, `q`로 인용문 처리할 경우 출처 표시용도로 주소(url)를 담아주는 속성.
## 특수문자 태그
* `&` 시작 `;` 종료
* `&copy;` &시작과 copyright의 copy 종료
* `&reg;` ®
## 주소태그
* `address` : 연락처, 회사소개, 고객센터 등 모든 사이트 아래에 나와있는 기본정보 footer 영역에 들어가는 본 사이트 주소
## 수평선 태그
* `hr` : 사이트를 각 영역으로 표시하는 수평선  block - 복잡한 html 태그 경계 구분
## 컴퓨터 명령어 태그
* `code`: 컴퓨터가 지원하는 다양한 명령어를 화면 표시에 표시 할 경우 inline 웹강의사이트에서 주로 사용하는 태그
## 링크태그 a
* block, inline 특징을 모두 가진다
* 절대경로와 상대경로를  href 속성에 작성한다
* 상대경로는 a태그 작성중인 파일 위치 기준 연결하고자 하는 목적지 파일이 같은 위치에 있는지, 하위 위치에 있는지 따라 다르게 작성한다
* `./` 현재 위치에서 시작
* `../` 상위 폴더로 나가기
* `.doll.jpg` : 현재 위치에서 doll.jpg 파일 찾기
* `../doll.jpg` :  상위 폴더로 한단계 나가서 doll.jpg 파일찾기
* `../a/doll.jpg` : 상위폴더로 한단계 나가고 a 폴더로 들어가서 doll.jpg 파일찾기
* `./b/doll.jpg` : 현재위치에서 b 폴더로 들어가서 doll.jpg 파일찾기
## 바로가기링크란?
* 긴 사이트 안에서 편리하게 필요한 정보를 빨리 찾을수 있게 글자에 링크를 걸어 바로갈 수 있는것을 말한다
* 단순 페이지 이동이 아닌 특정 위치로 스크롤 이동하는 바로가기 기능
## 바로가기 링크 제작 순서 및 주의사항
1. 이동 목적지에 가장 가까운 태그에 `id` 적용하기
2. 링크 대상에 `#id` href 속성값에 담기
* 주의사항 : #은 아이디 이동 링크에만 사용하기
* <id="">로 링크를 만든다
## 파비콘 적용 순서
1. 파비콘 크기로 이미지 다운받거나 편집하기
2. html에서 head안에 link태그로 `favicon` href주소 연결하기
## 이미지태그 `tag`
* 이미지 태그 안에 `alt`로 설명이 필요한 이미지엔 설명을 적고 설명이 필요 없는 이미지엔 `alt=""` 라도 적어야 한다
## figure, figcaption 태그
* 문서 안 사진을 감싸는 틀로서 활용하고 사진의 캡션을 정의 할 수 있습니다
## video 태그
* autoplay, muted, loop, controls 를 적어야함
## class, id 많이 사용하는 키워드
* wrapper, wrap, area 전체 묶는 영역
* contents, container 중~소 묶는 영역
* group, g 간단한 소그룹 영역
* top, btm, left, right 레이아웃 방향을 의미하는 키워드
* 예 : 의미있는단어_영역명
* 예 : product_wrap, item_area, price_g, main_contents
## div, span 그룹태그
### div
* 인라인고 블록이 2개 이상 형제일 경우 묶어주는 그룹태그
* 레이아웃 기준 1행에 2열 이상 배치일 경우
* 특정 의미를 가진 행에 같은 디자인 요소가 배치된 경우
### span
* 인라인이 2개 이상 형제일 경우 묶는 그룹태그
* 의미없는 디자인 요소 인라인 처리 필요 시 사용
## html5 semantic tag
* 
### semantic tag란?
* html5에서 생성된 의미있는 태그임
### header
* 로고 및 내비게이션을 묶어주는 웹 사이트 레이아웃 임
* 제목, 로고, 검색 폼, 작성자 이름 등의 요소도 포함할 수 있음
* 주로 맨 위 상단에 있음
### nav
* 다른 페이지로의 링크를 보여주는 구획을 나타냄. 자주 쓰이는 예제는 메뉴, 목차, 색인임
## ul,ol,li
* 작성 유형에 따라 순서가 있는 목록과 순서가 없는 목록으로 유형이 나뉩니다.
* 2개 이상의 목록(li) 구조을 묶어주는 그룹태그(ol)입니다.   
* 목록(li)의 순서가 있을 경우 ol을 사용합니다.
* 그룹(ol)은 반드시 목록(li)의 가장 근접한 부모로써 존재해야합니다.
* 2개 이상의 목록(li) 구조을 묶어주는 그룹태그(ul)입니다.
* 목록(li)의 순서와 연관 없을 경우 ul을 사용합니다.
* 그룹(ul)은 반드시 목록(li)의 가장 근접한 부모로써 존재해야합니다.
* ul 또는 ol 과 li 사이에 다른 태그를 삽입하지 않도록 주의해야합니다.   
* 순차/비순차 목록 사용 시 다른 블록 및 인라인 태그를 사용하려면 반드시 li 안 자식위치로 배치해야합니다.
* 순차/비순차 목록 1단 사용 시 추가 2단 / 3단을 제작하고 싶다면 새로운 목록(li)을 가지고 있는 (ul, ol) 부터 먼저 생성해야 합니다.
* 새로운 목록(li)이 만들어질때는 항상 ul 또는 ol 이 부모로 존재해야합니다.
## details, summary
* "열림" 상태일 때만 내부 정보를 보여주는 정보 공개 위젯을 생성합니다
* 요약이나 레이블은 (summary) 요소를 통해 제공할 수 있습니다.
## footer, mark, main, time
* `footer`:웹페이지 가장 하단에 위치합니다.
* 구획의 작성자, 저작권 정보, 관련 문서 등의 내용을 담습니다
* `mark`:현재 맥락에 관련이 깊거나 중요해 표시 또는 하이라이트한 부분을 나타냅니다.
* `main`:문서 (body) 의 주요 콘텐츠를 나타냅니다
* 주요 콘텐츠 영역은 문서의 핵심 주제나 앱의 핵심 기능에 직접적으로 연결됐거나 확장하는 콘텐츠로 이루어집니다.
* `time`:시간의 특정 지점 또는 구간을 나타냅니다.
## dl, dt, dd 정의형 목록 태그
* dl은 정의형 제목과 내용을 묶는 그룹입니다.
* dt는 dl안 자식으로 배치되며 제목을 의미합니다.
* dd는 dl안 자식으로 배치되며 dt의 다음 형제 요소로 배치되거나 기존 dd의 형제로도 배치될 수 있습니다.
* 다른 태그 조합 시 제목 또는 내용의 위치에 따라 dt 와 dd 안에만 추가 태그가 들어갈 수 있습니다.
* 제목과 내용 구조로 된 목록에 정의형 목록 태그를 사용합니다.

