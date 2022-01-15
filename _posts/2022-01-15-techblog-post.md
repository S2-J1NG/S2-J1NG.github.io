---
layout: post
title: "드디어 시작하는 기술 블로그 개발일지"
category: tech
hash-tag: [Blog, jekyll]
---

gitpage로 블로그를 만들고 싶은 생각은 꽤 오랫동안 했지만, 기초적인 HTML, CSS 지식만 있어서 시작을 망설였다.
velog, 노션 등 여러 곳에 기록했더니 관리도 잘 안 되고, 무엇보다 내 기록에 내가 애착이 생기지 않았다.

그래서 고생스럽더라도 내가 직접 만들고 공부하면서 블로그를 만들어 가려고 한다. 🛠

## jekyll 실행 오류
```shell
`require': cannot load such file -- webrick (LoadError)
```

jekyll를 모두 설치하고 나서 `jekyll server` 를 실행하면 이런 문구가 뜨는데 ruby3.0.0. 버전부터 webrick이 빠져서 이런 에러가 난다.
webrick을 설치하고 서버를 실행하면 정상적으로 작동한다.

```shell
bundle add webrick
jekyll server
```

jekyll 테마를 적용하고 서버를 다시 실행할 때도 똑같이 webrick을 추가해야 한다. ([참고 블로그](https://junho85.pe.kr/1850))

이제 scss와 html 그리고 약간의 Js를 한다면 내 블로그도 보기 좋겠지... 지금은 원시 웹을 보고 있는 거 같다.👾