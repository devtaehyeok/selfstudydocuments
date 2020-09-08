---
marp: true
header: EFFECTIVE JAVA
footer: "![](duck.png)  **written by thlim**"
pagenation : true
---
# EFFECTIVE JAVA

### Item 1 : 생성자 대신 정적 팩토리 메소드를 활용하라

```java
public static Boolean valueOf(boolean b){
    return b ? Boolean.TRUE : Boolean.False;
}
```
**팩토리 메서드 디자인 패턴과 무관.**
정적 팩토리 메소드의 장점 
1. 사용 필드 및 리턴 객체 설명 (가독성)
2. 매번 new object 리턴 불필요 
   - instance 관리에 유리함. (instance-controlled) a==b <=> a.equals(b);
   - immutable 클래스가 preconstruced 인스턴스를 사용할 수 있도록 해줌
   - singleton, noninstantiable 클래스 실현

---

3. return type 무관
   - 구현 클래스를 숨길 수 있음. 리턴만 바꾸면 됨. -> 컴팩트 API
   - interface-based frameworks




---