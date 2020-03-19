# digisos-alerts

Lager alerts for appene til team digisos

For mer informasjon om hvordan alerts fungerer, se: 
`https://doc.nais.io/observability/alerts`

### For NAV ansatte
Vi er tilgjengelige i slack-kanalen #digisos

## Utvikling:
En kan bruke `https://prometheus.nais.preprod.local/graph` som hjelp til å teste queries (i image).

Bruk `dev/digisos-alerts-dev.yaml` til å teste alerts i dev. Varsler dukker da opp i `#digisos-alerts-dev` på Slack

### Deploy dev:
Deploy digisos-alerts til riktig cluster i preprod:
`kubectl apply -f dev/digisos-alerts-dev.yml`

### Deploy prod:
Deploy digisos-alerts til riktig cluster i prod:

`kubectl apply -f digisos-alerts.yml`
