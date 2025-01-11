# Análise de Hipóteses e Teste A/B para Aumento de Receita

## Descrição do Projeto

Este projeto tem como objetivo analisar e priorizar hipóteses para aumento de receita em uma grande loja online e realizar uma análise detalhada de um teste A/B, utilizando técnicas estatísticas e frameworks de priorização.

---

## Contexto

Você, como analista de dados, foi responsável por:
1. Priorizar uma lista de hipóteses elaborada em conjunto com o departamento de marketing.
2. Analisar os resultados de um teste A/B para tomar uma decisão informada sobre a implementação de mudanças.

---

## Estrutura do Projeto

### Parte 1: Priorização de Hipóteses

O arquivo `hypotheses_us.csv` contém nove hipóteses com os seguintes campos:
- **Hypotheses**: Descrição breve da hipótese.
- **Reach**: Alcance do usuário (escala de 1 a 10).
- **Impact**: Impacto nos usuários (escala de 1 a 10).
- **Confidence**: Confiança na hipótese (escala de 1 a 10).
- **Effort**: Recursos necessários para testar a hipótese (escala de 1 a 10).

#### Tarefas:
1. Aplicar o framework **ICE** para priorizar as hipóteses e classificá-las em ordem decrescente de prioridade.
2. Aplicar o framework **RICE** e comparar os resultados com o ICE, explicando as mudanças nas prioridades.

---

### Parte 2: Análise do Teste A/B

Os arquivos `orders_us.csv` e `visits_us.csv` foram utilizados para realizar a análise do teste A/B, que contém:
- **Orders**: Informações sobre pedidos, incluindo receita, data e grupo (A ou B).
- **Visits**: Dados diários de visitas por grupo.

#### Tarefas:
1. **Receita Acumulada**:
   - Gráfico da receita acumulada por grupo.
   - Conclusões e conjecturas sobre as tendências observadas.

2. **Tamanho Médio do Pedido**:
   - Gráfico do tamanho médio acumulado do pedido por grupo.
   - Análise da diferença relativa entre os grupos.

3. **Taxa de Conversão**:
   - Calcular e traçar as taxas de conversão diárias de cada grupo.
   - Analisar as diferenças e a conversão acumulativa.

4. **Identificação de Anomalias**:
   - Definir anomalias com base nos percentis 95 e 99 para pedidos por usuário e preços.
   - Gráficos de dispersão para identificar outliers.

5. **Significância Estatística**:
   - Comparar conversão e tamanho médio dos pedidos entre os grupos com e sem dados filtrados.
   - Realizar testes de hipótese para validar diferenças.

6. **Tomada de Decisão**:
   - Com base nos resultados, decidir entre: 
     - **Interromper o teste e considerar um grupo como vencedor.**
     - **Interromper o teste sem considerar diferenças.**
     - **Continuar o teste.**

---

## Conclusão

Após a análise, a decisão foi **interromper o teste**, com as seguintes justificativas:
- O grupo **B** apresentou desempenho inferior ao grupo **A**.
- Não houve diferença significativa na conversão de pedidos.
- O tamanho médio dos pedidos do grupo **B** foi **4% menor** que o grupo **A**.

Recomendação final: **manter o grupo A como versão oficial.**

---

## Estrutura de Arquivos

- `/datasets/hypotheses_us.csv`: Hipóteses com parâmetros de priorização.
- `/datasets/orders_us.csv`: Dados de pedidos do teste A/B.
- `/datasets/visits_us.csv`: Dados de visitas do teste A/B.

---

## Tecnologias Utilizadas

- Python
- Pandas, NumPy
- Matplotlib, Seaborn
- Testes estatísticos: Scipy

---

## Como Utilizar

1. Clone este repositório.
2. Certifique-se de que os arquivos de dados estão na pasta `/datasets`.
3. Execute o script principal para reproduzir os resultados.

Autor
[Danilo José](https://www.linkedin.com/in/danilojosedelara/)

Projeto desenvolvido como parte de um curso de análise de dados.
