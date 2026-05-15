# gitops-config  Config Repository

## 역할
Kubernetes 매니페스트만 관리함. 소스 코드 없음.
: k8s 로컬 3노드 (VirtualBox/UTM)
동일 구조 재사용.

## 구조
apps/spring-boot/
  base/         공통 매니페스트 (Kustomize base)
  overlays/
    dev/        dev 환경
    staging/    staging 환경
    prod/       prod 환경
argocd/         ArgoCD 리소스 정의
