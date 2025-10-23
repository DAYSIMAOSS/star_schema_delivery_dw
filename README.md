#  Star Schema DW – Avaliação de Entregas  

Este projeto apresenta a **modelagem e implementação de um Data Warehouse** baseado no modelo **Star Schema (Esquema Estrela)**, com o objetivo de analisar **avaliações de entregas** realizadas por clientes.  

---

##  Visão Geral  

O projeto implementa uma arquitetura dimensional que facilita a análise de desempenho logístico e de satisfação de clientes.  
A modelagem foi realizada com base em princípios de **Business Intelligence (BI)** e **OLAP (Online Analytical Processing)**, permitindo explorar dados históricos de forma analítica.  

---

##  Estrutura do Projeto  

| Arquivo | Descrição |
|----------|------------|
| `PBL_e_os_guris_e_as_gurias_2TSCO_Fase2_item_1_4.docx` | Documento descritivo da modelagem conceitual e evidências de execução no Oracle. |
| `cria.sql` | Script de **criação das tabelas** fato e dimensão (DDL). |
| `apaga.sql` | Script de **remoção das tabelas** e limpeza do ambiente. |
| `Relational_1.pdf` | Modelo relacional com atributos, chaves e relacionamentos. |

---

##  Estrutura do Modelo Star Schema  

###  Tabela Fato  
**FATO_AVALIACAO_ENTREGA**  
Contém as métricas e indicadores analisados, como:  
- Nota de Embalagem  
- Nota de Pontualidade  
- Nota de Cortesia  
- Tempo de Entrega  
- Quantidade de Entregas Realizadas e Planejadas  
- Valor Total do Item  

###  Tabelas Dimensão  
- **DIM_CLIENTE** → informações dos clientes  
- **DIM_CENTRO_DISTRIBUICAO** → centros logísticos e CDs  
- **DIM_PRODUTO** → produtos avaliados  
- **DIM_TEMPO** → tempo e granularidade de análise (dia, mês, ano, trimestre)  
- **DIM_LOCAL**, **DIM_ESTADO**, **DIM_REGIAO** → estrutura geográfica  
- **DIM_CATEGORIA**, **DIM_SUBCATEGORIA** → hierarquia de produtos  

---

##  Tecnologias Utilizadas  
- **Oracle SQL Developer / Oracle Database**  
- **Modelagem Dimensional (Star Schema)**  
- **Linguagem SQL (DDL e DML)**  
- **Documentação técnica (Word e PDF)**  

---

##  Objetivo do Projeto  
Implementar um **Data Warehouse de avaliação de entregas**, promovendo:  
- Consolidação de dados logísticos e de satisfação.  
- Consultas analíticas com integridade referencial garantida.  
- Base sólida para dashboards e relatórios de performance.  

---

##  Execução  

1. Execute o script `apaga.sql` para limpar o ambiente (se necessário).  
2. Execute `cria.sql` para criar todas as tabelas fato e dimensão.  
3. Insira os dados de teste conforme definido no documento `.docx`.  
4. Valide as relações e integridade das chaves estrangeiras.  

---

##  Conceito de Star Schema  

O **Star Schema (Esquema Estrela)** é uma modelagem dimensional que organiza os dados em:  
- **Tabelas Fato**, que armazenam medidas quantitativas;  
- **Tabelas Dimensão**, que contêm os contextos descritivos dessas medidas.  

Essa estrutura facilita análises rápidas e intuitivas em ambientes de **Data Warehouse**, otimizando consultas para **BI e relatórios gerenciais**.  

---

##  Autoria  
Projeto desenvolvido por **Dayanne Simão**,  
como parte das atividades práticas da disciplina de Banco de Dados – FIAP.  

---

##  Licença  
Uso acadêmico e educacional. Créditos obrigatórios ao autor em caso de reprodução.  
