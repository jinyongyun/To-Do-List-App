# To-Do-List-App
오늘은 뭐할까 내일은 뭐할까 반드시 지켜야 하는 작심삼일 방지용 앱

## 활용 기술
UITableView
UIAlertController
UserDefaults

## UITableView
데이터를 목록 형태로 보여 줄 수 있는 가장 기본적인 UI 컴포넌트
UIScrollView를 상속받고 있어 스크롤이 가능하다
테이블 뷰를 사용하기 위해서는 UITableView 데이터 소스와 UITableView Delegate 프로토콜을 채택해여 구현해줘야 한다.
DataSource는 데이터를 받아 뷰를 그려주는 역할이고, Delegate는 테이블 뷰의 동작과 외관을 담당한다. 뷰가 변경되는 사안을 delegate가 담당하고 뷰는 delegate에 의존해 뷰를 업데이트한다.
tableView는 데이터 소스와 델리게이트의 정의에 따라 테이블 뷰를 어떻게 표시할지 결정한다.

## UITableViewDataSource
UITableVIewDataSource는 테이블 뷰를 생성하고 수정하는데 필요한 정보를 테이블 뷰 객체에 제공

func tableView(_ tableView: UITableView, numberOfRowsInSection section: Int) -> Int
//각 섹션에 표시할 행의 개수를 묻는 메소드
func tableView(_ tableView: UiTableView, cellForRowAt indexPath: IndexPath) -> UITableViewCell
// 특정 인덱스 Row 의 cell에 대한 정보를 넣어 cell을 반환하는 메소드
이 두개는 반드시 구현해야 하는 UITableViewDataSoruce 프로토콜 내부에 정의 되어 있는 메소드이다.

## UITableViewDelegate
테이블 뷰의 시각적인 부분을 설정하고, 행의 액션 관리, 엑세서리 뷰 지원 그리고 테이블 뷰의 개별 행 편집을 도와준다.

채택했을 때 필수로 구현해야 하는 메소드는 없다!

## 완성
![스크린샷 2022-06-30 오후 3 44 41](https://user-images.githubusercontent.com/102133961/176610431-ecfb52db-63d8-40db-a1d8-059e16d28aa9.jpg)
![스크린샷 2022-06-30 오후 3 45 11](https://user-images.githubusercontent.com/102133961/176610521-49f3b785-0f4e-4f75-ad06-9ae0b75d5c8b.jpg)
![스크린샷 2022-06-30 오후 3 45 30](https://user-images.githubusercontent.com/102133961/176610566-8b210b92-e61c-49d4-93a4-e641d92bc4c8.jpg)
