# 📦 Dashboard de Eficiência de Transportes

> Versão com **dados sintéticos** de um painel que desenvolvi e que foi usado nas apresentações de performance para a **gerência e os gestores da operação de transportes**.

![Dashboard Logístico](images/demonstração.gif)

---

## 🎯 Perguntas que o painel responde

- 🕒 **Pontualidade:** as transportadoras chegam no horário agendado para carregamento?
- 🚛 **Volume por perfil de veículo:** quais tipos de veículo mais carregam?
- 🏭 **Volume por CD e por transportadora:** onde está concentrada a operação (Pareto 80/20)?
- 💰 **Custo de frete por transportadora:** quem mais pesa no custo e como isso evolui no tempo?

---

## 🧱 Estrutura do Projeto

```
dashboard-logistica/
├── data/
│   └── base de dados.xlsx        # Base sintética (~11 mil ordens de coleta)
├── images/
│   ├── dashboard.jpg             # Screenshot do painel
│   └── demonstração.gif          # Demonstração navegando no painel
├── src/
│   └── Dashboard_Logístico.pbix  # Arquivo do Power BI
└── README.md
```

---

## 📊 Destaques do Dashboard

- **Pareto 80/20 de volume e de frete por transportadora**
- **Pontualidade na chegada ao CD** (no prazo × atrasado)
- **Distribuição de carregamentos por perfil de veículo**
- **Volume por CD de origem**
- **Tendência mensal de carregamentos**
- **Mapa interativo com os principais destinos**

---

## 🧪 Como os Dados Sintéticos Foram Gerados

Os dados foram criados utilizando Python, com:

- Distribuições proporcionais realistas (ex.: 80/20 entre transportadoras)
- Campos típicos de operação logística:
  - Transportadora
  - Tipo de veículo
  - Cidade / Estado
  - Data do carregamento
  - Quantidade de caixas
  - Valor de frete
  - Indicador de pontualidade
- Volume simulado: ~18 milhões de caixas
- Frete agregado simulado: ~63 milhões

---

## 🛠️ Tecnologias Utilizadas

- **Power BI**
- **Python (para gerar dados sintéticos)**
- **Pandas**
- **NumPy**

---

## ▶️ Como Reproduzir

1. Baixe o arquivo `.pbix` na pasta `src/`.
2. Abra no Power BI Desktop.
3. Os dados sintéticos estão na pasta `data/`.
4. Você pode editar o modelo, trocar parâmetros ou gerar novos dados.

---

## 🚀 Possíveis Extensões

- Previsão de demanda com Prophet ou ARIMA
- Dashboard de performance de transportadoras com ranking por KPI
- Criação de API fake servindo dados logísticos
- Versão web do dashboard usando Streamlit

---

## 📚 Lições Aprendidas

- Boa parte da operação logística pode ser resumida em poucos KPIs estratégicos.
- Visualizações simples (Pareto, linha, barra e gauge) contam histórias poderosas.
- A criação de dados sintéticos é essencial para portfólios profissionais na área.
- Power BI + Python formam um combo forte para projetos de supply chain.

---

## ✉️ Contato

[LinkedIn — Leonardo Souza Coelho](https://www.linkedin.com/in/leoscoelho/)

Projetos de dados, logística, automação e IA.
