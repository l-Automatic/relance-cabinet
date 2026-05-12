# relance-cabinet

Outil de relance client assisté par IA — démonstration pour cabinets d'expertise comptable.

## Stack
- HTML + CSS + JS vanilla, tout dans `index.html`
- Aucun framework, aucun backend, aucun fichier séparé

## Fonctionnalités
- Liste clients avec statut (Relance en attente / À jour / Non répondu)
- Fiche client avec email/tél éditables inline, ton IA, instructions IA
- Historique des relances par client
- 4 onglets de relance : TVA, Pièces manquantes, Bilan, Relance libre
- Mode démo : redirige tous les envois vers un email/SMS de test
- Génération de messages via API Claude (TODO)
- Envoi email via webhook n8n SMTP (TODO)
- Envoi SMS via API Twilio (TODO)

## Données
Les clients et historiques sont fictifs et codés en dur dans le JS.

## Constantes de configuration (haut du fichier JS)
- `DEMO_EMAIL` / `DEMO_PHONE` — destinations de test en mode démo
- `CLAUDE_API_KEY` — clé API Anthropic
- `N8N_WEBHOOK_URL` — URL webhook n8n pour l'envoi email
- `TWILIO_ACCOUNT_SID` / `TWILIO_AUTH_TOKEN` / `TWILIO_PHONE_FROM` — config SMS

## Design
Vert #1D9E75, fond #F8F9FA, cards blanches, border-radius 12px — cohérent avec dashboard-cabinet.
