# Tech Challenge | NPS Preditivo em E-commerce

## Transformando dados operacionais em experiência do cliente

---

## Sobre o Projeto

Com o crescimento acelerado do e-commerce, garantir uma boa experiência do cliente se tornou um desafio operacional.

Neste projeto, atuei como cientista de dados com o objetivo de responder uma pergunta central:

**O que realmente impacta a satisfação do cliente — e como antecipar isso antes do NPS acontecer?**

A proposta foi sair do olhar reativo (pós-pesquisa) e evoluir para uma abordagem proativa, usando dados operacionais para prever e evitar insatisfação.

---

## Objetivo

Identificar os principais drivers de satisfação (NPS) e gerar insights acionáveis para apoiar decisões em:

- Logística  
- Atendimento  
- Experiência do cliente  

---

## Problema de Negócio

O NPS era coletado apenas ao final da jornada, limitando a capacidade de ação da empresa.

Mesmo com indicadores operacionais semelhantes, alguns clientes se tornavam promotores enquanto outros viravam detratores.

O desafio foi entender: **quais fatores realmente explicam essa diferença?**

---

## Principais Insights

### 1. Atraso na entrega é o principal driver de insatisfação

- Forte correlação negativa com o NPS  
- Quanto maior o atraso, menor a satisfação  

O atraso se mostrou como a principal alavanca de melhoria.

---

### 2. Reclamações são reflexo de falhas na jornada

- Detratores concentram mais reclamações  
- Indicam fricção acumulada na experiência  

---

### 3. Tempo de resolução impacta, mas menos

- Influência moderada  
- O problema maior é a ocorrência de falhas, não apenas o tempo de resolução  

---

## Ponto de Ruptura na Experiência

Foi identificado um limite claro de tolerância do cliente:

| Faixa de atraso | NPS médio |
|----------------|----------|
| 0–2 dias       | ~5.0     |
| 3–5 dias       | ~2.9     |
| 6+ dias        | ~0.8     |

A partir de aproximadamente 3 dias de atraso, há uma queda acentuada no NPS, caracterizando um ponto de ruptura na experiência.

---

## Perfil dos Clientes

### Promotores
- Entrega no prazo  
- Baixa ou nenhuma ocorrência de problemas  
- Experiência fluida  

### Detratores
- Atrasos na entrega  
- Necessidade de suporte  
- Problemas acumulados ao longo da jornada  

---

## Insight Estratégico

O cliente tende a tolerar pequenos problemas isolados, mas não tolera a fricção acumulada ao longo da experiência.

---

## Áreas Impactadas

- Logística  
- Atendimento  
- Experiência do cliente (CX)  
- Estratégia  

---

## Abordagem Analítica

- Análise exploratória de dados (EDA) orientada a negócio  
- Correlação entre variáveis operacionais e NPS  
- Segmentação de clientes (Detratores, Neutros e Promotores)  
- Identificação de padrões e pontos de ruptura  

---

## Tecnologias Utilizadas

- Python  
- Pandas  
- Seaborn  
- Matplotlib  
- Jupyter Notebook  

---

## Recomendações

- Reduzir entregas com atraso superior a 3 dias  
- Criar alertas para pedidos com risco de atraso  
- Priorizar clientes com múltiplas interações  
- Atuar preventivamente antes da insatisfação  

---

## Conclusão

O NPS se mostrou diretamente ligado à eficiência operacional, especialmente à logística e ao tratamento de problemas.

Ao antecipar falhas como atrasos e fricções no atendimento, é possível evoluir de uma abordagem reativa para uma estratégia proativa de experiência do cliente.

---

## Autores:

RM373099 - LUIZ GUILHERME GENUINO <br>
RM373570 - VICTOR BRYAN MOTA SILVA
