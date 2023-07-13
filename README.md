# **`'마크다운'`**
-------------------
------------------
# 하나짜리
## 두개짜리
### 세개짜리
#### 네개짜리

------ (3개이상)

리스트

순서가 있는 리스트
1. 순서
2. 순서2
    1. 내부로 들어오는 리스트
        1. 또 다시 내부로 들어오는 리스트

순서가 없는 리스트
* 첫번째
* 두번째
    * 내부로 들여쓰기
    * 들여쓰기
        * 또 내부로 들여쓰기

1. 첫 번째 순서는....
    * 1번을 하고
    * 2번을 하면
* 순서가 없는 리스트 내부에
    1. 이렇게 순서가 있는 리스트를 사용 가능합니다.
    2. 그렇습니다.
----------
# 코드블럭 사용하기

```python
print('hello')
```

* 이코드는 출력하는 코드입니다.
* 여기에서 `print`는 파이썬 함수입니다.
 
```javascript
console.log('hello World')
```

-------------
# 하이퍼 링크 만들기

[강아지 사진 API](https://dog.ceo/dog-api/)

------------
### 이미지 만들기

![강아지 사진](https://images.dog.ceo/breeds/dane-great/n02109047_282.jpg)

------------

이 문장 중에서 바로 **이것** 이 핵심이다.
이 문장의 출처는 *여기*입니다.
~~사실 무단 도용했습니다.~~


> 인용문 작성 할 수 있다.
>    >내부 인용도 가능


-----

# 표 만들기

| |컬럼1|컬럼2|
|---|---|---|
|1|내용|내용|
|2|내용|내용|


-----------


# **CLI**

1. **GUI**와 반대개념
2. *수많은 서버~~~* 
3. ~~GIT BASH~~
4. 명령어
    * touch 파일명.txt  - 파일 만들기
    * mkdir 폴더명 - 폴더 만들기
    * ls (-a) - 목록 보여주기
    * **cd 폴더명** - 폴더 내부에 존재하는 
    폴더로 이동
        * cd .. - 상위 폴더로 이동 
    * start 이름 - 열기
    * code 파일명 - vscode로 열기
        * code . - 현재 폴더에 있는 전부 vscode로 열기
    * rm 파일명 - 파일 지우기
        * rm `-r` 폴더명 - 폴더 지우기

------


# **GIT**
* 개념
1. working directory
    * 실제 작업중인 파일들 위치하는 영역
2. staging area
    * 변경된 파일들 중 잠시 중간에 저장해놓는 영역
3. repository
    * 버전 이력들과 파일들이 영구적으로 저장되는 영역 모든 버전과 변경 이력이 기록됨

---
* **git 동작**
1. git init
    * 로컬 저장소 초기화 설정 - git 버전 관리를 시작할 디렉토리에서 진행되고 디렉토리 안에 있는 하위 폴더까지 git으로 관리 가능
2. git add
    * 변경 사항이 있는 파일을 staging area에 추가
3. git commit
    * staging area에 있는 파일들을 repository에 기록하여 해당 시점을 생성하고 변경 이력을 남기는 것
    * `**어떤 이유로 이 버전을 찍게되었는지를  text로 기록하는 것이 필수**`

    
?. git restore
    * staging area를 비운다?
