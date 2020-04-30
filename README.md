# digisos-alerts

Lager alerts for appene til team digisos

For mer informasjon om hvordan alerts fungerer, se: 
`https://doc.nais.io/observability/alerts`

### For NAV ansatte
Vi er tilgjengelige i slack-kanalen #digisos

## Utvikling:
Man kan bruke `https://prometheus.nais.preprod.local/graph` som hjelp til å teste queries (i image).

Bruk `dev/digisos-alerts-dev.yaml` til å teste alerts i dev-sbs. Varslene vil gjelde for alle namespaces i dev-sbs, og de skal dukke opp i `#digisos-alerts-dev`.

### Apply i dev-sbs:
`kubectl apply -f dev/digisos-alerts-dev.yml`

### Apply i prod-sbs:
`kubectl apply -f digisos-alerts.yml`
