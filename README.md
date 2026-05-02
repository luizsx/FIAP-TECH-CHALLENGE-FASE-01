# Tech Challenge | NPS 

## Transformando dados operacionais em experiência do cliente

---

## 1. Sobre o Projeto

Com o crescimento acelerado das empresas, garantir uma boa experiência do cliente se tornou um desafio operacional.

Neste projeto, o objetivo foi responder a seguinte pergunta de negócio:

**O que realmente impacta a satisfação do cliente — e como antecipar isso antes do NPS acontecer?**

A proposta foi sair de uma visão reativa (analisar o NPS após a coleta) para uma abordagem proativa, utilizando dados operacionais para antecipar problemas e melhorar a experiência do cliente.

---

## 2. Objetivo

Identificar os principais fatores que impactam o NPS e gerar insights acionáveis para apoiar decisões em:

- Logística  
- Atendimento  
- Experiência do cliente  
- Estratégia  

---

## 3. Problema de Negócio

O NPS é coletado apenas ao final da jornada do cliente, o que limita a capacidade da empresa de agir preventivamente.

Mesmo com indicadores operacionais semelhantes, alguns clientes se tornam promotores enquanto outros se tornam detratores.

O desafio é entender quais fatores explicam essa diferença e como atuar antes da insatisfação acontecer.

---

## 4. Descrição da Base de Dados

A base contém informações operacionais e comportamentais da jornada do cliente.

### Variáveis disponíveis:

- `customer_id`: Identificador único do cliente  
- `order_id`: Identificador único do pedido  
- `customer_age`: Idade do cliente  
- `customer_region`: Região geográfica do cliente  
- `customer_tenure_months`: Tempo de relacionamento do cliente com a empresa (em meses)  
- `order_value`: Valor total do pedido  
- `items_quantity`: Quantidade de itens no pedido  
- `discount_value`: Valor de desconto aplicado ao pedido  
- `payment_installments`: Número de parcelas do pagamento  
- `delivery_time_days`: Tempo total de entrega (em dias)  
- `delivery_delay_days`: Quantidade de dias de atraso na entrega  
- `freight_value`: Valor do frete  
- `delivery_attempts`: Número de tentativas de entrega  
- `customer_service_contacts`: Número de contatos com o atendimento  
- `resolution_time_days`: Tempo para resolução de problemas (em dias)  
- `complaints_count`: Número de reclamações registradas  
- `repeat_purchase_30d`: Indica recompra em até 30 dias (0 = não, 1 = sim)  
- `csat_internal_score`: Score interno de satisfação  
- `nps_score`: Nota de satisfação do cliente (0 a 10)  

### Variável criada:

- `classificacao`: categorização do NPS:
  - Detratores (0–6)  
  - Neutros (7–8)  
  - Promotores (9–10)  

---

## 5. Metodologia

A análise foi conduzida com foco em negócio, seguindo as etapas:

### 5.1 Entendimento do problema
- Papel do NPS no e-commerce  
- Áreas impactadas (logística, atendimento, estratégia)

### 5.2 Análise Exploratória de Dados (EDA)
- Distribuição das variáveis  
- Análise de correlação  
- Segmentação por classificação de clientes  

### 5.3 Identificação de padrões
- Comparação entre detratores, neutros e promotores  
- Análise de variáveis críticas  
- Identificação de ponto de ruptura na experiência  

---

## 6. Principais Insights

- Atraso na entrega é o principal fator de impacto negativo no NPS  
- Clientes com mais reclamações tendem a ser detratores  
- Tempo de resolução tem impacto moderado  
- A experiência do cliente é afetada pelo acúmulo de fricções  

---

## 7. Ponto de Ruptura na Experiência

Foi identificado um limite claro de tolerância:

| Faixa de atraso | NPS médio |
|----------------|----------|
| 0–2 dias       | ~5.0     |
| 3–5 dias       | ~2.9     |
| 6+ dias        | ~0.8     |

A partir de aproximadamente 3 dias de atraso, há uma queda significativa na satisfação do cliente.

---

## 8. Perfil dos Clientes

### Promotores
- Entrega no prazo  
- Poucas ou nenhuma reclamação  
- Experiência fluida  

### Detratores
- Atrasos na entrega  
- Necessidade de suporte  
- Problemas acumulados  

---

## 9. Insight Estratégico

O cliente tende a tolerar pequenos problemas isolados, mas não tolera fricção acumulada ao longo da jornada.

---

## 10. Como Reproduzir a Análise

### Pré-requisitos

- Python 3.x  
- Jupyter Notebook ou Jupyter Lab  

Instale as dependências:

```bash
pip install pandas seaborn matplotlib notebook
```


## 11. Autores <br>
RM373099 - LUIZ GUILHERME GENUINO <br>
RM373570 - VICTOR BRYAN MOTA SILVA<br><br>


