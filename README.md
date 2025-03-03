![Frame 1000002424](https://github.com/OMZigak/iOS/assets/144984293/d5e851a7-4ecf-467f-a09a-7cb3433b996d)
![표지](https://github.com/user-attachments/assets/f1982348-39cd-45c4-bb73-3266637734be)
```
이 세상 모든 지각 꾸물이들의 정시 도착 꿈을 이뤄줄 꿈같은 서비스, 꾸물꿈 ⏰💤
34기 NOW SOPT AppJam 꾸물꿈 프로젝트입니다.
```
[꾸물꿈에 대해 더 자세히 알고 싶다면? 프로젝트 설계 및 주요 기능 소개 보기✔️](https://arrow-frog-4b9.notion.site/9c6895231a2346d0b5b9a15570f47b22?pvs=4)


# 목차
1. [프로젝트 소개]
2. [iOS Team]  
3. [기술 스택]  
4. [코딩 컨벤션]  
5. [브랜치 전략]  
6. [폴더링]  
7. [트러블 슈팅]  
</br>

![Frame 1000002423](https://github.com/OMZigak/iOS/assets/144984293/e8373f56-2bf7-4f99-ba68-a8eb94c31c9e)

<details>
<summary> </summary>

|김진웅</br>[@JinUng41](https://github.com/JinUng41)|이지훈</br>[@hooni0918](https://github.com/hooni0918)|이유진</br>[@youz2me](https://github.com/youz2me)|김수연</br>[@mmaybei](https://github.com/mmaybei)|
|:---:|:---:|:---:|:---:|
|<img src = "https://github.com/user-attachments/assets/9ec0d2f4-3515-4d2c-8433-b0326a06b6ac" width ="250">|<img src = "https://github.com/user-attachments/assets/513a88e4-db78-4e11-9c42-6dda99bfe6fa" width ="250">|<img src = "https://github.com/user-attachments/assets/566a0a8c-c673-4650-b9f4-3b74d7443aa9" width ="250">|<img src = "https://github.com/user-attachments/assets/0c785026-a0c1-4e1a-bc28-fc12072b724e" width ="250">|
|`약속 추가 플로우`, `모임 상세`|`푸시 알림`, `온보딩`, `마이페이지`|`모임 추가 플로우`, `약속 상세`|`홈`, `내 모임`, `준비 정보 입력`|

</details>
</br>


![Frame 1000002428](https://github.com/OMZigak/iOS/assets/144984293/8c3ba259-6b8d-47b9-9f5d-97e8bc48ccd7)
<details>
<summary> library </summary> 
  
|library|description|
|:---:|:---:|
|**FirebaseSDK**|FCM을 이용한 푸쉬 알림을 구현하기 위함|
|**KakaoSDK**|카카오 소셜 로그인 구현을 위함|
|**Lookin**|UI 구현에 있어, 뷰 계층을 보다 쉽게 파악하기 위함|
|**Moya**|추상화된 네트워크 레이어를 보다 간편하게 사용하기 위함|
|**RxCocoa**|뷰의 상태 관리를 위한 동적 프로그래밍 도입|
|**RxSwift**|뷰의 상태 관리를 위한 동적 프로그래밍 도입|
|**Snapkit**|UI 구현에 있어, 오토레이아웃을 보다 간편하게 사용하기 위함|
|**Then**|UI 구현에 있어, 클로저를 통해 인스턴스를 초기화하기 위함|
|**Kingfisher**|이미지 캐싱 처리 및 UI 성능 개선을 위함|
</br>
</details>

![Frame 1000002425](https://github.com/OMZigak/iOS/assets/144984293/7975890a-1ffc-4b51-84e8-8102c454c52e)
[꾸물아요들의 코딩컨벤션 보기✔️](https://github.com/OMZigak/iOS_Styleguide)
</br>
</br>


![Frame 1000002426](https://github.com/OMZigak/iOS/assets/144984293/fc19dbd0-5755-4a67-87c0-8ab4b1558ea2)

<details>
<summary> </summary>

```
main 브랜치: 최종 제출용
suyeon 브랜치: 개발 작업용 (default 브랜치)

1. 기능 개발, 네트워크, 리팩토링, 세팅 등 작업할 내용에 대한 이슈 생성
2. suyeon 브랜치에서 이슈 브랜치 생성
3. 이슈 브랜치에서 작업
4. 작업 완료 후 PR 작성, 체크리스트를 통해 어떤 것을 해결한 이슈인지 명시
5. 코드리뷰를 통해 모든 구성원이 approve하였을 때 suyeon 브랜치로 머지
```
</details>

</br>

![Frame 1000002427](https://github.com/OMZigak/iOS/assets/144984293/89e48d23-a134-4ad1-8c9d-bf01769a2f46)


<details>
<summary> </summary>
  
```
📁 Kkumulkkum
├── 📁 Application
│   ├── AppDelegate
│   ├── SceneDelegate
├── 📁 Source
│   ├── 🗂️ Onboarding
│   │   ├── 🗂️ Model
│   │   ├── 🗂️ ViewModel
│   │   ├── 🗂️ View
│   │   ├── 🗂️ ViewController
│   ├── 🗂️ Home
│   ├── 🗂️ My
│   ├── 🗂️ Core
│   │   ├── TabBar
│   │   ├── View
│   │   ├── Cell
├── 📁 Resource
|   ├── 🗂️ Extension
|   |   ├── UIStackView+
|   |   ├── UIView+
|   |   ├── ...
|   ├── 🗂️ Util
|   |   ├── ReuseIdentifiable
|   |   ├── Screen
|   |   ├── ...
|   ├── 🗂️ Font
|   |   ├── .ttf
|   ├── Asset.xcassets
│   ├── Info.plist
├── 📁 Network
```

</details>

![Frame 1171276151](https://github.com/user-attachments/assets/a79a75bc-92d6-4745-a613-275b3ffb9770)

<details>

  
# 직렬화를 통한 Data Race 해결
  [링크](https://github.com/OMZigak/KKUYOS/pull/407)
## 문제상황

- 홈 화면에서 여러 API 호출(로그인 유저, 가까운 약속, 다가오는 약속)이 동시에 이루어질 때 토큰 만료 시 Data Race 발생
- 약 10번 중 1번 정도 자동 로그인 실패 현상 확인
- 각 API 요청이 개별적으로 토큰 갱신 메커니즘을 트리거하여 중복 실행 문제
- 
## 해결방법

### 직렬 큐 방식 도입

- TokenRefreshManager 클래스를 생성하여 토큰 갱신 로직 중앙화
- 
```swift
private let queue = DispatchQueue(label: "com.TokenRefreshManager.queue")
```

- 토큰 갱신 중 새로운 요청은 대기 후 처리하는 방식 구현

```swift
if self.isRefreshing {
    DispatchQueue.global().asyncAfter(deadline: .now() + 0.1) {
        self.refreshToken(completion: completion)
    }
    return
}

```

### 동시성 제어 방식 비교 및 선택 이유

- NSLock: 세밀한 제어 가능하나 데드락 위험성
- 세마포어: 대기시간을 예측할 수 없어 사용자 경험 저하 우려
- **직렬 큐: 순차적 실행 보장, 낮은 오버헤드, 구현 단순성**

### 컨커런시 도입 제한 요인

- Alamofire Interceptor의 adapt와 retry 메서드가 컨커런시를 지원하지 않음
- 서드파티 라이브러리 의존성의 제약 경험
- 이를 통해 Third-party 라이브러리에 과도하게 의존하지 않는 아키텍처 설계의 중요성 학습

### 리프레시 토큰 로테이션 적용

- 토큰 갱신 시 새로운 AccessToken과 RefreshToken 모두 저장하는 방식 적용

## 결과

- 자동 로그인 성공률 99% 이상으로 향상
- 동시 API 요청 상황에서도 안정적인 토큰 갱신 보장
- 사용자가 토큰 만료로 로그아웃되는 상황 최소화


  <br>


# Custom Pulse 구현 및 성능 개선
  [링크](https://github.com/OMZigak/KKUYOS/pull/409)
  <br>
3. 토큰 갱신 성능 최적화
 링크
# 토큰 갱신 관리자 성능 최적화

## 문제 상황

기존 토큰 갱신 메커니즘은 재귀적 호출 패턴을 사용해 동시에 여러 요청이 들어올 경우 시간 복잡도가 O(n)으로 증가했습니다. Instruments 프로파일링을 찍어본 결과

- 호출 스택이 깊어지고(20개 이상의 중첩된 워커 스레드), CPU 사용량이 불규칙한 스파이크를 보였습니다
- 각 요청마다 0.1초의 지연이 누적되어 반응성이 저하되었습니다
- 전체 실행 시간의 52.52%가 스택 트레이스에 소비되고 있었습니다
- 워커 스레드들이 각각 0.8%~3.6%의 CPU 시간을 분산 차지하며 리소스 사용이 비효율적이었습니다

## 핵심 알고리즘 개선

이 문제를 해결하기 위해 다음 알고리즘과 자료구조를 적용했습니다:

- **콜백 큐 패턴**: 모든 요청을 배열에 저장하고 일괄 처리하여 네트워크 요청을 O(1)로 감소

```swift
private var pendingCompletions: [(Result<String, Error>) -> Void] = []
```

- **디바운싱 알고리즘**: 20ms 내 연속 요청을 단일 작업으로 통합하여 중복 제거

```swift
self.refreshWorkItem?.cancel()
let workItem = DispatchWorkItem { [weak self] in
    self?.performTokenRefresh(with: currentRefreshToken)
}

```

- **지수 백오프 알고리즘**: 네트워크 실패 시 2^n * 100ms 패턴으로 재시도하여 복원력 강화

```swift
let delay = pow(2.0, Double(self.requestCount)) * 0.1
```

## 개선 효과

- 호출 스택 깊이 감소: 20개 이상 → 5개 미만으로 간소화되어 메모리 사용량 최적화
- 중첩 재귀 호출 제거: 메인 스레드가 94.6%로 효율적으로 작업 처리
- CPU 사용 패턴: 불규칙한 스파이크에서 더 낮고 균일한 패턴으로 개선
- 응답 시간: 최대 작업 시간 162ms에서 큰 폭으로 감소
- 시간 복잡도: 네트워크 요청 횟수가 O(n) → O(1)로 개선되어 사용자 요청 수에 무관한 일정한 반응 시간 보장
- 재시도 메커니즘: 지수 백오프를 통한 네트워크 불안정 상황에서의 복원력 향상

## 구체적인 개선 결과

Instruments를 통한 프로파일링에서 개선을 확인했습니다:

1. `_dispatch_workloop_worker_thread`의 중첩 호출이 감소하고 메인 스레드(580ms)가 효율적으로 작업을 처리
2. `_CFRunLoopRun`과 같은 CoreFoundation 함수들이 더 체계적으로 호출
3. CPU 사용량 그래프가 더 일정하고 예측 가능한 패턴을 보임
4. `refreshToken` 함수의 재귀적 중첩 호출이 사라지고, 단일 호출 패턴으로 변경

이러한 최적화를 통해 토큰 갱신 처리 시간이 요청 수에 관계없이 일정하게 유지되어 앱의 전반적인 반응성과 성능을 향상시켯습니다.

### 개선 전후 비교
<p align="center">
  <img width="40%" alt="개선 이전" src="https://github.com/user-attachments/assets/100a87f4-d93c-4b50-b78d-de70ecf2d1d3" />
  <img width="40%" alt="개선 이후" src="https://github.com/user-attachments/assets/cfef6122-17dc-4234-b722-ba4c368d6022" />
</p>

  <br>

  
4. SOLID 의거 코드 원칙 수립
  링크
<br>
</details>



