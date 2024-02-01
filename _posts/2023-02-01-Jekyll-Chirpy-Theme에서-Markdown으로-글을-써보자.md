---
categories: [기타, 블로그] #대분류 소분류
tags: [jekyll, chirpy, markdown] #무제한으로 설정 가능. 모두 lower case로 입력
image: https://i.esdrop.com/d/ZklKfna5T3.jpg #게시글 프리뷰 이미지
---

<!-- https://chirpy.cotes.page/posts/write-a-new-post/#images -->

Jekyll Chirpy Theme을 활용하여 깃허브 블로그를 구축했다. 앞으로 블로그를 활용함에 있어서 두고두고 유용할 마크다운 문법에 대해 기록해둔다.

> 주의. 일반적인 마크다운 문법에 더해 Jekyll Chirpy에서 적용되는 사항도 함께 적었기 때문에 착오가 생기지 않도록 주의하세요.

## Front Matter
포스트의 맨 위에 아래와 같은 정보를 입력해야 한다.
```markdown
---
title: TITLE # 파일명으로 대체 가능
date: YYYY-MM-DD HH:MM:SS +/-TTTT # 파일명으로 대체 가능
categories: [TOP_CATEGORIE, SUB_CATEGORIE]
tags: [TAG] # TAG names should always be lowercase
---
```

## 제목
제목은 아래와 같이 표기한다.
```markdown
# h1(오른쪽 Contents 인덱스에 표기 X)
## h2(오른쪽 Contents 인덱스에 표기 O)
### h3(오른쪽 Contents 인덱스에 h2 하위로 표기 O)
```

## 글씨체 및 인용
보통글씨
```markdown
보통글씨
```

*이탤릭*
```markdown
*이탤릭*
```

**볼드**
```markdown
**볼드**
```

~~취소선~~
```markdown
~~취소선~~
```

> 인용은 이와 같이 사용합니다.

```markdown
> 인용은 이와 같이 사용합니다.
```

## 리스트
### Unordered List
- A
- B
- C

### Ordered List
1. A
2. B
3. C

## 이미지
![](https://i.esdrop.com/d/ZklKfna5T3.jpg)
_강아지 사진 설명_
![](https://i.esdrop.com/d/ZklKfna5T3.jpg){: .shadow}
_그림자가 적용된 사진_

```markdown
![](https://i.esdrop.com/d/ZklKfna5T3.jpg)
_강아지 사진 설명_
![](https://i.esdrop.com/d/ZklKfna5T3.jpg){: .shadow}
_그림자 효과가 적용된 사진_
```

## 코드블록
<!-- 코드 언어를 나오게 할 수도 있다.(소문자로 해야하는듯) -->
```markdown
```c++
int a = 10;
int b = 5;
int c = a + b;
printf(c);
```
```

## Youtube embed
{%include embed/youtube.html id="jNQXAC9IVRw" %}
> 왜인지 모르겠지만 코드 블록으로 마크다운으로 쓴 게 그대로 보이지 않음.