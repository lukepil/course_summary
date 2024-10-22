[메인 페이지로 가기](main.md)

[이전 섹션으로 가기](section_11-2.md)

# Apache Kafka와 RabbitMQ 비교 및 교체

## 설명:

이 섹션에서는 Apache Kafka와 RabbitMQ의 차이점과 Apache Kafka를 사용하여 RabbitMQ를 대체하는 방법을 설명합니다. Kafka는 대규모 스트리밍 데이터 처리를 위한 분산 이벤트 스트리밍 플랫폼이며, 실시간 데이터 스트림을 처리하는 데 특화되어 있습니다.

### Kafka의 주요 구성 요소는 다음과 같습니다:

	1.	Producers: Kafka 주제(Topic)에 메시지를 게시하는 역할을 합니다. Producers는 특정 주제에 메시지를 작성하고, Kafka는 이를 주제의 로그에 추가합니다.
	2.	Topics: Kafka에서 데이터를 조직하는 단위로, 여러 파티션으로 나뉘어 병렬 처리와 부하 분산을 지원합니다.
	3.	Brokers: Kafka 서버로, 주제의 저장과 복제를 관리하며, Producers로부터 메시지를 수신하여 Offset을 할당하고, 이를 Consumers에게 제공합니다.
	4.	Partitions: 주제를 여러 파티션으로 나누어 병렬 처리와 부하 분산을 가능하게 합니다. 각 파티션은 메시지의 순차적 로그를 보관합니다.
	5.	Offsets: 각 파티션 내에서 고유한 메시지 식별자로, Consumers가 메시지를 처리한 상태를 추적하는 데 사용됩니다.
	6.	Replication: 주제를 여러 Brokers에 복제하여 장애 복구 및 고가용성을 보장합니다.
	7.	Consumers: Kafka 주제에서 메시지를 읽고, 메시지를 처리하는 역할을 합니다.

Kafka와 RabbitMQ의 차이점은 Kafka가 주로 대규모 스트리밍 데이터 처리에 적합하고, RabbitMQ는 더 복잡한 라우팅 요구를 처리할 수 있다는 점입니다. Kafka는 주로 고속 데이터 스트림을 다루며, 데이터를 분산 시스템에서 복제하고 소비하는 데 강점을 보입니다.

이 섹션에서는 Kafka를 사용하여 RabbitMQ를 대체하는 방법을 단계별로 설명합니다. Kafka 관련 Maven 의존성을 추가하고, application.yml 파일에 Kafka 관련 설정을 정의하는 방식으로 구성됩니다. Kafka와의 통합을 통해 마이크로서비스의 이벤트 스트리밍을 확장할 수 있습니다.

## 중요 부분:

	1.	Kafka 구성 요소: Producers, Topics, Brokers, Partitions, Offsets, Replication 등 Kafka의 핵심 개념을 설명합니다.
	2.	Kafka vs RabbitMQ: Kafka는 대용량 스트리밍 데이터에 최적화된 반면, RabbitMQ는 복잡한 메시지 라우팅을 처리하는 데 적합합니다.
	3.	Kafka를 통한 RabbitMQ 대체: Kafka 의존성을 추가하고 application.yml 파일에 Kafka 관련 설정을 적용하여 RabbitMQ를 대체하는 방법을 설명합니다.

## 결론:

Apache Kafka는 대규모 스트리밍 데이터 처리에 강점을 지닌 분산 이벤트 스트리밍 플랫폼으로, RabbitMQ에 비해 더 큰 규모의 데이터 흐름을 처리할 수 있습니다. Kafka를 활용해 이벤트 스트리밍을 구성하면, 실시간 데이터를 고속으로 처리하고, 고가용성과 복구 기능을 보장할 수 있습니다.

[다음 섹션으로 가기](section_11-3.md)
