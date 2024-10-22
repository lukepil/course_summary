[메인 페이지로 가기](main.md)

[이전 섹션으로 가기](section_11-1.md)

# Spring Cloud Stream을 사용한 이벤트 생성 및 소비

## 설명:

이 섹션에서는 Spring Cloud Stream을 사용하여 마이크로서비스에서 이벤트를 생성하고 소비하는 방법을 설명합니다. StreamBridge 클래스는 Spring Cloud Stream 내에서 데이터를 출력 바인딩으로 보내는 역할을 합니다. 이벤트를 생성할 때, StreamBridge 클래스를 사용하여 이벤트를 원하는 출력 바인딩으로 전송할 수 있습니다.

예를 들어, **계정 마이크로서비스(Accounts Microservice)**에서 이벤트를 생성하고 소비하는 절차가 설명됩니다. 이벤트는 데이터베이스의 **통신 상태(Communication Status)**를 업데이트하는 방식으로 처리되며, 이러한 작업을 위한 코드 스니펫도 포함되어 있습니다.

이벤트를 소비하는 과정에서는 updateCommunication이라는 함수를 정의하고, 해당 함수가 RabbitMQ로부터 수신된 이벤트를 처리하도록 설정합니다. application.yml 파일에는 이벤트를 처리하기 위한 바인딩 설정이 포함되며, 이벤트가 올바르게 전송되고 소비되도록 바인딩 이름과 대상을 지정합니다.

또한, 이 섹션에서는 Apache Kafka와 RabbitMQ의 비교가 이루어집니다. Kafka는 대용량 데이터 스트리밍을 처리하기 위한 분산 이벤트 스트리밍 플랫폼이고, RabbitMQ는 메시지 브로커로서 더 복잡한 라우팅 요구사항을 처리할 수 있습니다.

## 중요 부분:

 1. StreamBridge를 사용하여 이벤트 생성: Spring Cloud Stream에서 StreamBridge를 사용하여 데이터를 바인딩된 출력으로 보낼 수 있습니다.
 2. Apache Kafka vs RabbitMQ: Kafka는 대용량 스트리밍 데이터에 적합하고, RabbitMQ는 복잡한 라우팅 요구 사항에 적합합니다.
 3. 이벤트 소비 함수 정의: updateCommunication과 같은 소비 함수를 통해 이벤트를 수신하고 처리합니다.

## 결론:

Spring Cloud Stream을 통해 마이크로서비스에서 비동기 이벤트 기반 통신을 처리할 수 있으며, StreamBridge를 사용해 이벤트를 생성하고, RabbitMQ 또는 Kafka를 통해 소비할 수 있습니다. Kafka는 대용량 데이터 스트리밍에 적합하고, RabbitMQ는 복잡한 라우팅 시나리오에 적합합니다.


[다음 섹션으로 가기](section_11-3.md)
