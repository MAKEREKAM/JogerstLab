# JogerstLab
YouTube 검색창에 '요거스트'라는 단어를 입력할 시 발생하는 추천 검색어에 대한 연구

## 규칙

- `요거스트`라는 단어를 입력했을 때 나오는 추천 검색어들을 요거스트로 부른다.
- 요거스트 또는 요거스트 + ` `를 입력했을 때 나오는 요거스트들을 하위 요거스트로 부른다.
- 최상위 요거스트는 `요거스트`로 한다.
- 알고리즘의 영향을 받고 생성되는 '작위 요거스트'와 시크릿 모드에서 발생하는 '무작위 요거스트'를 구분한다.
- 하위 요거스트를 생성하지 않는 최하위 요거스트를 구분한다.
- 자신의 하위 요거스트가 자신을 생성하는 순환 요거스트를 구분한다.
- 자신을 하위 요거스로 가지는 재귀 요거스트를 구분한다.

## 무작위 요거스트
```
- 요거스트
  - unitychantoonshader
    - unitychantoonshader (재귀)
  - onphotonserializeview
    - onphotonserializeview (재귀)
    - wemission
      - wemission (재귀)
      - ic_franej6bg
        - ic_franej6bg (재귀)
- loggamja
  - unitychantoonshader
  - ic_franej6bg
```
