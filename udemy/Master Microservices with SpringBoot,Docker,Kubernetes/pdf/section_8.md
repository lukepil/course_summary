[메인 페이지로 가기](main.md)

[이전 섹션으로 가기](section_7.md)

# 마이크로서비스에서의 복원력 (Resiliency)

## 설명:

이 섹션은 **마이크로서비스의 복원력(Resiliency)**을 향상시키기 위한 다양한 패턴과 도구를 설명합니다. 특히 네트워크 문제나 서비스 장애 상황에서 어떻게 시스템의 안정성을 유지할 수 있는지를 다룹니다. 네트워크 문제나 서비스 장애가 발생할 경우, 복원력을 높이기 위해 다양한 패턴이 사용됩니다.

Hystrix는 한때 널리 사용된 복원력 패턴 구현 라이브러리였으나, 2018년 유지보수 모드에 들어갔습니다. 그 후 Resilience4j가 이를 대체하는 도구로 자리 잡았으며, 네트워크 문제나 서비스 장애에 대비한 경량의 오류 복원 라이브러리로 기능합니다.

Resilience4j는 다음과 같은 패턴을 제공합니다:

 1. 서킷 브레이커(Circuit Breaker): 서비스가 실패할 때 요청을 중단합니다.
 2. 폴백(Fallback): 요청이 실패할 경우 대체 경로를 제공합니다.
 3. 재시도(Retry): 서비스가 일시적으로 실패할 때 재시도합니다.
 4. 비율 제한(Rate Limiter): 일정 시간 내에 서비스가 받을 수 있는 호출 수를 제한합니다.
 5. 벌크헤드(Bulkhead): 하나의 서비스가 과부하가 되지 않도록 동시에 허용되는 요청 수를 제한합니다.

또한 Bulkhead 패턴은 소프트웨어 아키텍처에서 시스템 내의 각 컴포넌트가 서로 영향을 미치지 않도록 리소스 격리를 적용합니다. 이는 배가 침몰하지 않도록 구획을 나누는 것과 같은 개념으로, 하나의 서비스가 리소스를 과다하게 사용하더라도 다른 서비스에 영향을 주지 않게 합니다.

## 중요 부분:

 1. 서킷 브레이커와 폴백: 네트워크 문제나 서비스 장애 시 자동으로 요청을 중단하고, 대체 경로를 설정하여 서비스 장애를 최소화합니다.
 2. 벌크헤드 패턴: 하나의 서비스가 다른 서비스에 영향을 주지 않도록 격리하여, 리소스 소모를 방지하고 시스템의 안정성을 유지합니다.

## 결론:

Resilience4j와 같은 라이브러리를 통해 마이크로서비스의 복원력을 강화할 수 있으며, 서비스 간 리소스 격리를 통해 시스템 안정성을 높일 수 있습니다. 특히 벌크헤드 패턴을 적용하면 특정 서비스의 문제로 인해 전체 시스템이 영향을 받는 것을 방지할 수 있습니다.

[다음 섹션으로 가기](section_9.md)
