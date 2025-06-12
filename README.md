# 📉 Análise de Evasão de Clientes (Churn)

Este projeto tem como objetivo **identificar os fatores que levam clientes a cancelarem os serviços** de uma empresa de telecomunicações. Com base nos dados fornecidos, realizamos uma análise exploratória detalhada, buscando insights que ajudem a empresa a **reduzir a evasão e melhorar a retenção de clientes**.

---

## 🧰 Tecnologias Utilizadas

- 🐍 **Python 3.11**
- 📊 **Pandas** – manipulação e limpeza de dados
- 🎨 **Seaborn** & **Matplotlib** – criação de gráficos
- 💻 **Google Colab** – ambiente de análise
- 🔄 **JSON + `json_normalize()`** – leitura e tratamento de dados aninhados

---

## 🗂️ Etapas do Projeto

### 📥 Extração
- Os dados foram obtidos a partir de um repositório no GitHub, no formato `.json`.
- Foram importados manualmente para o Google Colab e normalizados com `pandas.json_normalize()`.

### 🧹 Tratamento de Dados
- Remoção de valores inválidos (224 registros com `Churn` vazio);
- Conversão de colunas numéricas (`Charges.Monthly`, `Charges.Total`);
- Padronização de valores categóricos e correção de inconsistências;
- Verificação de duplicatas e valores ausentes.

### 🔎 Análise Exploratória
Analisamos a evasão com base em diferentes categorias de dados:

| Grupo               | Variáveis analisadas                              |
|---------------------|----------------------------------------------------|
| Fidelidade          | Tipo de contrato, tempo de permanência (`tenure`) |
| Perfil do cliente   | Idoso, parceiro(a), dependentes                   |
| Financeiro          | Gastos mensais, forma de pagamento                |
| Serviços contratados| Suporte técnico, TV, segurança, backup            |

Gráficos em português foram gerados com visual limpo e cores suaves, focando em clareza para relatórios e apresentações.

---

## 📊 Principais Insights

- 📆 **Contratos mensais** têm taxa de churn muito mais alta que contratos anuais ou bienais;
- 💸 Clientes com **pagamento automático (débito)** cancelam com mais frequência;
- 🧓 **Idosos** e pessoas **sem suporte técnico** tendem a evadir mais;
- 🛡️ **Serviços adicionais** como backup, segurança e suporte ajudam na retenção.

---

## 📝 Conclusão

A análise mostrou que **contratos curtos, ausência de serviços complementares e métodos de pagamento automáticos** estão ligados à evasão. Com esses dados, a empresa pode:

- Criar campanhas para incentivar **contratos mais longos**;
- Investir em **comunicação clara sobre os benefícios de suporte técnico**;
- Reavaliar a **experiência com débito automático**.

---

## ✨ Autora

> Desenvolvido por Vitória de Lima Santos   
> Apaixonada por dados, tecnologia e entender o comportamento dos usuários.  
> Em formação contínua na área de Data Science.
