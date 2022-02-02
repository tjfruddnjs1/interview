# REST

## URI vs URL

> URI는 식별하고, URL은 위치를 가르킨다.

- URI(Uniform Resource Identifier) : 자원의 위치뿐만 아니라 자원에 대한 고유 식별자로서, URL 의미를 포함
- URL(Uniform Resource Locator) : 자원이 실제로 존재하는 위치

> example

```
https://example.io : 서버를 나타내기 때문에 > URL O ,URI O
https://example.io/images : 서버 + images라는 네트워크 상의 자원의 위치 > URL O , URI O
https://example.io/images/dog.jpeg : 서버 + images 디렉터리 + dog.jpeg > URL O, URI O
https://example.io/user/123 : URL은 https://example.io/user , 원하는 정보에 도달하기 위한 식별자 123을 포함시 URI > URI O, URL X
https://example.io/profile?id=11 : URL은 https://example.io/profile , 원하는 정보에 도달하기 위한 식별자(여기서는 ?id=11)를 포함시 URI > URI O, URL X
```

## QUERYSTRING

> 사용자가 입력 데이터를 전달하는 방법중의 하나로, url 주소에 미리 협의된 데이터를 파라미터를 통해 넘기는 것

- ? 뒤에 = 로 연결된 key, value 형식
- 파라미터가 여러개일 경우 &를 붙여 여러개의 파라미터
- = 로 key, value 구분

## REST vs RESTful

> 웹에 존재하는 모든 자원(이미지, 동영상, DB 자원)에 고유한 URI를 부여해 활용

- 구성
1. 자원(URI)
2. 행위(HTTP Method)
3. 표현 : 자원의 표현 ex.JSON  

> `RESTful`이란 REST API의 설계 규칙을 올바르게 지킨 시스템

- 규칙
1. URI는 동사보다는 명사를, 대문자보다는 소문자
2. 마지막에 슬래시 (/)를 포함하지 않는다
3. 띄어쓰기, 언더바(_) 대신 하이픈(-)을 사용 > 가독성
4. 파일확장자는 URI에 포함하지 않는다
5. 행위(HTTP method)를 포함하지 않는다