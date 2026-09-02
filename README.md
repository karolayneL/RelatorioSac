# 📊 Sistema de SAC — Excel + Power BI

## 📝 Descrição
Este projeto é um Sistema de Serviço de Atendimento ao Cliente (SAC) desenvolvido com o objetivo de organizar, tratar, analisar e visualizar dados de suporte e atendimento. A partir de uma base de dados não estruturada inicial, foi criado um fluxo de análise que culmina em um dashboard interativo. O projeto visa solucionar a falta de visibilidade sobre o desempenho do atendimento, permitindo que gestores e equipes responsáveis pelo atendimento ao cliente compreendam o comportamento dos chamados, identifiquem problemas recorrentes e tomem decisões baseadas em dados.

## 🎯 Objetivos
*   **Organização dos atendimentos:** Estruturar a base histórica de chamados do SAC para viabilizar análises consistentes.
*   **Análise de indicadores:** Mapear o volume de chamados, tempos de resposta e canais mais utilizados.
*   **Identificação de problemas recorrentes:** Apontar gargalos operacionais e categorias com maior tempo de resolução.
*   **Apoio à tomada de decisão:** Fornecer uma ferramenta visual intuitiva para gestores acompanharem a operação diária.

## 🛠️ Ferramentas Utilizadas
*   **Microsoft Excel:** Utilizado para tabulação, organização inicial e consolidação do arquivo de dados.
*   **Power BI:** Utilizado para a criação do dashboard interativo e visualização de dados.
*   **Power Query (ETL):** Utilizado para extração, transformação, limpeza e padronização dos dados brutos.
*   **DAX (Data Analysis Expressions):** Utilizado para a criação de medidas e colunas calculadas.
*   **Modelagem de Dados:** Estruturação do modelo relacional para garantir a performance e precisão dos filtros no Power BI.

## 🔄 Etapas do Projeto
1.  **Coleta e estruturação dos dados:** Importação e consolidação das informações a partir do arquivo bruto `Base SAC.xlsx`.
2.  **Tratamento e limpeza dos dados:** Remoção de duplicatas, tratamento de valores nulos e padronização de formatos através do Power Query.
3.  **Organização da base:** Estruturação dos dados em um formato tabular adequado para consumo pelo software de BI.
4.  **Análise dos dados:** Exploração inicial para entender distribuições e correlações básicas no atendimento.
5.  **Criação dos indicadores:** Definição das métricas-chave (KPIs) com DAX para avaliar o desempenho do SAC.
6.  **Desenvolvimento do dashboard no Power BI:** Construção da interface no arquivo `Relatorio Sac.pbix` com gráficos interativos e filtros dinâmicos.
7.  **Geração de insights:** Interpretação visual dos resultados para responder a perguntas de negócio.

## 📊 Indicadores Analisados

**Indicadores consolidados no dashboard:**
*   **Quantidade Total de Atendimentos:** Volume bruto de chamados recebidos no período selecionado.
*   **Tempo Médio de Resolução (TMR):** Média de tempo decorrido desde a abertura até o fechamento do chamado.
*   **Volume de Atendimentos por Canal:** Distribuição de chamados divididos por E-mail, Telefone, Chat, etc.
*   **Categorias mais Frequentes:** Top motivos que levam os clientes a acionarem o suporte.

## 🖥️ Dashboard
O dashboard foi projetado para oferecer uma visão gerencial rápida e intuitiva. Através dele, é possível interagir com os dados e filtrar as informações por período, canal e status.

![Visão Geral do Dashboard](imagens/dashboard_visao_geral.png)
*Legenda: Visão consolidada dos principais KPIs e volume de chamados do SAC.*

![Análise Detalhada](imagens/dashboard_analise_detalhada.png)
*Legenda: Detalhamento do tempo médio de resolução e distribuição de chamados por categoria.*

## 💡 Principais Análises e Insights
O dashboard construído permite responder a perguntas essenciais para o negócio. Com a análise dos dados, foi possível constatar os seguintes pontos:
*   **Identificação de Gargalos:** Determinadas categorias de problemas apresentam um Tempo Médio de Resolução significativamente maior, indicando a necessidade de revisão de processos ou treinamento da equipe.
*   **Preferência de Canal:** A análise evidenciou qual canal recebe o maior volume de atendimentos, permitindo sugerir uma realocação estratégica da equipe para reduzir o tempo de espera dos clientes.
*   **Sazonalidade dos Chamados:** Foi possível mapear os períodos de maior pico de acionamentos do SAC, facilitando o planejamento de escalas da equipe de atendimento.

## 📈 Resultados Esperados
*   **Melhor visualização dos dados:** Centralização de informações dispersas em uma única tela interativa.
*   **Identificação de padrões:** Clareza sobre os picos de demanda e falhas recorrentes.
*   **Acompanhamento dos indicadores:** Facilidade para monitorar metas operacionais da equipe.
*   **Apoio à tomada de decisão:** Embasamento numérico para justificar melhorias operacionais e estruturais.
*   **Maior organização das informações do SAC:** Transição de planilhas isoladas para um modelo de dados estruturado e auditável.

## 📁 Estrutura do Repositório
```text
RelatorioSac/
├── README.md
├── dados/
│   └── Base SAC.xlsx
├── powerbi/
│   └── Relatorio Sac.pbix
└── imagens/
    ├── dashboard_visao_geral.png
    └── dashboard_analise_detalhada.png



🚀 Como Utilizar o Projeto
Faça o clone deste repositório: git clone https://github.com/karolayneL/RelatorioSac.git

Acesse a pasta do projeto em sua máquina.

Para visualizar a base de dados original, abra o arquivo Base SAC.xlsx localizado na pasta dados/.

Para visualizar e interagir com o dashboard, é necessário ter o Power BI Desktop instalado.

Abra o arquivo Relatorio Sac.pbix localizado na pasta powerbi/.

Nota: Caso ocorra erro de atualização de dados no Power BI, vá em "Transformar Dados" > "Configurações da Fonte de Dados" e altere o caminho para a pasta onde o arquivo Base SAC.xlsx está salvo no seu computador.

🧠 Aprendizados e Habilidades Desenvolvidas
Durante a execução deste projeto de portfólio, desenvolvi e apliquei as seguintes habilidades técnicas e analíticas:

Excel: Estruturação inicial e tabulação de dados.

Power Query (ETL): Limpeza, transformação e padronização da base de dados.

Modelagem de Dados: Construção de relacionamentos eficientes entre tabelas fato e dimensão.

DAX: Escrita de expressões analíticas para criação de métricas dinâmicas.

Power BI: Importação de dados, construção de relatórios e visualização de dados.

Análise de Indicadores: Tradução de necessidades da área de Customer Experience em métricas tangíveis.

Data Storytelling: Disposição lógica e visual das informações para facilitar a interpretação por parte dos gestores.

🔮 Próximos Passos
Automatização da atualização dos dados via banco de dados relacional (SQL).

Inclusão de novos indicadores de qualidade, como NPS (Net Promoter Score).

Criação de análises preditivas para estimar o volume futuro de chamados.

Classificação automática dos motivos de contato utilizando scripts em Python.

👩‍💻 Autora
Karolayne Lira da Silva

Estudante de Sistemas de Informação na UNINASSAU | Foco em Análise de Dados e Qualidade de Software

LinkedIn: https://www.linkedin.com/in/karolayne-lira-1b5501230/
