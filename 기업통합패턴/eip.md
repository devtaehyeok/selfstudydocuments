# Enterprise Integration Patterns

카멜의 EIP에 대해 분석한 문서

- 카멜 용어정리
1. component
-   메세징, 데이터 전송, 알림 등 서비스 제공 객체
-  ActiveMQ, AWS DynaomDB 같은 서비스.





목차
1. 메세징 시스템
2. 메세징 채널
3. 메세지 구성
4. 메세지 라우팅
5. 메세지 트랜스폼
6. 메세지 엔드포인트
7. 시스템 관리


## 1. 메세징 시스템
### 1. 메세지 채널
    An enterprise has two separate applications that need to communicate, preferably by using Messaging.
    : 어떻게 어플리케이션이 메세지를 사용하여 다른 어플리케이션과 커뮤니케이션 하는가?

![](/images/eip/eip_112630.png)

한 응용 프로그램이 채널에 정보를 쓰고 다른 응용 프로그램이 해당 정보를 채널에서 읽는 메시지 채널을 사용하여 응용 프로그램을 연결한다.

송신 app은 
단지 메세징 시스템에 정보를 넣는게 아니라,
특정 메세지 체널에 메세지를 추가하고, 수신 app은 특정 메세지 채널에서 정보를 검색한다.

### `카멜 구현`

```xml
<route>
  <from uri="direct:foo">
  <to uri="jms:queue:foo"/>
</route>
```