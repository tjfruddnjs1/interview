# PAGINATION

## LIMIT, OFFSET

- LIMIT : 행의 개수를 제한
- OFFSET : 행의 index를 제한(어디서 부터 시작할지)

- 페이징 구현 구성요소 
1. 현재 페이지 넘버 : (현재 페이지 넘버 - 1) * 페이지 사이즈 = OFFSET (0부터 시작)
2. 페이지 사이즈
3. 전체 갯수