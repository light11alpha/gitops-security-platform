# Rapports de Vulnérabilités - Trivy Operator

## Résumé du cluster (dernier scan)
- Total CVEs : 485
- Critiques : 17
- Hautes : 170
- Moyennes : 261
- Faibles : 37

## Images analysées : 11

| Image | Critique | Haute | Moyenne |
|-------|----------|-------|---------|
| nginx:alpine (notre app) | 0 | 0 | 0 |
| argocd:v3.4.5 | 4 | 43 | 107 |
| dex:v2.45.0 | 5 | 42 | 19 |
| redis:8.2.3-alpine | 2 | 9 | 1 |
| coredns:1.14.4 | 0 | 10 | 6 |
| metrics-server:v0.8.1 | 2 | 12 | 8 |
| kyverno:v1.18.2 | 0 | 4 | 5 |
| trivy-operator:0.32.0 | 0 | 2 | 1 |

## Conclusion
Notre application métier (nginx:alpine) est sans vulnérabilité. Les CVEs détectées concernent les outils système (ArgoCD, k3s) et doivent être traitées via des mises à jour upstream.
