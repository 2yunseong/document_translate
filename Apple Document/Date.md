# Date

특정한 한 점의 시간, 어느 달력이나 시간대로 부터 독립적이다.

## 선언(Declaration)

```swift
struct Date
```

## 개요(Overview)

`Date` 의 값은 시간의 한 점을 캡슐화한 값입니다. 이 값은 어떤 특정한 달력 시스템이나 시간대로 부터 독립적 입니다. 

Date 값은 절대적인 참고할 날짜로부터 상대적인 시간간격을 나타냅니다.

`Date` 구조체는 날짜를 비교하고, 두 날짜의 시간 간격을 비교하고, 한 날짜에 상대적인 시간간격을 가진 날짜로 부터 새로운 날짜를 생성하는 메소드를 제공합니다.

날짜나 시간을 현지화해서(그 상황에 맞게) 표현할 수 있는 인스턴스인 `DateFormatter`와 달력 계산을 수행하는 `Calender` 인스턴스와 함께 date 값을 함께 사용할 수 있습니다. 

`Date` 는 `NSDate` class와 이어져 있습니다. Objective - C API 와 상호작용할 때 이것들을 교차해서 사용할 수 있습니다.

## 주제
### Date 생성

`init()`

현재 날짜와 시간으로 초기화 된 date 값으로 생성

`init(timeIntervalSinceNow: TimeInterval)`

현재 시간과 주어진 초의 상대적인 시간으로 초기화된 date 값 생성

`init(timeInterval: TimeInterval, since: Date)`

주어진 date에 대한 초 단위의 상대적인 시간으로 초기화된 date 값 생성

`init(timeIntervalSinceReferenceDate: TimeInterval)`

2001년 1월 1일 00:00:00 UTC에 대한 초 단위의 상대적인 시간으로 초기화된 date 값 생성

`init(timeIntervalSince1970: TimeInterval)`

1970년 1월 1일 00:00:00 UTC에 대한 초 단위의 상대적인 시간으로 초기화된 date 값 생성

`init(from: Decoder)`

디코더로 부터 주어진 디코딩 값으로 새로운 인스턴스 생성

Link : [Apple Developer Document - Date](https://developer.apple.com/documentation/foundation/date)