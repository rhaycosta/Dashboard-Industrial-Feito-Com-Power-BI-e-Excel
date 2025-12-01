# Painel de Análise de Produção 🏭

Este projeto consiste em um dashboard analítico desenvolvido no **Power BI** para monitoramento de KPIs industriais.

## 📷 Visualização do Projeto
![preview](https://github.com/user-attachments/assets/8621a0e4-3404-4376-8af8-b13798e78eb7)

## 🛠 Tecnologias Utilizadas
* **Power BI** (ETL, Modelagem, DAX, Visualização)
* **Excel / SAP** (Fonte de dados)

## 📋 Funcionalidades
* **Monitoramento de KPIs:** Acompanhamento visual de Qtd de Ordens, Tempo Médio e Total Produzido.
* **Análise de Eficiência:** Indicadores de taxa de conclusão vs. erros e paradas.
* **Segmentação:** Detalhamento por tipo de material (ex: Mola, Parafuso) e tendências mensais.

---

## 🏗️ Como foi construído (Passo a Passo)

O desenvolvimento do painel seguiu as melhores práticas de Business Intelligence:

### 1. Coleta e Tratamento (ETL)
* Conexão com planilhas de exportação do sistema (Excel/SAP).
* Tratamento de dados no **Power Query**: Promoção de cabeçalhos, alteração de tipos de dados (Data, Número, Texto) e limpeza de linhas vazias para garantir a integridade da análise.

### 2. Modelagem e Cálculos (DAX)
* Criação de medidas explícitas para os principais indicadores:
    * `Total Ordens` (Contagem distinta).
    * `Total Produzido` (Soma agregada).
    * `Taxa de Conclusão` (Cálculo percentual para análise de eficiência).
* Organização de colunas para permitir a segmentação correta por Data e Categoria.

### 3. Visualização de Dados (UI/UX)
* **Cartões (KPIs):** Posicionados no topo para leitura imediata dos números macro.
* **Gráfico de Rosca:** Utilizado para visualizar a composição do status (Concluído vs Erro vs Parado).
* **Gráfico de Linhas:** Implementado para analisar a tendência de produção ao longo dos meses (Sazonalidade).
* **Gráfico de Barras:** Para ranking de volume de produção por tipo de material.

---

## 🚀 Como visualizar
Como o GitHub não renderiza arquivos `.pbix` nativamente:
1. Faça o download do arquivo `Análise de Produção.pbix` deste repositório.
2. Abra-o utilizando o Power BI Desktop.
