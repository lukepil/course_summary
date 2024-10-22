[메인 페이지로 가기](main.md)

[이전 섹션으로 가기](section_10.md)

# 이벤트 기반 마이크로서비스 구축

## 설명:

이 섹션에서는 **이벤트 기반 마이크로서비스(Event-Driven Microservices)**의 구축 방법을 설명합니다. 특히, **비동기 통신(Asynchronous Communication)**을 통해 마이크로서비스 간의 통신을 최적화하는 방법과 시간 결합(Temporal Coupling) 문제를 피하는 방법을 다룹니다.

이벤트 기반 마이크로서비스는 주로 **이벤트 브로커(Event Brokers)**를 통해 퍼블리셔/구독자(Pub/Sub) 모델을 사용하여 이벤트를 전달합니다. RabbitMQ와 Apache Kafka는 널리 사용되는 이벤트 브로커 도구로, 이를 통해 이벤트를 퍼블리시하고 구독자들이 해당 이벤트를 처리할 수 있습니다.

Spring Cloud Function은 비즈니스 로직을 Java의 표준 함수 인터페이스(Supplier, Function, Consumer)로 구현하여, 비동기 이벤트 기반 마이크로서비스를 효율적으로 구축할 수 있습니다.

## 중요 부분:

	1.	이벤트 기반 모델: Pub/Sub 모델과 이벤트 스트리밍 모델을 통해 시스템 간 비동기 통신을 구현합니다.
	2.	RabbitMQ와 Kafka의 역할: RabbitMQ는 퍼블리셔/구독자 모델에 자주 사용되며, Kafka는 대규모 이벤트 스트리밍 처리에 유용합니다.
	3.	Spring Cloud Function: 비즈니스 로직을 자바 함수로 구현하고, 다양한 배포 환경에 맞춰 패키징할 수 있습니다.

## 결론:

이벤트 기반 마이크로서비스는 비동기 통신과 이벤트 브로커를 통해 시스템의 유연성을 극대화하고, 확장성과 복원력을 확보할 수 있습니다. RabbitMQ와 Kafka는 이러한 시스템을 지원하는 핵심 도구이며, Spring Cloud Function을 통해 비즈니스 로직을 함수로 구현할 수 있습니다.

[다음 섹션으로 가기](section_11-1.md)
