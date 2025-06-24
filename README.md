# 0624_test



## GitHub 사용법

### ✅ GitHub 계정 만드는 순서 (2025년 기준)

1. **웹 브라우저 열기**
   크롬(Chrome), 엣지(Edge), 사파리(Safari) 중 편한 걸 사용하세요.

2. **GitHub 웹사이트 접속**
   주소창에 아래 주소를 입력하고 Enter 누르세요: https://github.com

3. **회원가입 시작하기**
   화면 오른쪽 위 또는 중간에 있는 Sign up 버튼 클릭

4. **이메일 주소 입력**
   평소 자주 사용하는 이메일을 입력

5. **비밀번호 만들기**
   영어 대문자, 소문자, 숫자, 특수문자를 섞어 안전하게!
   예시: Git1234!hub

6. **사용자 이름(Username) 정하기**
   나만의 고유한 이름을 지어요 (다른 사람이 쓰고 있으면 불가)
   - 예시: jetsunmom, sungsookjang66 등
   - 영어, 숫자, 하이픈(-) 가능 (띄어쓰기 ❌)

### ✅ Repository 만들기 순서

1. **GitHub에 로그인 후 New Repository 클릭**
2. ![new](https://github.com/user-attachments/assets/3481a680-f677-403b-be8c-1fe59d5aa7cb)

3. **Repository 이름 입력**
4. **Public/Private 선택**
5. **README.md 파일 생성 체크**
6. **Create repository 버튼 클릭**
   
![create_repository](https://github.com/user-attachments/assets/8c2eb16b-8dfc-465a-88cd-d35770d12df0)

## Markdown 문법

## 목차
- 1.마크다운 
  - 1.1 글머리
  - 1.2 글자 꾸미기
  - 1.3 목록 만들기
  - 1.4 이미지
  - 1.5 인용문
- 2.colab과 연동
- 3.W3school로 파이썬 연습

1.마크다운
============

# 1.1 글머리
```
# 글머리1
## 글머리2
### 글머리3
#### 글머리는 6까지만 지원
##### ※기호 뒤에 띄어쓰기 필수
```
# 글머리1
## 글머리2
### 글머리3
#### 글머리는 6까지만 지원
##### ※기호 뒤에 띄어쓰기 필수

# 1.2 글자 꾸미기
```
**굵게**
*기울임*
~~취소선~~
`코드처럼`
```
**굵게**
*기울임*
~~취소선~~
`코드처럼`

# 1.3 목록 만들기
```
- 항목1
- 항목2
  - 하위항목

1. 첫번째
2. 두번째
```

- 항목1
- 항목2
  - 하위항목
 
1. 첫번째
2. 두번째


# 1.4 이미지
![image](https://github.com/user-attachments/assets/982a60e8-5bf0-41bc-9a66-2fb3fbdfb6e7)


# 1.5 인용문
```
> 인용문입니다.
>> 중첩 인용도 가능합니다.
```
> 인용문입니다.
>> 중첩 인용도 가능합니다.

## Colab 기초  


![image](https://github.com/user-attachments/assets/06565493-e11e-4c7c-be67-e78baf6aff98)


## 2. About Python3

![image](https://github.com/user-attachments/assets/d3382497-075e-445a-8e91-8016f500e96a)

https://www.w3schools.com/

```
W3schools에서  파이썬 연습
```
Python에서 주의해야 할 점들
문법 관련 주의사항
들여쓰기 (Indentation)
Python은 들여쓰기로 코드 블록을 구분합니다
탭과 스페이스를 섞어 쓰면 안 됩니다
일관성 있게 스페이스 4개 또는 탭 사용

# 잘못된 예
# 올바른 예
if True:
print("Hello")  # 들여쓰기 없음 - 에러!
if True:
1234 print("Hello")  # 스페이스 4개, 4칸띄기기


대소문자 구분
Python은 대소문자를 구분합니다
Print와 print는 완전히 다른 것
# 잘못된 예
# 올바른 예
Print("Hello")  # 에러! (대문자 P)
print("Hello")  # 올바름





변수와 데이터 타입
변수명 규칙
숫자로 시작할 수 없음
특수문자 사용 불가 (밑줄 _ 제외)
예약어 사용 불가
# 잘못된 변수명
# 올바른 변수명
2name = "John"     # 숫자로 시작
my-name = "John"   # 하이픈 사용
class = "A"        # 예약어 사용
name2 = "John"
my_name = "John"
class_name = "A"


문자열 처리 주의사항
# 따옴표 주의
# 잘못된 경우
# 올바른 경우
text = "She said "Hello""  # 에러!
text = "She said \"Hello\""  # 올바름
text = 'She said "Hello"'   # 올바름



# 문자열과 숫자 연산
# 잘못된 경우
# 올바른 경우
age = 25
print("나이: " + age)   # 에러! 타입 불일치
age = 25
print("나이: " + str(age))   # 올바름
print(f"나이: {age}")        # 올바름 (f-string)









리스트와 인덱스
인덱스 범위 주의
my_list = [1, 2, 3]
print(my_list[3])  # 에러! 인덱스 범위 초과
print(my_list[2])  # 올바름 (마지막 요소)
print(my_list[-1]) # 올바름 (뒤에서 첫 번째)

리스트 복사 주의
list1 = [1, 2, 3]
list2 = list1        # 참조 복사 (같은 메모리)
list2.append(4)
print(list1)         # [1, 2, 3, 4] - 원본도 변경됨!

# 올바른 복사 방법
list2 = list1.copy()  # 또는 list1[:]

반복문과 조건문
무한 루프 주의
# 위험한 코드
while True:
    print("무한 루프!")  # Ctrl+C로 중단해야 함

# 안전한 코드
count = 0
while count < 10:
    print(f"카운트: {count}")
    count += 1  # 카운터 증가 잊지 말기!

조건문에서 할당 연산자 실수
x = 5
if x = 10:  # 에러! 할당 연산자 사용
    print("x는 10")

if x == 10:  # 올바름! 비교 연산자 사용
    print("x는 10")

## 3.  data structure / data sciencs

- [데이터 구조 개요](./data_structures.md)
- [Pandas](./pandas.md)
- [Numpy](./numpy.md)
- [Matplotlib](./Matplotlib.md)

## 4. Machine Learning

- [Machine Learning Basic](./ml_basic.md)
- [모델 훈련 및 평가](./ml_test.md)

## 5. OpenCV

- [OpenCV Basic](./OpenCV_basic.md)
- [이미지 처리](./image_test.md)

  
## 6. CNN(Convolution Neural Network
- [CNN_Basic](./CNN_basic.md)
- [CNN_자율주행 관련 코드](./cnn_test.md)

## 7. Ultralytics
- [Ultralytics_Basic](./Ultralytics_basic.md)
- [YOLOv8](./YOLOv8_test.md)
- [YOLOv12](./YOLOv12_test.md)
  
## 8. TensorRT vs PyTorch 
- [PyTorch_Basic](./PyTorch_basic.md)
- [TensorRT](./TensorRT_test.md)
- [YOLOv12](./YOLOv12_test.md)

## 9. TAO Toolkit on RunPod
- [TAO_사용법](.TAO_install.md)
- [TAO_Toolkit](.TAO_Toolkit.md)

## 10. 칼만필터, CARLA, 경로 알고리즘
- [kalman](.kalman.md)
- [CARLA_simulator](.CARLA.md)

## 11. ADAS & (ADAS TensorRT vs PyTorch)
- [adas_basic](.adas_basic.md)
- [TensorRT vs PyTorch 비교](.vs.md)
- 
