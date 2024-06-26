# 제목(Header)

# 제목 1
## 제목 2
### 제목 3
#### 제목 4
##### 제목 5
###### 제목 6

# 문장(Paragraph)
동해물과 백두산이 마르고 닳도록 
하느님이 보우하사 우리나라 만세

# 줄바꿈(Line Breaks) : 2번 띄어쓰기 또는 br태그
동해물과 백두산이 마르고 닳도록  
하느님이 보우하사 우리나라 만세  
무궁화 삼천리 화려 강산<br/>
대한 사람 대한으로 길이 보전하세

# 강조(Emphasis) : u 태그는 마크다운에서만 사용
_이텔릭_  
**두껍게**  
**_이텔릭 + 두껍게_**  
~~취소선~~  
<u>밑줄</u>

# 목록(List) : 들여쓰기 탭을 2번하라고 강의에서는 나왔지만 1번해도 가능
1. 순서가 필요한 목록
1. 순서가 필요한 목록
    1. 순서가 필요한 목록
    1. 순서가 필요한 목록
1. 순서가 필요한 목록

- 순서가 필요하지 않은 목록
- 순서가 필요하지 않은 목록
    - 순서가 필요하지 않은 목록
- 순서가 필요하지 않은 목록
    - 순서가 필요하지 않은 목록
    - 순서가 필요하지 않은 목록
- 순서가 필요하지 않은 목록

# 링크(Links) : taget="_blank" 를 통해 새탭으로 열고 싶을때에는 원시html 문 사용해야 함

```markdown
[대체텍스트](url)
```


### 1-A. 원시 html 사용 예제
```html
<a href="http://google.com">Google</a>  
```
<a href="http://google.com">Google</a>  

---  
### 1-B. Markdown 코드 사용 예제
```markdown
[Google](http://google.com)    
```
[Google](http://google.com)  

### 2-A. (HTML) 링크에 커서 가져가는 경우 메모 보이기
```html
링크에 커서를 hovor한 경우 title 에 적은 메모가 보이게 하는 원시 HTML 예제
<a href="http://naver.com" title="NAVER로 이동!">NAVER</a>   
```
<a href="http://naver.com" title="NAVER로 이동!">NAVER</a>   

### 2-B. (Markdown) 링크에 커서 가져가는 경우 메모 보이기
```markdown
링크에 커서를 hovor한 경우 title 에 적은 메모가 보이게 하는 markdown 예제
[NAVER](http://naver.com "NAVER로 이동!") 
```
[NAVER](http://naver.com "NAVER로 이동!")


### 3. (HTML) 새탭에서 열기
```markdown
<a href="http://naver.com" title="NAVER로 이동!" target="_blank">NAVER</a>   
```
<a href="http://naver.com" title="NAVER로 이동!" target="_blank">NAVER</a>   



# 이미지(image) : 링크와 이미지 차이는 ! 가 있느냐만 차이
```markdown
이미지 넣기 : ![대체텍스트](이미지 url 주소)
이미지클릭시 url로 이동 : [이미지코드](url)
```

```plaintext
이미지 넣기 예제
```
![HEROPY](https://heropy.blog/css/images/logo.png)


```plaintext
이미지클릭시 url로 이동 예제
```
[![HEROPY](https://heropy.blog/css/images/logo.png)](https://heropy.blog)


# 인용문(BlockQuote)

> 남의 말이나 글에서 직접 또는 간접으로 따온 문장.  
> (네이버 국어 사전)

> 인용문을 작성하세요!
>> 중첩된 이용문
>>> 중중첩된 인용문 1  
>>> 중중첩된 인용문 2  
>>> 중중첩된 인용문 3  


# 인라인(inline) 코드 강조

CSS에서 `Background` 혹은 `background-image` 속성으로 요소에 배경이미지를 삽입할 수 있습니다.


# 블록(block) 코드 강조
```html
<a href="http://google.com" target="_blank">Google</a> 
```

```css
.list > li {
    position: absolute;
    top: 40px;
}
```

```javascript
function func() {
    var a = 'AAA';
    return a;
}
```

```bash
$ git commit -m 'Study Markdown'
```

```plaintext
동해물과 백두산이 마르고 닳도록  
하느님이 보우하사 우리나라 만세
```

# 표(TAble)

```markdown
왼쪽 정렬이 기본값
```
position 속성

값 | 의미 | 기본값
--|--|--
static | 기준 없음 | O
relative | 요소 자신 | X
absolute | 위치 상 부모 요소 | X
fixed | 뷰포트 | X

```markdown
가운데 정렬을 원하는 경우  |:--:|
컬럼2를 가운데 정렬 예시
```
값 | 의미 | 기본값
--|:--:|--
static | 기준 없음 | O
relative | 요소 자신 | X
absolute | 위치 상 부모 요소 | X
fixed | 뷰포트 | X

```plaintext
우측 정렬을 원하는 경우  |--:|
컬럼3를 우측 정렬 예시
```

값 | 의미 | 기본값
--|:--:|--:
static | 기준 없음 | O
relative | 요소 자신 | X
absolute | 위치 상 부모 요소 | X
fixed | 뷰포트 | X

# 원시 HTML (Raw HTML)
> markdown에서는 심플한 코드를 지양  
html의 문법을 그대로 사용하는 것이 원시 html 개념임

동해물과 <u>백두산</u>이 마르고 닳도록<br/>
하느님이 보우하사 우리나라 만세

동해물과 <span style="text-decoration: underline;">백두산</span>이 마르고 닳도록<br/>
하느님이 보우하사 우리나라 만세

> markdown 에서 지원하지 않는 기능이  
필요한 경우 원시 HTML 사용
- 예1. `a 태그`에서 `target 속성` 필요시
```html
<a href="http://naver.com" title="NAVER로 이동!" target="_blank">NAVER</a>   
```
- 예2. `img 태그`에서 `width 속성` 필요시
```html
<img width="70" src="https://heropy.blog/css/images/logo.png" alt="HEROPY" />   
```

# 수평선(Horizontal Rule)

---
***
___

