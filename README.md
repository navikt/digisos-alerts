# digisos-alerts

Lager alerts for appene til team digisos

For mer informasjon om hvordan alerts fungerer, se: 
`https://doc.nais.io/observability/alerts`

### For NAV ansatte
Vi er tilgjengelige i slack-kanalen #team_digisos

## Utvikling:
Man kan bruke `https://prometheus.nais.preprod.local/graph` som hjelp til å teste queries (i image) eller bruke [port forwarding](https://kubernetes.io/docs/tasks/access-application-cluster/port-forward-access-application-cluster/) mot Prometheus i dev.

Bruk `dev-<fss/gcp>-alerts.yml` til å teste alerts i et dev-cluster. De vil da alerts dukke opp i `#digisos-alerts-dev`.

## Autodeploy
Det er satt opp autodeploy av alle alerts ved push på main.

### Manuell apply i dev:
`kubectl apply -f dev-<fss/gcp>-alerts.yml`

### Manuell apply i prod:
`kubectl apply -f prod-<fss/gcp>-alerts.yml`
