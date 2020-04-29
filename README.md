# digisos-alerts

Lager alerts for appene til team digisos

For mer informasjon om hvordan alerts fungerer, se: 
`https://doc.nais.io/observability/alerts`

### For NAV ansatte
Vi er tilgjengelige i slack-kanalen #digisos

## Utvikling:
Man kan bruke `https://prometheus.nais.preprod.local/graph` som hjelp til å teste queries (i image).

Bruk `dev/digisos-alerts-<namespace>.yaml` til å teste alerts i q0 eller q1. Varsler dukker da opp i `#digisos-alerts-dev` på Slack

### Apply til namespace i dev-sbs:
`kubectl apply -f dev/digisos-alerts-<namespace>.yml -n <namespace>`

### Apply prod-sbs:
`kubectl apply -f digisos-alerts.yml`
