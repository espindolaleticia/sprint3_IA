# Relatório de modelos e parâmetros — Sprint 03

## Parâmetros controlados

- `temperature`: `0.2`
- `top_p`: `0.9`
- `max_tokens` / `num_predict`: `350`
- Modelo principal: `gpt-oss:120b`
- Modelo comparativo: `gpt-oss:20b`
- Prompts comparados: `v1` e `v2`

## Comparativo executado

| Modelo | Prompt | Qualidade no mini-eval | Latência média | Status |
|---|---|---:|---:|---|
| gpt-oss:120b | v1 | 75.00% | 1009.83 ms | OK |
| gpt-oss:120b | v2 | 75.00% | 911.18 ms | OK |
| gpt-oss:20b | v1 | 62.50% | 3060.98 ms | OK |
| gpt-oss:20b | v2 | 75.00% | 2736.78 ms | OK |

## Leitura dos resultados

Use a combinação com maior aderência ao eval e latência aceitável como justificativa do modelo/prompt principal. Se o segundo modelo não estiver disponível na conta Ollama, altere `MODEL_NAME_2` no `.env` para outro modelo acessível e execute novamente.