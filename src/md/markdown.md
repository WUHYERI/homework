# ~ 마크다운 문법을 알아보자 ~

###### 마크다운은 문서 작성을 위한 형식으로 사용되며 문법이 간결하고, HTML삽입이 가능합니다.

### 목차

- [Headers](#headers)<br>
- [Line](#line)<br>
- [Line Breakers](#line-breakers)<br>
- [Emphasis](#emphasis)<br>
- [Lists](#lists)<br>
- [Backlash Escapes](#backlash-escapes)<br>
- [Links](#links)<br>
- [Code Block](#code-block)<br>
- [Table](#table)<br>

---

## Headers
\# 을 사용하여 헤더를 만듭니다.<br> # 의 개수에 따라 헤더의 크기가 달라집니다.

> # # H1 가장 크다
> ## ## H2
> ### ### H3
> #### #### H4
> ##### ##### H5
> ###### ###### H6 가장 작다

## Line

\- \* \_ 중 하나를 3개 이상 작성하여 라인을 만들 수 있습니다.<br>

`---`<br>
`***`<br>
`___`<br>

---

---

## Line Breakers

\<br> 를 사용해서 줄바꿈을 할 수 있습니다.<br>
~~~
안녕하세요 반갑습니다.<br>저는 이 글의 작성자 우혜리 입니다.
~~~
안녕하세요 반갑습니다.<br>저는 이 글의 작성자 우혜리 입니다.

## Emphasis

\* \- \~ 을 사용하여 글씨를 강조할 수 있습니다.<br>
`*기울기*`<br>_안녕하세요~_<br>
`**굵게** `<br>**안녕하세요~**<br>
`***굵은 기울기*** `<br>**_안녕하세요~_**<br>
`~~취소선~~ `<br>~~안녕하세요~~~<br>
`_기울기_ `<br>_안녕하세요~_<br>
`__굵게__ `<br>**안녕하세요~**<br>
`___굵은 기울기___ `<br>**_안녕하세요~_**<br>

## Blockquotes

\> 를 사용하여 인용을 할 수 있습니다. \> 는 3개까지 가능합니다.

```markdown
안녕하세요
> 반갑습니다
> > 다음에
> > > 또만나요
```

안녕하세요
> 반갑습니다
> > 다음에
> > > 또 만나요 ~

## Lists
1. list <br> 
\* \+ \- 를 사용하여 순서가 없는 목록을 만들 수 있습니다.
```makrdown
* 안녕하세요
* 안녕하세요
  * hi
    * bye
```
* 안녕하세요
* 안녕하세요
  * hi
    * bye

---
2. ordered list <br> 
숫자를 사용하여 순서가 있는 목록을 만들 수 있습니다. <br> 
1 번부터 순서대로 알아서 숫자를 매깁니다.
```markdown
1. 안녕하세요
2. 반갑습니다
100. 다음에 또 만나요
```
1. 안녕하세요
2. 반갑습니다
100. 다음에 또 만나요

## Backlash Escapes
\를 사용하여 특수문자를 표현할 수 있습니다.<br>
``` \* ``` <br>
\*

## image

```![텍스트](이미지파일경로)``` 를 사용하여 이미지를 추가할 수 있습니다. <br> "이미지 이름" 을 추가하여 마우스를 올려놨을 때 나오는 텍스트를 수정할 수 있습니다.
```markdown
![프로필사진](https://github.com/WUHYERI/homework/blob/main/src/assets/profile.jpg?raw=true "원숭이가 웃기다")
```
![프로필사진](https://github.com/WUHYERI/homework/blob/main/src/assets/profile.jpg?raw=true "원숭이가 웃기다")


## Links
1. external link<br>
```[이름](주소 "설명")```를 사용하여 외부링크를 삽입할 수 있습니다.
```markdown
[참고사이트](https://inpa.tistory.com/entry/MarkDown-%F0%9F%93%9A-%EB%A7%88%ED%81%AC%EB%8B%A4%EC%9A%B4-%EB%AC%B8%EB%B2%95-%F0%9F%92%AF-%EC%A0%95%EB%A6%AC "블로그인가?")
```
[참고사이트](https://inpa.tistory.com/entry/MarkDown-%F0%9F%93%9A-%EB%A7%88%ED%81%AC%EB%8B%A4%EC%9A%B4-%EB%AC%B8%EB%B2%95-%F0%9F%92%AF-%EC%A0%95%EB%A6%AC "블로그인가?")

2. internal link<br>
```[보여지는 내용](#이동할 헤드(제목))``` 을 사용하여 내부로 이동할 수 있습니다.<br>
내부 링크는 Heather의 소문자로 변환된 이름을 사용합니다.<br>Heather의 공백은 - 으로 변환됩니다.
```markdown
[목차로 이동합니다](#목차)
```
[목차로 이동합니다](#목차)


## Code Block
\```을 사용하여 코드블럭을 만들 수 있습니다.<br>
언어를 지정해주면 syntax color가 적용됩니다.
```
~~~html
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <title>Title</title>
</head>
<body>
    <h1>Hello, World!</h1>
</body>
</html> 
~~~
~~~javascript
function test() {
 console.log("look ma’, no spaces");
}
~~~
```
~~~html
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <title>Title</title>
</head>
<body>
    <h1>Hello, World!</h1>
</body>
</html>
~~~
~~~javascript
function test() {
 console.log("look ma’, no spaces");
}
~~~
## Table
헤더는 | 로 구분하고 구분선은 - 로 만듭니다. :를 사용하여 각 열의 정렬을 설정할 수 있습니다.
```markdown
| 정렬방법 |   왼쪽정렬  |오른쪽정렬| 가운데 정렬  
|:--:     |:--         |--:     |     :--:|
|결과     | 왼쪽        | 오른쪽  |가운데     |

|칸|채우기|입력|
|:--:|:--:|---|
|안하면|공란     |

```
| 정렬방법 |   왼쪽정렬  |오른쪽정렬| 가운데 정렬  
|:--:     |:--         |--:     |     :--:|
|결과     | 왼쪽        | 오른쪽  |가운데     |

|칸|채우기|입력|
|:--:|:--:|---|
|안하면|공란     |

---