---
title:   "[Python] list.sort()와 sorted(list)의 차이점"
categories: 
  - Python
tags:
  - Python
  - Tips
toc: false
toc_sticky: false
toc_label: 
published: true
---

파이썬 기초문제를 풀던 중 아래와 같은 궁금점이 생겼습니다.  
문제는 아래와 같습니다.  
  
{: .notice}
List에 있는 값을 오름차순으로 정렬 하시오.  
```
$ input
data = [2, 4, 3, 1, 5, 10, 9]
```
저는 문제를 보고 별 생각없이  
'data.sort()를 data 에 다시 반환하는 형식으로 풀어야겠다.'  
'그럼 출력 시 [1, 2, 3, 4, 5, 9, 10] 이 출력될 것이다 ! '  
이라고 생각하고 아래와 같이 입력 했는데요.  
```
data = [2, 4, 3, 1, 5, 10, 9]  
data =  data.sort()  
print(data)
```  
값이 아래와 같이 출력 됐습니다.  
```
None
```  
여기서 궁금한 점이 생겼는데요!  
data.sort() 메서드는 데이터 타입이 list가 아니라 None인걸까요?  
None이라면 왜 None인지 또한 다른 메서드도 같은 데이터 타입인지 궁금해졌습니다.

### Python에서 `list.sort()`와 `sorted(list)`의 차이점에 대해 알아봅시다.
  
- **`list.sort()`**
```python
list.sort([reverse=<True|False>][, key=<function>])
```
  - **sort** 메서드는 리스트틑 정렬하는 함수입니다.  
  - 원본 리스트를 정렬하되 반환값은 'None'입니다.
  - 원본 리스트의 순서를 변경합니다. **(원본 리스트에 영향을 줍니다.)**

{: .notice}  
위에서 생겼던 궁금점이 여기서 해결되었습니다!  
sort 매서드는 리스트를 정렬하되, 반환값은 `'None'` 이므로  
위의 예제에서 data.sort()의 반환값인 data의 type과 반환값이 `'None'`으로 출력됬던 것입니다.  

- **`sorted(list)`**
```
sorted(iterable[, key=<function>][, reverse=<True|False>])
```
 - sort 매서드와 마찬가지로 리스트를 정렬하는 함수입니다.
 - 정렬된 새로운 리스트를 반환합니다. 
 - 원본 리스트의 순서를 변경하지 않습니다. **(원본 리스트에 영향을 주지 않습니다.)**
 - 모든 iterable에 동작합니다. (list, tuple, dict, 문자열 등)
  
sorted 를 예제를 통해 한번 확인해봅시다.
  
```
list = [1, 3, 2]
print(sorted(list))
# [1, 2, 3]
print(list)
# [1, 3, 2]
```
  
### 결론 및 요약
- `list.sort()` 매서드는 **원본 리스트의 순서를 변화**시킬 수 있습니다.
- `sorted(list)` 매서드는 **원본 리스트의 순서를 건드리지 않습니다.**
- `list.sort()` 매서드는 새로운 복사본을 만들지 않기 때문에 `sorted(list)` 매서드보다 빠릅니다.
  
{: .notice}
> 참고자료  
> - <https://docs.python.org/ko/3/howto/sorting.html>
> - <https://blog.naver.com/PostView.nhn?isHttpsRedirect=true&blogId=wideeyed&logNo=221745416992&redirect=Dlog&widgetTypeCall=true&directAccess=false>