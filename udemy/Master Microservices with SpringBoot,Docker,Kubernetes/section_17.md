[메인 페이지로 가기](main.md)

[이전 섹션으로 가기](section_16.md)

# Section 17 - Server-Side Service Discovery and Load Balancing Using Kubernetes

## 설명
이 섹션에서는 Kubernetes의 네트워크 관련 기능을 활용하여 서버 측에서 서비스 디스커버리와 로드 밸런싱을 구현하는 방법을 설명합니다. 마이크로서비스 환경에서 서버 간 통신을 효율적으로 처리하기 위해 Kubernetes의 클러스터 내에서 서비스를 자동으로 탐색하고, 부하를 여러 서비스 인스턴스에 분산시키는 로드 밸런싱 전략을 배웁니다.

## 내용
 1. **Kubernetes의 서비스 디스커버리**: Kubernetes 클러스터 내부에서 서비스 디스커버리는 자동으로 처리됩니다. 각 서비스는 Service 리소스를 통해 클러스터 내부에 자신을 등록하며, Kubernetes DNS를 통해 다른 서비스가 해당 서비스를 탐색할 수 있습니다. 이 방식은 Eureka와 같은 서비스 디스커버리 도구를 사용하지 않아도, Kubernetes 자체에서 서비스를 자동으로 탐색하고 통신할 수 있게 합니다.
 2. **로드 밸런싱**: Kubernetes는 Service 객체에 로드 밸런싱 기능을 내장하고 있어, 클러스터 내에서 여러 개의 서비스 인스턴스 간에 트래픽을 분산시킵니다. 클라이언트의 요청이 들어오면, Kubernetes는 이를 적절한 인스턴스에 라우팅하며, 이를 통해 트래픽을 고르게 분배하고, 특정 인스턴스에 과도한 부하가 걸리는 것을 방지합니다. 특히 ClusterIP 및 NodePort 서비스 타입을 통해 클러스터 내 또는 외부에서 요청을 받을 수 있습니다.
 3. **External Load Balancers**: Kubernetes는 외부 트래픽을 관리하기 위한 외부 로드 밸런서를 지원합니다. 클라우드 제공업체의 로드 밸런서를 활용하여, 클러스터 외부에서 들어오는 요청도 클러스터 내 서비스로 적절히 분배될 수 있도록 설정합니다. 이를 통해 대규모 외부 트래픽이 들어오더라도 서비스 가용성을 유지할 수 있습니다.

## 결론
Kubernetes는 서버 측에서 자동으로 서비스 디스커버리와 로드 밸런싱을 처리하는 강력한 기능을 제공합니다. 이를 통해 마이크로서비스 간 통신을 간소화하고, 트래픽을 적절하게 분산시켜 시스템의 확장성과 가용성을 높일 수 있습니다. 외부 로드 밸런서를 통해 클러스터 외부 트래픽도 효율적으로 처리할 수 있습니다.

[다음 섹션으로 가기](section_18.md)