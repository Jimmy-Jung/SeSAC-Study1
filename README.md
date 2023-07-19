# SeSAC-Study1

### Q1. Entry Point가 무엇이며, 왜 필요할까요?

### A1.

Xcode에서 Entry Point는 iOS 앱이 시작될 때 호출되는 함수입니다. 이 함수는 `AppDelegate.swift` 파일에서 찾을 수 있으며, iOS 앱의 핵심적인 기능 중 하나입니다. Entry Point가 없으면 앱이 실행되지 않을 수 있습니다.

### Q2. Enrty Point가 없으면 어떻게 될까요?

### A2.

Entry Point가 없으면 iOS 앱이 실행되지 않습니다. Entry Point는 iOS 앱이 시작될 때 호출되는 함수입니다. 이 함수는 `AppDelegate.swift` 파일에서 찾을 수 있으며, iOS 앱의 핵심적인 기능 중 하나입니다.

### Q3. Entry Point 삭제 후 디버그 영역을 확인하고, 앱이 다시 정상적으로 동작할 수 있도록 Entry Point를 지정해보세요.

<img width="783" alt="image" src="https://github.com/Jimmy-Jung/SeSAC-Study1/assets/115251866/1f636867-df97-4a06-be62-aa399fd240ff">


이 오류는 iOS 앱이 실행될 때 `Main.storyboard` 파일에서 지정된 Entry Point가 올바르게 설정되지 않아서 발생하는 오류입니다.

 Entry Point가 설정되어 있지 않으면 iOS 앱이 시작될 때 실행될 뷰 컨트롤러를 찾을 수 없기 때문에 발생합니다.

 이 오류를 해결하려면 `Main.storyboard` 파일에서 올바른 Entry Point를 지정해야 합니다.

<img width="783" alt="image" src="https://github.com/Jimmy-Jung/SeSAC-Study1/assets/115251866/9c6a967c-ba66-49da-a40b-43f76a4fc77b">

<img width="785" alt="image" src="https://github.com/Jimmy-Jung/SeSAC-Study1/assets/115251866/61fba31f-518d-471c-b4f9-85d44e6b76f7">


`Main.storyboard`에서 진입접으로 사용될 Tab Bar Controller를 클릭해 인스팩터 영역을 보면 

Is Initial View Controller를 클릭해 진입점을 생성해주면 Tab Bar Controller 좌측에 진입접을 나타내는 화살표가 표시된다.

### UI 구현하기

<img width="783" alt="image" src="https://github.com/Jimmy-Jung/SeSAC-Study1/assets/115251866/70ad9ff6-865b-40a8-8f2d-5c8266e2f529">



### Q1 iOS15버전과 iOS14버전에서 Button은 어떤 차이가 있을까?


### A1

iOS15버전 이후로 버튼을 default로 설정하면 title text의 길이에 따라 자동으로 …이 표시된다.

### Q2 Xcode 프로젝트의 최소 지원 버전을 iOS 13.0 버전 이하로 설정하면 빌드가 되지 않고 오류가 발생하는데 왜 그럴까?

<img width="783" alt="image" src="https://github.com/Jimmy-Jung/SeSAC-Study1/assets/115251866/d3c3e58a-fa01-4a8f-9cf4-3c46cda95c5e">

### A2

AppDelegate와 SceneDelegate에서 iOS13.0에서 이용가능하다는 오류가 발생한다.

최소지원버전을 iOS13이상으로 설정해주면 오류를 해결할 수 있다.

iOS13.0이후 버전은 AppDelegate가 SceneDelegate로 분할되었다.

iOS13.0 부터 SwiftUI를 지원하면서 객체들이 기본적으로 Struct로 이루어져 있다.

기존에 @UIApplicationMain Attribute는 Class만 적용 가능하기 때문에 

@main Attribute로 업그레이드 되었다.

@main Attribute는 **Structure, Class, Enumeration 모두에 적용**할 수 있다.


### Q3 탭뷰 컨트롤러를 무한정 연결하면 어떻게 될까?

### A3

<img width="683" alt="image" src="https://github.com/Jimmy-Jung/SeSAC-Study1/assets/115251866/c02b98ed-cc09-43ba-9717-b01f13f3671e">

탭뷰 아이템은 5개가 최대고, 5개를 넘어가면 5번째 탭이 More로 바뀌고 More탭에 TableView형태로 정리된다.


