# foco-estudantil-hackathon-dados
Projeto de mensuração baseado em uma ideia de Hackathon (2020), focado em foco, hábitos de estudo e procrastinação

##  Contexto
O objetivo deste projeto foi dar uma repaginada em uma ideia desenvolvida em um Hackathon em 2020, que na época ficou restrita a slides e à apresentação do pitch.

Em 2025, o projeto foi resgatado com um novo enfoque:
- Reestruturação da apresentação utilizando Gamma
- Criação do protótipo visual com apoio do Leonardo AI
- Construção de um dataset fictício para simular o comportamento de estudantes
- Modelagem e análise dos dados para geração de gráficos e métricas

A proposta central foi validar, por meio da mensuração de dados, a ideia de um “quadro de sonhos”
associado a recompensas visuais, conceito que na época da pesquisa mostrou influência psicológica
positiva na motivação e na formação de hábitos.

---

## Problema identificado 
Estudantes apresentam dificuldade em manter o foco nos estudos devido à procrastinação, distrações digitais e ausência de acompanhamento estruturado de hábitos.

A falta de métricas dificulta entender:
- Quando os alunos estudam mais
- Em quais condições o foco é maior
- Se recompensas realmente ajudam a reduzir a procrastinação

---

## Proposta 
A proposta do projeto é simular, por meio de dados, uma aplicação de acompanhamento de hábitos de estudo que permite mensurar:
- Tempo de foco
- Pausas durante as sessões
- Tempo de procrastinação
- Impacto de recompensas visuais no engajamento

Um dos conceitos centrais é o uso de um **“quadro de sonhos”**, baseado em pesquisas sobre motivação e reforço psicológico, no qual recompensas visuais ajudam a sustentar o foco e a construção de hábitos.

---

##  Estrutura do Dataset

### Tabela: usuarios
| Coluna     | Descrição                |
|------------|--------------------------|
| usuario_id | Identificador do usuário |
| nome       | Nome do usuário          |

---

### Tabela: sessoes_estudo
| Coluna     | Descrição                               |
|------------|-----------------------------------------|
| sessao_id  | Identificador da sessão                 |
| usuario_id | Relacionamento com usuários             |
| dia_semana | Dia da semana da sessão                 |
| recompensa | Recompensa associada à sessão de estudo |

---

###  Tabela: metricas_sessao
| Coluna             | Descrição                     |
|--------------------|-------------------------------|
| sessao_id          | Relacionamento com sessão     |
| tempo_foco_min     | Tempo de foco em minutos      |
| pausas             | Quantidade de pausas          |
| procrastinacao_min | Tempo gasto em procrastinação |

---

###  Tabela: dim_recompensa
| Coluna        | Descrição                   |
|---------------|-----------------------------|
| recompensa_id | Identificador da recompensa |
| descricao     | Tipo de recompensa          |

---

## Resumo

### 1️⃣ Quando as pessoas mais estudam?
- A maioria das sessões de estudo acontece no meio da semana.
- Quarta-feira e Sexta-feira concentram o maior número de sessões.
- Sábado e Domingo apresentam o menor volume de estudos registrados.

**Interpretação:** durante a semana há maior disciplina e rotina, enquanto o fim de semana tende a ser menos estruturado.

---

### 2️⃣ Em que dia o foco é melhor?
- O tempo médio geral de foco é de aproximadamente **35 minutos**.
- **Sábado** apresenta o maior tempo médio de foco (**40,5 minutos**).
- **Quinta-feira** vem logo em seguida.
- **Segunda-feira** é o dia com menor tempo médio de foco (**32,5 minutos**).

**Interpretação:** apesar de menos sessões no sábado, quando há estudo, o foco tende a ser maior.

---

### 3️⃣ A recompensa realmente ajuda?
A comparação entre sessões **com recompensa** e **sem recompensa** mostra diferenças claras:

| Métrica             | Sem Recompensa | Com Recompensa |
|---------------------|----------------|----------------|
| Tempo médio de foco | 32,8 min       | 38,2 min       |
| Pausas              | 2,7            | 1,4            |
| Procrastinação      | 24,6 min       | 9,2 min        |

**Conclusão prática:** o uso de recompensas aumenta o tempo de foco, reduz pausas e diminui significativamente a procrastinação.

---

### 4️⃣ Quem são os “campeões” de foco?
Os estudantes com maior tempo médio de foco foram:
- Pedro — **40,5 minutos**
- Ana — **40,0 minutos**
- Marcos — **36,7 minutos**
- Lucas — **35,5 minutos**
- Juliana — **35,0 minutos**

**Interpretação:** mesmo em um dataset fictício, é possível identificar padrões de desempenho individual.

---

##  Ferramentas Utilizadas
- Excel — criação do dataset fictício
- Power BI — modelagem de dados e visualização
- Gamma — repaginação da apresentação
- Leonardo AI — criação do protótipo visual
- GitHub — versionamento e documentação

---

##  Observação
As análises e interpretações foram realizadas com apoio de ferramentas de BI e Inteligência Artificial, com foco em desenvolver raciocínio analítico, estruturação de dados e comunicação de insights.

---

##  Autora
**Izabel Lima**  
Projeto desenvolvido para fins de estudo.
