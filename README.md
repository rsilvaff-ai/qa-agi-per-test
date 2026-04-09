# Teste de Performance - BlazeDemo

## Descrição
Automação de teste de performance para a compra de passagem aérea no site BlazeDemo.

## Cenário de Teste
- Compra de passagem aérea
- Critério de aceitação: 250 RPS, 90th percentile < 2s

## Requisitos
- Java 8+
- Apache JMeter 5.6.3+

## Execução
1. Abra o JMeter.
2. Carregue o arquivo `blazedemo_test_plan.jmx`.
3. Execute o teste (Load ou Peak test).
4. Os relatórios serão gerados em `results/`.

## Resultados Esperados
- Requisições por segundo: 250 RPS
- Tempo médio: < 2 s
- 90th percentile: < 2 s
- Erros: 0%

## Considerações
- Ajuste de threads foi necessário para atingir 250 RPS.  
- Teste de pico revela que acima de 300 threads a latência aumenta significativamente.