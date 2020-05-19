# digisos-alerts

Lager alerts for appene til team digisos

For mer informasjon om hvordan alerts fungerer, se: 
`https://doc.nais.io/observability/alerts`

### For NAV ansatte
Vi er tilgjengelige i slack-kanalen #digisos

## Utvikling:
Man kan bruke `https://prometheus.nais.preprod.local/graph` som hjelp til å teste queries (i image) eller bruke [port forwarding](https://kubernetes.io/docs/tasks/access-application-cluster/port-forward-access-application-cluster/) mot Prometheus i dev-sbs.

Bruk `dev-alerts.yml` til å teste alerts i dev-sbs. Varslene vil gjelde for alle namespaces i dev-sbs, og de skal dukke opp i `#digisos-alerts-dev`.

## Autodeploy
Det er satt opp autodeploy av alertene ved push på master.

### Manuell apply i dev-sbs:
`kubectl apply -f dev-alerts.yml`

### Manuell apply i prod-sbs:
`kubectl apply -f prod-alerts.yml`
