# 일기장 앱
---

- UITabBarController:
    - 다중 선택 인터페이스를 관리하는 컨테이너 뷰 컨트롤러. 선택에 따라 어떤 자식 뷰 컨트롤러를 보여줄 건인지가 결정됨.
    - layer: Custom View hierarchy > Navigation View > Tab Bar View > Window > Assembled View
    i.e. 아이폰 시계 앱

- UICollectionView
    - 데이터 항목의 정렬된 컬렉션을 관리하고 커스텀한 레이아웃을 사용해 표시하는 객체
    - 구성요소:
        - Cell
            컬렉션 뷰의 컨텐츠 표시
        - Supplementary View
            섹션에 대한 정보를 표시
        - Decoration View
            컬렉션 뷰에 대한 배경을 꾸밀 때 사용
    - Layout and FlowLayout
        - FlowLayout
            1. Flow 레이아웃 객체를 작성하고 컬렉션 뷰에 이를 할당한다
            *2. 셀의 Width, Height를 정한다*
            3. 필요한 경우 셀들 간의 좌우 회소 간격, 위아래 최소 간격을 설정한다.
            4. 섹션에 header와 footer가 있다면 이것들의 크기를 지정한다.
            5. 레이아웃의 스크롤 방향을 설정한다.
    - UICollectionViewDataSource
        - 컬렉션 뷰로 보여지는 컨텐츠들을 관리하는 객체
        - 프로토콜이 중요함
        - collectionView - numberOfItemsInSection : 지정된 섹션에 표시할 셀의 개수를 묻는 메서드
        - collectionView - cellForItemAt : 컬렉션 뷰의 지정된 위치에 표시할 셀을 요청하는 메서드
        - numberOfSections : 섹션의 개수를 묻는 메서드
    - UICollectionViewDelegate
        컨텐츠의 표현, 사용자와의 상호작용과 관련된 것들을 관리하는 객체
    i.e. slider
