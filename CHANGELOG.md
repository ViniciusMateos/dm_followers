# Changelog

## [1.0.1] — 2026-06-28

### Modificado
- update: caps de volume desligados por padrão (`MAX_DMS_DIA`/`HORA`/`POR_RUN` = 0) — manda pra todos os novos de uma vez; delays, janela e kill-switch seguem ligados

### Documentação
- docs: tabela de limites do README atualizada (caps desligados, delays atuais)

## [1.0.0] — 2026-06-26

### Adicionado
- feat: worker que manda DM pros novos seguidores lidos da aba de notificações
- Lê o feed de atividades (`PolarisActivityFeedStoriesViewQuery`) e filtra "começou a seguir você"
- Navegação humana: abre o perfil → cria a conversa → manda a DM, com dwells e pausas aleatórias
- Retomada: 1ª run começa do `COMECAR_DE`; salva o último e nos próximos runs só pega os novos
- Mensagem com o nick do destinatário (suporta spintax, mas configurada fixa)
- Caps por dia/hora/run, janela de horário, kill-switch de bloqueio e saldo final
- `--login`, `--import-cookies`, `--dry-run`, `--start-from`, `--start-from-oldest`, `--debug`
- Mensagens de erro explicativas (status HTTP em português)
