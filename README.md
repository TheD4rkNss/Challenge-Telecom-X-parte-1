# 📈 TelecomX - Análise de Evasão de Clientes

![Python](https://img.shields.io/badge/python-v3.8+-blue.svg)
![Pandas](https://img.shields.io/badge/pandas-v1.5+-green.svg)
![Plotly](https://img.shields.io/badge/plotly-v5.0+-orange.svg)
![Status](https://img.shields.io/badge/status-active-success.svg)

## 📋 Sobre o Projeto

Este projeto realiza uma análise completa de evasão de clientes (churn) da empresa TelecomX, utilizando técnicas de análise exploratória de dados para identificar padrões e fatores que influenciam a decisão dos clientes de cancelar seus serviços.

## 🎯 Objetivos

- Analisar o comportamento de churn dos clientes da TelecomX
- Identificar fatores que influenciam na evasão de clientes
- Fornecer insights para estratégias de retenção
- Desenvolver recomendações baseadas em dados para reduzir a taxa de churn

## 🛠️ Tecnologias Utilizadas

- **Python 3.8+**
- **Pandas** - Manipulação e análise de dados
- **NumPy** - Computação numérica
- **Matplotlib** - Visualização de dados
- **Seaborn** - Visualização estatística
- **Plotly Express** - Gráficos interativos
- **Jupyter Notebook** - Ambiente de desenvolvimento

## 📊 Estrutura dos Dados

O dataset contém informações sobre clientes da TelecomX com as seguintes características:

### Dados Demográficos
- **customerID**: Identificador único do cliente
- **gender**: Gênero do cliente
- **SeniorCitizen**: Indicador se é cidadão idoso
- **Partner**: Possui parceiro
- **Dependents**: Possui dependentes
- **tenure**: Tempo de permanência (meses)

### Serviços Contratados
- **PhoneService**: Serviço telefônico
- **MultipleLines**: Múltiplas linhas
- **InternetService**: Tipo de internet (DSL, Fiber optic, No)
- **OnlineSecurity**: Segurança online
- **OnlineBackup**: Backup online
- **DeviceProtection**: Proteção de dispositivos
- **TechSupport**: Suporte técnico
- **StreamingTV**: Streaming de TV
- **StreamingMovies**: Streaming de filmes

### Informações de Conta
- **Contract**: Tipo de contrato (Month-to-month, One year, Two year)
- **PaperlessBilling**: Faturamento sem papel
- **PaymentMethod**: Método de pagamento
- **Charges.Monthly**: Cobrança mensal
- **Charges.Total**: Cobrança total
- **Total.Day**: Gasto diário calculado

### Variável Alvo
- **Churn**: Cliente cancelou o serviço (Yes/No)

## 🔄 Metodologia

### 1. 📌 Extração
- Carregamento dos dados do dataset JSON
- Importação das bibliotecas necessárias
- Verificação inicial da estrutura dos dados

### 2. 🔧 Transformação
- **Normalização**: Conversão de colunas aninhadas (JSON) para formato tabular
- **Limpeza**: Remoção de duplicatas e tratamento de valores ausentes
- **Padronização**: Conversão de valores binários (0/1) para formato categórico (No/Yes)
- **Tratamento de Tipos**: Conversão de tipos de dados apropriados
- **Feature Engineering**: Criação da coluna `Total.Day` (gasto diário)

### 3. 📊 Análise Exploratória
- Análise da distribuição de churn
- Correlações entre variáveis
- Análise por segmentos de clientes
- Visualizações interativas com Plotly

## 🔍 Principais Insights

### Fatores de Risco para Churn
- **Tipo de Contrato**: Contratos mensais apresentam maior taxa de churn
- **Método de Pagamento**: Pagamentos eletrônicos automáticos têm menor churn
- **Tempo de Permanência**: Clientes novos (primeiros 6 meses) são mais propensos ao churn
- **Tipo de Internet**: Clientes com fibra óptica apresentam comportamento diferente

### Características dos Clientes que Cancelam
- Maior concentração em contratos month-to-month
- Menor tempo de permanência
- Padrões específicos de uso de serviços adicionais

## 🚀 Recomendações

### Estratégias de Retenção
1. **Programa de Onboarding**: Implementar programa especial para novos clientes nos primeiros 6 meses
2. **Monitoramento Proativo**: Criar alertas para clientes com perfil de alto risco de churn
3. **Personalização de Ofertas**: Desenvolver ofertas específicas baseadas no perfil de gastos do cliente
4. **Melhoria na Experiência**: Focar na experiência do cliente, especialmente para contratos mensais

### Ações Específicas
- Incentivar migração para contratos anuais ou bianuais
- Promover métodos de pagamento automáticos
- Criar campanhas de retenção para clientes com baixo tenure
- Melhorar a experiência com serviços de fibra óptica

## 🚀 Como Executar

1. **Clone o repositório**
```bash
git clone https://github.com/seu-usuario/Challenge-Telecom-X-parte-1.git
cd Challenge-Telecom-X-parte-1
```

2. **Instale as dependências**
```bash
pip install pandas numpy matplotlib seaborn plotly jupyter
```

3. **Execute o notebook**
```bash
jupyter notebook TelecomX_BR.ipynb
```

## 📋 Pré-requisitos

- Python 3.8 ou superior
- Jupyter Notebook
- Bibliotecas Python listadas em `requirements.txt`

## 🔗 Fonte dos Dados

Os dados são carregados diretamente da URL:
`https://raw.githubusercontent.com/alura-cursos/challenge2-data-science/refs/heads/main/TelecomX_Data.json`

## 📈 Métricas de Avaliação

- **Taxa de Churn**: Percentual de clientes que cancelaram
- **Distribuição por Segmentos**: Análise por diferentes características
- **Correlações**: Identificação de fatores mais relevantes
- **Padrões Temporais**: Análise baseada no tempo de permanência

## 🤝 Contribuições

Contribuições são bem-vindas! Para contribuir:

1. Faça um fork do projeto
2. Crie uma branch para sua feature (`git checkout -b feature/AmazingFeature`)
3. Commit suas mudanças (`git commit -m 'Add some AmazingFeature'`)
4. Push para a branch (`git push origin feature/AmazingFeature`)
5. Abra um Pull Request

## 📄 Licença

Este projeto está licenciado sob a licença MIT. Veja o arquivo `LICENSE` para mais detalhes.

## 📧 Contato

Para dúvidas ou sugestões, entre em contato através do email: [seu-email@exemplo.com]

---

*Este projeto foi desenvolvido como parte do Challenge de Data Science da Alura, focando na análise de evasão de clientes para fornecer insights acionáveis para a empresa TelecomX.*
