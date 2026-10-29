# Monitor de Arquivos CNC

Monitora arquivos `.cnc` em uma pasta e altera velocidades de avanço (`F`) conforme o valor de exposição (`exp`) encontrado no arquivo.

## Funcionamento
- Verifica arquivos modificados recentemente.
- Identifica o valor de exposição e consulta a faixa de velocidades configurada.
- Substitui os valores de avanço definidos no script.
- Exibe as alterações realizadas e informa quando não há novas alterações.

## Configurações
- `ARQUIVOS_PROBLEMA`: pasta monitorada.
- `DIAS_VERIFICADOS`: período de arquivos considerados.
- `TEMPO_AUSENTE`: tempo sem alterações para exibir aviso.
- `v_fixa` e `faixa`: velocidades originais e velocidades de substituição.
- `validade`: data limite de execução do script.

## Dependências
Bibliotecas padrão do Python.

## Execução
```bash
python nome_do_script.py