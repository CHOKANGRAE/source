# 마크다운 이해하기

------

## 내용상의 제목을 표현하려면

`#` 제목(h1)- 하나의 문서에서 가장 중요한
`##` 제목(h2)- h1보다는 낮은 두번째 중요한
`###` h3 - 세번째 중요한 제목
`####` h4 - 네번째 중요한 제목
`#####` h5 - 다섯번째 중요한 제목
`######` h6 - 제목요소중에서 가장 낮은 위치 제목

------

## 내용을 표현하려면

내용을 표기하는 방법은, 단순하게 글을 작성하기만 하면 된다.
이때 줄바꿈은 띄어쓰기 두번 또는 `<br />` 표기를 하여 처리

> 또는 글 앞머리에 `>` 를하여, 내용을 작성
> 인용문 이라는 뜻을 가지고 있으나, 마크다운에서는 이미지를 추가 설명, 포인트로 체크사항을 알리는 용도 등으로 사용

하나의 내용이 끝나고 다른 내용을 작성하려면 엔터로 구분하지만, 명확하게 처리하기 위해 한칸을 비워두는 것이 좋다.

------

## 목록으로 처리하려면

마크다운에서는 리스트형식으로 처리되는 방법이 크게 2가지가 있다.

1. 순서가 있는 리스트

- 순서가 없는 리스트

------

### 순서가 있는 리스트

**order list** 개념을 가지고 있으며,
내용 앞에 `숫자.띄어쓰기 내용` 을 작성하여 여러 목록을 구분하며,
숫자는 순서대로 입력하지 않아도, 알아서 자동으로 처리 된다.

1. 순서가 있는 리스트
2. 순서대로 숫자를 표기
3. 자동으로 숫자가 카운트
4. 어떻게 쓰더라도 형식만 맞으면 원할하게 처리

------

### 순서가 없는 리스트

앞에 숫자가 표기되지 않고, 불릿기호가 표기되는 형식으로,
`unorder list`라는 의미로 부여가 된다.
작성요령은 목록의 앞에 `-띄어쓰기 내용`을 작성하면 된다.

- 순서가 없는 리스트
- `-`표기만 하면 된다.
- 기호는 알아서 자동으로 부여가 된다.

------

### 다단 리스트

다단 리스트란 목록에서 하위목록이 존재할 경우에 사용하는 표기방법
하위 리스트를 표기할 경우에는 상위 목록과는 들여쓰기(스페이스2, 탭)를 다르게 처리하면 된다.

- 목록을 표기하는 형태
- 다단리스트를 표현해보자
  - 하위 목록 리스트로 표기
  - 한번 들여쓰기를 작성하면 하위목록으로 처리
    1. 세번째 다단리스트로 처리
    2. 순서가 있는 없든 리스트자체는 관계가 없고,
    3. 단순히 들여쓰기를 어떻게 하였는가?
  - 두번째 목록 리스트
- 첫번째 목록 리스트

------

### 체크리스트 만들기

-  마크다운 내용정리
-  git사용법 정리
-  스케치요령
-  프로토타입툴 내용정리

------

### 강조 표현하기

내용이나, 제목, 리스트 등에서 굵게, 기울이기, 취소 등의 표기를 해서 강조를 하고자 할때 사용하는 기능

- **굵게하기** : 글씨의 앞 뒤에 `**`를 붙이면된다.
- *기울이게하기* : 글씨의 앞 뒤에 `*`를 붙이면 된다.
- ~~취소선~~ : 글씨의 앞 뒤에 `~~`를 붙이면 된다.
- ~~***굵기+기울임***~~

------

## 코드뷰 보기

실제 사용하는 언어에 대한 코드를 마크다운문서에서 볼 수 있도록 한 형태로 한줄코드, 여러줄 코드로 나뉜다.

------

### 한줄 코드

내용상에서 단어형식으로 짧게 코드로 보여주기 위한 형식
`<br />`처럼 코드를 보게 만들기로 앞 뒤에 ``` 을 표기

------

### 여러줄 코드

시작줄과 끝줄을 구분하며,
\``` 표기를 연달아 3개씩 시작과 끝줄에 작성하며,
시작 표기부분에 사용하는 언어의 명칭을 기입

```
<!doctype html>
<html>
  <head>
    <meta charset="utf-8">
    <title></title>
  </head>
  <body>
  </body>
</html>
```

------

## 링크 및 이미지

링크는 앵커로 불리우는 기능으로써 선택한 페이지로 이동하게 만드는 기능

------

### 주소만 보이게 만드는 기능

이동할 주소의 앞/뒤에 `<`,`>`를 각각 붙이고, 주소를 입력

[http://naver.com](http://naver.com/)
[http:google/com](http://google/com)

------

### 설명을 첨부하여 클릭시 해당하는 주소로 이동

설명란은 `[ ]`를 주소란은 `( )`를 만들어서 각각의 내용을 작성

[네이버로이동](http://naver.com/)
[웹표준문서: http://w3.org/tr](http://w3.org/tr)

------

### 이미지 연결하기

이미지를 연결하여 바로 볼 수 있도록 처리할 수 있다.
사용 요령은 앵커(링크기능)기능과 형태가 거의 같으며 앞에 `!`를 붙이면 된다. `[]`표기는 이미지에 대한 설명을 작성 하는 곳으로, 글이 보이지 않더라도 반드시 입력해야 한다.