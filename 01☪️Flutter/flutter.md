 ## < > 
![[Screenshot 2025-01-20 at 11.42.13 PM.png]]

## Sync 
1. ﻿﻿﻿메서드를 통해서 나오는 결과물은 future
2. ﻿﻿﻿Await 키워드를 만날때까지 Synchronous 방식으로 코드처리
3. ﻿﻿﻿await 키워드를 만나면 future가 완료될 때까지 대기
4. ﻿﻿﻿future가 완료 되자마자 그 다음 코드들을 실행

![[Screenshot 2025-01-20 at 11.46.35 PM.png]]

## Final vs const 
final is literally finally chosen when the application is working 
so it called run time const because it choosen for the last moment 
final 변수는 rebuild 될 수 있음

const must be init before compile also at the moment of declare should be initialized is demanded 
Compile-time constant = Run-time constant
```dart
void main() {
const time = DateTime.now();}
```
is impossible 

```dart

Widget build(BuildContext context) {

const survey = [

{

'질문': '좋아하는 음식은?'

'답변: ['김치찌개', '불고기', '비빔국수'],

질문': '좋아하는 색상은?'

'답변: ['파랑', '노랑', '보라'],

'질문': '좋아하는 캐릭터는?'

'답변: ['아이언맨', '배트맨', '스파이더맨'],

```

should be
## const 

When Flutter BuildTree rebuilding moment const prevent this variable rebuild again for useless rebuilding compartment

## Future 


1. ﻿﻿﻿Future 클래스는 비동기 작업을 할 때 사용
2. ﻿﻿﻿Future 는 일정 소요시간 후에 실제 데이터나 에러를 반환

3. ﻿﻿﻿다트에 의해서 future 객체가 내부적인 배열에 등록
4. ﻿﻿﻿Future관련해서 실행되어야 하는 코드들이 이벤트 큐에 등록
5. ﻿﻿﻿불완전한 future객체가 반환
6. ﻿﻿﻿Synchronous 방식으로 실행되어야 할 코드 먼저 실행
7. ﻿﻿﻿최종적으로 실제적인 data값이 future 객체로 전달
rr


- `Future`는 객체가 즉시 반환되지만, 결과는 나중에 제공됨.
#### Future Builder 

`FutureBuilder` is a widget in Flutter that helps handle asynchronous data fetching using a `Future`. It **rebuilds** the UI whenever the `Future`'s **state changes.**

abcdefg hiaea

## Getter 
a person or thing that gets a specified desirable thing.

ELECTRONICS•PHYSICS - a substance used to remove residual gas from a vacuum tube, or [impurities](https://www.google.com/search?client=safari&sa=X&sca_esv=c3860552ec9c0b33&rls=en&biw=1058&bih=670&q=impurities&si=ACC90nyOnVY18Aw7zUtkWPYo5mTnVzqWXO5NXGz4lZuM1nSYCLg_uhvwYpUyP_I7z-piGMjbFAcnlSa99EgscvupjYyqjrywM2qbQt3lCyPmGz8RIeWtQgI%3D&expnd=1&ved=2ahUKEwir9OLCnoKLAxXep1YBHeh9JZUQyecJegQIOxAR) or defects from a [semiconductor](https://www.google.com/search?client=safari&sa=X&sca_esv=c3860552ec9c0b33&rls=en&biw=1058&bih=670&q=semiconductor&si=ACC90nyj24cUGopiOVnGD91130XTRDyGiKBkyVxkiKiYef-mpglebUlH4FlIpiM9pwsFYcNM1Z_mWiYOqRRgksTrbRce5WL5TF4n08-G6K-GDK9H-aJkHOo%3D&expnd=1&ved=2ahUKEwir9OLCnoKLAxXep1YBHeh9JZUQyecJegQIOxAS) crystal.

## UI MainExis

space evenly 
![[Screenshot 2025-01-19 at 7.27.51 PM.png|500]]![[Screenshot 2025-01-19 at 7.32.30 PM.png|500]]

```dart
children: <Widget>[

- Image.asset('images/glogo.png'),
Text('Login with Google'

),  Text Opacity ( opacity: 0.0,)

child: Image.asset('images/glogo.png'),
// for make enverly 
```
## VoidCallBack
```dart 
void myFunction() {
  print("Button Pressed!");
}

ElevatedButton(
  onPressed: myFunction, // Using VoidCallback
  child: Text("Click Me"),
)
```
Here, `myFunction` is a `VoidCallback` because:

- It takes **no parameters**.
- It returns **void**.