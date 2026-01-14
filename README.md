<b>:: Monitoramento de Criptomoedas em Tempo Real ::</b>

Este projeto, desenvolvido na Data Science Academy, tem como objetivo construir um sistema integrado de monitoramento do mercado de criptomoedas em tempo real, unindo práticas modernas de engenharia de dados e desenvolvimento web interativo.

<br />

<b>:: Tecnologias utilizadas ::</b>

Apache Kafka → para ingestão assíncrona de dados de cotações via API

MongoDB → para armazenamento flexível e ágil dos dados filtrados

Streamlit → para visualização em tempo real em formato de dashboard interativo

CoinCap API → fonte gratuita de dados de mercado de criptomoedas

<br />
<b>:: Como funciona o fluxo de dados ::</br>
<br />
Coleta de dados → Usamos a API do CoinCap.io para extrair informações de cotações de criptomoedas em tempo real.<br /><br />

Ingestão com Kafka → Os dados brutos são enviados para o Apache Kafka, garantindo processamento assíncrono e sem perda de mensagens.

Processamento e filtragem → Em Python, consumimos os dados do tópico Kafka, aplicamos filtros simples e enviamos os resultados para o MongoDB.

Armazenamento → O MongoDB foi escolhido por sua flexibilidade e porque o projeto demanda apenas filtragem leve antes da persistência.

Visualização → Criamos uma aplicação web interativa em Streamlit, que consulta o MongoDB e apresenta os dados em tabelas e gráficos em tempo real.

<br />
<b>:: Por que não usei PySpark? ::</b>
<br /><br />
Embora o PySpark seja uma ferramenta poderosa para processamento em larga escala, neste projeto ele seria um canhão para matar um mosquito.
O volume de dados é moderado e não há necessidade de processamento distribuído. Kafka + MongoDB já atendem perfeitamente ao objetivo.
<br />
<br />
<b>Benefícios desse projeto</b>
<br /><br />
✅ Praticar o uso do Apache Kafka em cenários reais<br />
✅ Construir um pipeline de dados de ponta a ponta<br />
✅ Criar um dashboard em tempo real para análise de mercado<br />
✅ Útil para estudantes de engenharia de dados e também para investidores de criptomoedas<br />
