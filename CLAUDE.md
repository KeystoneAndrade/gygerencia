# GyGerencia

## Regras invioláveis

- **NUNCA** alterar a chave do `localStorage` (`STORAGE_KEY`), migrar dados, limpar via `removeItem`/`clear`, ou rodar qualquer código que sobrescreva os dados existentes no dispositivo do usuário. Os dados financeiros do usuário vivem só ali — qualquer reset apaga tudo de forma irreversível.
- Não introduzir lógica de "seed", "reset", ou "limpar dados antigos" no boot do app.
- Mudanças no formato dos dados devem ser feitas como migrações aditivas e idempotentes que preservam o conteúdo existente.
