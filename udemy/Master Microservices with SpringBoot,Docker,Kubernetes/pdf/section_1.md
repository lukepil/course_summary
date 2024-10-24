[메인 페이지로 가기](main.md)

# COURSE AGENDA (강의 계획)

## 설명:

이 섹션에서는 마이크로서비스 관련 강의에서 다룰 핵심 주제와 과정을 체계적으로 소개합니다. Spring Boot와 마이크로서비스의 개념을 중심으로, 마이크로서비스의 경계를 어떻게 정의하고 적절하게 크기를 조정하는지에 대한 내용이 포함되어 있습니다. 이 과정에서 중요한 주제는 마이크로서비스의 컨테이너화입니다. Docker를 사용하여 마이크로서비스를 컨테이너화하는 방법을 학습하며, 이 과정에서 컨테이너화의 필요성과 이점이 설명됩니다.

또한, Spring Cloud Config를 사용한 마이크로서비스의 설정 관리가 중요한 주제로 다뤄집니다. 여러 마이크로서비스가 개별적으로 설정을 관리해야 하기 때문에, 설정 관리 도구의 필요성이 크며, 이를 통해 전체적인 서비스 구조를 안정적으로 유지할 수 있습니다.

Service Discovery & Service Registration(서비스 검색 및 등록)은 마이크로서비스 환경에서 중요한 요소입니다. Eureka를 사용하여 각 마이크로서비스가 네트워크에서 발견될 수 있도록 구성하고, 자동으로 등록되는 구조를 만듭니다. 이는 대규모 마이크로서비스 아키텍처에서 필수적인 요소입니다.

강의는 또한 Spring Cloud Gateway를 사용한 엣지 서버 구축을 다룹니다. 엣지 서버는 사용자와 마이크로서비스 간의 게이트웨이 역할을 하며, 네트워크 성능과 보안을 높이는 데 중요한 역할을 합니다.

**복원력 강화(Resiliency Patterns)**도 언급됩니다. 마이크로서비스는 독립적이기 때문에 각 서비스가 고립된 문제를 해결할 수 있어야 합니다. 이를 위해 Resiliency Patterns는 서비스 장애 시 자동으로 복구하거나 최소한의 영향으로 문제를 해결하는 메커니즘을 제공합니다.

모니터링 및 가시성(Observability) 역시 중요한 주제입니다. Grafana와 Prometheus 같은 도구를 통해 마이크로서비스 상태를 실시간으로 모니터링하고, 성능 및 리소스 사용량을 분석하는 방법을 다룹니다. 이 과정은 시스템 안정성을 보장하고 문제를 신속하게 해결하는 데 필수적입니다.

강의 후반부에서는 OAuth2/OpenID와 Spring Security를 사용하여 마이크로서비스 보안을 강화하는 방법을 설명합니다. 마이크로서비스 간의 인증 및 권한 부여는 안전한 통신을 위해 필수적이며, 이를 통해 각 서비스가 안전하게 상호작용할 수 있습니다.

마지막으로, RabbitMQ, Kafka와 같은 메시지 브로커를 사용한 이벤트 기반(Event-Driven) 마이크로서비스의 구현 방법을 다룹니다. 이 방식은 시스템 간의 비동기 통신을 가능하게 하여, 각 서비스가 서로 독립적으로 동작할 수 있게 하며, 효율적인 데이터 전송을 지원합니다.

Kubernetes를 사용한 컨테이너 오케스트레이션도 주된 주제입니다. 다수의 컨테이너를 자동으로 배포하고 관리하며, 필요할 때마다 확장 및 축소할 수 있는 방법을 학습하게 됩니다.

## 중요 부분:

 • Spring Boot와 Docker를 사용하여 마이크로서비스를 적절하게 구성하고 관리하는 법.
 • Spring Cloud Config를 통해 분산된 마이크로서비스 설정을 중앙에서 관리하는 중요성.
 • Eureka를 사용한 서비스 검색 및 등록으로 마이크로서비스의 동적 관리.
 • Resiliency Patterns을 통한 마이크로서비스 복원력 강화.
 • OAuth2/OpenID와 Spring Security를 통한 안전한 마이크로서비스 통신.
 • RabbitMQ와 Kafka를 사용한 이벤트 기반 마이크로서비스의 구현.
 • Kubernetes로 마이크로서비스 컨테이너 오케스트레이션 관리.

## 결론:

이 강의는 Spring Boot와 Docker를 사용한 마이크로서비스 설계 및 구축, 그리고 이를 안정적으로 운영하기 위한 필수 도구 및 기법들을 학습합니다. 특히, Kubernetes를 통해 마이크로서비스를 자동으로 관리하고 확장하는 방법을 배우며, 실시간 마이크로서비스 개발자들이 사용하는 다양한 모범 사례를 이해할 수 있습니다.

[다음 섹션으로 가기](section_2.md)
