도서관리 서비스 (Assignment 03)

Service Topic

도서관리 서비스를 만들었습니다. 사용자가 가지고 있는 책을 등록하고, 등록한 책을 확인하거나 수정하고 삭제할 수 있도록 여러 페이지로 구성했습니다.

Data Fields

도서명, 저자, 출판사, 출판년도, ISBN, 카테고리를 사용했습니다. 도서명은 책의 제목이고 저자는 책을 쓴 사람입니다. 출판사는 책을 발행한 곳이고 출판년도는 책이 출판된 연도입니다. ISBN은 책의 국제표준도서번호이고 카테고리는 컴퓨터/IT, 인문학, 소설, 과학 등으로 책을 구분하기 위해 사용했습니다.

List Page

index.html에서는 도서명, 저자, 출판년도, 카테고리를 표로 보여주도록 만들었습니다. 책을 클릭하면 view.html로 이동해서 상세 내용을 볼 수 있고, 위쪽에 있는 Add 버튼을 누르면 add.html로 이동해서 새로운 책을 등록할 수 있도록 했습니다.

Validation

add.html과 edit.html에서 입력값을 확인하도록 했습니다. 도서명, 저자, 출판년도, ISBN, 카테고리는 입력하지 않으면 제출되지 않도록 했습니다. 도서명은 2자 이상 입력해야 하고, 출판년도는 1000년부터 2026년까지 입력할 수 있도록 했습니다. 카테고리도 반드시 하나를 선택해야 합니다. 추가로 ISBN은 숫자와 하이픈(-)으로만 입력할 수 있고 10~17자 사이인지 확인하도록 했습니다.

RWD (Responsive Web Design)

화면 크기가 달라져도 사용할 수 있도록 Bootstrap의 container, table-responsive, row-cols 등을 사용했습니다. my.css에는 @media (max-width: 576px)를 추가해서 모바일 화면에서는 제목 크기를 줄이고 버튼이 화면 너비에 맞게 나오도록 했습니다. 표의 글자 크기도 모바일 화면에서는 작게 설정했습니다. Desktop과 Mobile 환경에서 확인했고 iPhone SE와 Galaxy S20 크기에서도 화면 밖으로 내용이 넘어가지 않는지 확인했습니다. 폼과 버튼도 정상적으로 작동하는지 확인했습니다.

Bootstrap

Bootstrap 5.3을 사용했고 navbar, container, row/col, table, table-responsive, card, form-control, form-select, btn, btn-primary, btn-danger, btn-outline-secondary 등을 사용했습니다.

Problem & Solution

add.html에서 추가 버튼을 눌렀을 때 index.html의 목록에 새로 입력한 책이 나타나지 않는 문제가 있었습니다. 이번 과제는 백엔드나 데이터베이스를 사용하지 않고 HTML을 중심으로 만든 과제라서 입력한 데이터를 페이지가 이동한 후에도 저장할 수 없었습니다. 그래서 실제 데이터를 저장하는 기능은 구현하지 않고, 추가 버튼을 누르면 확인 메시지를 보여주고 index.html로 이동하도록 만들었습니다.

Reflection

이번 과제를 하면서 Bootstrap의 반응형 그리드 시스템과 Media Query를 같이 사용하는 방법을 익혔습니다. 또한 needs-validation과 was-validated 클래스를 사용해서 입력값을 확인하는 Bootstrap 폼 검증 방법도 새롭게 알게 되었습니다.