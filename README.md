# Site Change Monitor Template

Este template monitora mudanças em páginas web e envia alertas no Slack.

## Páginas monitoradas

- https://olist.com/
- https://olist.com/planos/

## Como usar

1. Faça fork deste repositório ou clone.
2. Adicione um secret no GitHub Actions:
    - **SLACK_TOKEN** → seu token de bot do Slack
3. O workflow roda diariamente (pode ser ajustado no `.github/workflows/site-monitor.yml`).
4. Se alguma página mudar, você receberá um alerta no canal configurado.

## Customização

- Para adicionar/remover URLs, edite `check_site.py`, lista `URLS`.