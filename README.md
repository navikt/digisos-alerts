# digisos-alerts

Lager alerts for appene til team digisos

For mer informasjon om hvordan alerts fungerer, se: 
`https://doc.nais.io/observability/alerts`

### For NAV ansatte
Vi er tilgjengelige i slack-kanalen #digisos

## Utvikling:
Man kan bruke `https://prometheus.nais.preprod.local/graph` som hjelp til å teste queries (i image).

Bruk `dev/digisos-alerts-<q0/q1>.yaml` til å teste alerts i q0 eller q1. Varsler dukker da opp i `#digisos-alerts-dev` på Slack

### Deploy dev:
Deploy digisos-alerts til riktig cluster i preprod:
`kubectl apply -f dev/digisos-alerts-<q0/q1>.yml`

### Deploy prod:
Deploy digisos-alerts til riktig cluster i prod:

`kubectl apply -f digisos-alerts.yml`
