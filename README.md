# TP01 – Integração de Sistemas de Informação  
**Aluno:** Renato Barbosa 
**Número:** 22570
**Professor:** Óscar Ribeiro  
**Ano Letivo:** 2025/26  

---

##  Descrição do Projeto
Este projeto teve como objetivo desenvolver um processo **ETL (Extract, Transform, Load)** utilizando a plataforma **KNIME**, aplicado a um cenário fictício de vendas de uma loja online.  
O processo integra três fontes de dados distintas:  
- **Clientes**: ficheiro CSV (`clientes.csv`)  
- **Vendas**: ficheiro XML (`vendas.xml`)  
- **Produtos**: dados obtidos de uma API pública [https://fakestoreapi.com/products](https://fakestoreapi.com/products)  

Os dados foram limpos, normalizados e integrados num único fluxo. Foram realizadas validações de emails e telefones, correções textuais e cálculos do total gasto por cliente, categoria e produto.  
O resultado final foi exportado em vários formatos (CSV, Excel e JSON) e gravado numa base de dados **PostgreSQL**, permitindo análise e visualização através de gráficos no KNIME.

---

##  Como Executar o Projeto
1. Instalar o **KNIME Analytics Platform** (versão 5.x ou superior).  
2. Importar o workflow contido na pasta `dataint/`.  
3. Garantir que os ficheiros de entrada estão em `data/input/`.  
4. Executar o workflow completo, iniciando no componente **Extract**.  
5. Os ficheiros de saída serão gerados automaticamente em `data/output/`.  
6. (Opcional) Verificar os dados gravados na base de dados **PostgreSQL** através do Beekeeper Studio.  

---

##  Estrutura do Repositório
tp01-25431/
│
├── README.md
│
├── doc/
│ └── 25431_doc.pdf # Relatório final em PDF
│
├── dataint/
│ └── workflow_knime.knwf # Workflow exportado do KNIME
│
├── data/
│ ├── input/ # Ficheiros de entrada
│ │ ├── clientes.csv
│ │ └── vendas.xml
│ │
│ └── output/ # Ficheiros de saída e exemplos
│ ├── resultado_clientes.csv
│ ├── resultado_categorias.xlsx
│ └── resultado_produtos.json
│
└── src/ # Código adicional (se aplicável)

##  Vídeo de Demonstração
O vídeo de demonstração do projeto pode ser consultado através do seguinte link:  
👉 [**Ver demonstração no YouTube**](https://youtu.be/TSlvSnjiV5E)

*(O mesmo link encontra-se também disponível no relatório em formato QR Code.)*

---

##  Ferramentas e Tecnologias
- **KNIME Analytics Platform 5.x**  
- **PostgreSQL** + **Beekeeper Studio**  
- **FakestoreAPI** (dados JSON de produtos)  
- **Microsoft Excel** / **CSV** / **JSON** para exportações  

---

## Entrega
Data limite: **19 de outubro de 2025 – 23h59**  

---