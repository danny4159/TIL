# markdown 문법

## 제목(heading)

#의 갯수를 바탕으로 제목의 레벨을 지정한다.

### 제목3

#### 제목4

##### 제목5

###### 제목6

## 목록

* 순서가 없는
* 목록
  * tab을 눌러서 하위 레벨로
  * 목록을 작성할 수 있습니다.
* 그리고, shift+tab을 통해서 상위 레벨로 갈 수 있습니다.

1. 순서가 있는
2. 목록
   1. 엔터누르고 tab하면 하위 레벨
      1. 한번 더
   2. shift+tab로 상위 레벨
3. 한번더 상위 레벨

## 코드 블럭 (이것때문에 markdown을 쓴다)

```java
system.out.println("hi");
// comment 
```

```python
print('hi')
# comment
// not comment
```

```html
<h1>
    제목
</h1>
<!-- comment-->
```

```bash
$ git init
```

`inline codeblock`

## 인용문

`>`를 통해서 인용문을 표현한다.

> 인용문

## 표

| 순번 | 이름   | 비고 |
| ---- | :----- | ---- |
| 1    | 홍길동 |      |
| 2    | 정규남 |      |
| 3    | 백승빈 |      |

## 이미지

![다니엘](C:\Users\danny\Desktop\다니엘.jpg)

![다니엘](C:%5CUsers%5Cdanny%5CDesktop%5CTIL%5Cmd-images%5C%EB%8B%A4%EB%8B%88%EC%97%98.jpg)

* typora에서 위의 설정을 하면, 상대경로로 이미지가 관리 된다.



## 링크

[구글](https://google.com)에서 검색을 잘하자 !



## 기타

*기울임(이탤릭)*

**굵게(볼드)**

~~취소선~~

---

