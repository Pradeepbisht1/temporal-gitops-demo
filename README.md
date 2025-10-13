# Temporal HA via Argo CD — Personal Demo Repo

Use this repo to demo your work without org access. At 5 PM, show:
1) Argo CD UI: Create `postgres-temporal-dev` and `temporal-ha-dev` from `argocd-apps/*.yaml` OR by using the UI with the same fields.
2) Values: base + overlay pattern under `base/helm-chart/temporal/` and `overlays/dev/temporal/`.
3) Infra resources: namespaces + DSN secret under `k8s/` (in the org, these will live in Infra_k8s/Resources/Temporal).

Folders
- base/helm-chart/temporal/values.yaml — default values
- overlays/dev/temporal/values.yaml — dev overrides
- k8s/ — namespaces + DSN secret
- argocd-apps/postgres-temporal-dev.yaml — App pointing to Bitnami Postgres HA (inline values)
- argocd-apps/temporal-ha-dev.yaml — App pointing to official Temporal chart (inline values)
# temporal-gitops-demo
