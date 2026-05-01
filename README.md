# Tech Challenge | NPS Preditivo em E-commerce

## 1. Objetivo do Projeto

Este projeto tem como objetivo identificar os principais fatores que impactam a satisfação do cliente (NPS) em um e-commerce, utilizando dados operacionais.

A proposta é transformar uma análise reativa (após a coleta do NPS) em uma abordagem proativa, permitindo antecipar problemas e apoiar decisões de negócio para melhorar a experiência do cliente.

---

## 2. Descrição da Base de Dados

A base contém informações operacionais relacionadas à jornada do cliente, incluindo:

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
- `customer_service_contacts`: Número de contatos do cliente com o atendimento  
- `resolution_time_days`: Tempo para resolução de problemas (em dias)  
- `complaints_count`: Número de reclamações registradas pelo cliente  
- `repeat_purchase_30d`: Indica se houve recompra em até 30 dias (0 = não, 1 = sim)  
- `csat_internal_score`: Score interno de satisfação do cliente  
- `nps_score`: Nota de satisfação do cliente (NPS), variando de 0 a 10  


Além disso, foi criada a variável:

- `classificacao`: categorização do NPS em:
  - Detratores (0–6)
  - Neutros (7–8)
  - Promotores (9–10)

---

## 3. Metodologia Utilizada

A análise foi conduzida com foco em negócio, seguindo as etapas:

### 3.1 Entendimento do problema
- Identificação do papel do NPS no e-commerce  
- Mapeamento das áreas impactadas (logística, atendimento, estratégia)  

### 3.2 Análise Exploratória de Dados (EDA)
- Distribuição das variáveis  
- Análise de correlação entre variáveis operacionais e NPS  
- Segmentação por classificação (Detratores, Neutros, Promotores)  

### 3.3 Identificação de padrões
- Comparação de métricas operacionais entre grupos  
- Análise de variáveis críticas (atraso, reclamações, tempo de resolução)  
- Identificação de ponto de ruptura na experiência  

---

## 4. Principais Resultados

- Atraso na entrega é o principal fator de impacto negativo no NPS  
- Clientes com mais reclamações tendem a ser detratores  
- Existe um ponto de ruptura a partir de aproximadamente 3 dias de atraso  
- A experiência do cliente é impactada pelo acúmulo de fricções ao longo da jornada  

---

## 5. Como Reproduzir a Análise

### Pré-requisitos

- Python 3.x  
- Bibliotecas:
  - pandas  
  - seaborn  
  - matplotlib  

Instalação:

```bash
pip install pandas seaborn matplotlib
