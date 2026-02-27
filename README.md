# Taming Big Data with Apache Spark 4 and Python – Hands On!

Este repositório contém notebooks e arquivos de dados utilizados durante o curso **"Taming Big Data with Apache Spark 4 and Python – Hands On!"**, oferecido pela **Sundog Education**.  
O conteúdo foi desenvolvido como parte do aprendizado prático de **Big Data Analysis** com **PySpark**, explorando desde conceitos básicos de RDDs até módulos avançados como **Spark SQL**, **Spark Streaming** e **GraphX**.

---

## 🛠️ Tecnologias e Ferramentas

![Python](https://img.shields.io/badge/Python-3.8+-3776AB?style=for-the-badge&logo=python&logoColor=white)
![Apache Spark](https://img.shields.io/badge/Apache_Spark-4.x-E25A1C?style=for-the-badge&logo=apachespark&logoColor=white)
![PySpark](https://img.shields.io/badge/PySpark-Latest-E25A1C?style=for-the-badge&logo=apachespark&logoColor=white)
![Pandas](https://img.shields.io/badge/Pandas-150458?style=for-the-badge&logo=pandas&logoColor=white)
![Jupyter](https://img.shields.io/badge/Jupyter-F37626?style=for-the-badge&logo=jupyter&logoColor=white)
![Docker](https://img.shields.io/badge/Docker-2496ED?style=for-the-badge&logo=docker&logoColor=white)
![AWS](https://img.shields.io/badge/AWS_EMR-232F3E?style=for-the-badge&logo=amazonaws&logoColor=white)

**Principais tecnologias utilizadas:**
- **Apache Spark 4.x** - Framework de processamento distribuído
- **PySpark** - API Python para Spark
- **Pandas & Pandas-on-Spark** - Análise de dados e integração híbrida
- **Jupyter Notebook** - Ambiente interativo de desenvolvimento
- **Docker** - Containerização do ambiente Spark
- **AWS EMR** - Execução em cluster na nuvem

---

## Sobre o Projeto

Durante o curso, foram estudadas técnicas modernas para análise de grandes volumes de dados utilizando o **Apache Spark 4**, com ênfase no uso de **PySpark** e **Pandas-on-Spark**.  

Os notebooks neste repositório reproduzem os exercícios e exemplos práticos aprendidos, sendo material ideal para consulta, revisão e experimentação.

**Principais objetivos de aprendizado:**

- Processar e transformar grandes conjuntos de dados com Spark
- Utilizar **DataFrames**, **Datasets** e **Spark SQL** para análise distribuída
- Implementar transformações eficientes com **RDDs** (Resilient Distributed Datasets)
- Integrar Spark com **Pandas** para análise híbrida de dados
- Executar jobs em clusters locais e na nuvem (AWS EMR)
- Explorar módulos avançados: **Spark ML**, **Streaming** e **GraphX**
- Aplicar boas práticas de otimização e paralelização de tarefas

---

## Estrutura do Repositório

```
Spark_Notebooks/
│
├── Dados/                           # Arquivos de dados usados nos exercícios
│   ├── ml-100k/                     # MovieLens Dataset (recomendações de filmes)
│   ├── 1800.csv
│   ├── book.txt
│   ├── customer-orders.csv
│   ├── fakefriends.csv
│   └── fakefriends-header.csv
│
├── Spark_Basics/                    # Exercícios introdutórios sobre RDDs
│   ├── 12.data100.ipynb
│   ├── 14.friends.ipynb
│   ├── 16.minTemperatures.ipynb
│   ├── 17.maxTemperatures.ipynb
│   ├── 18.bookTxt.ipynb
│   ├── 20.bookSorted.ipynb
│   └── 22.byTotal.ipynb
│
├── Spark_DataFrame_DataSet/         # Exemplos com DataFrames e SQL
│   ├── 25.sqlFunctions.ipynb
│   ├── 26.dataFrames.ipynb
│   ├── 28.friendsByAgeDataframe.ipynb
│   ├── 29.wordCount.ipynb
│   ├── 31.totalSpent.ipynb
│   ├── 34.pandas.ipynb
│   ├── 34.pandasConversion.ipynb
│   └── 34.pandas-transform-apply.ipynb
│
├── docker-compose.yaml              # Configuração do ambiente Docker
├── .gitignore
└── README.md
```

---

## Requisitos e Instalação

### Pré-requisitos

- **Python 3.8+**
- **Apache Spark 4.x**
- **Jupyter Notebook**
- **Docker** (opcional, para ambiente containerizado)

### Instalação de Dependências

```bash
# Criar ambiente virtual (recomendado)
python -m venv .venv
source .venv/bin/activate  # Linux/Mac
# ou
.venv\Scripts\activate     # Windows

# Instalar pacotes necessários
pip install findspark pyspark pandas jupyter matplotlib
```

### Iniciando o Ambiente

```bash
# Iniciar Jupyter Notebook
jupyter notebook

# Ou via Docker
docker-compose up
```

Acesse o Jupyter Notebook via navegador em `http://localhost:8888`

---

## Tópicos Cobertos

O projeto reflete os principais módulos estudados no curso:

### 1. Getting Started with Spark
Instalação, configuração e primeiros exemplos com PySpark. Criação de sessões Spark, carregamento de dados e operações básicas.

### 2. Spark Basics and the Legacy RDD Interface
Manipulação direta de RDDs (Resilient Distributed Datasets) — filtragem, mapeamento, agregações e ordenação distribuída.

### 3. SparkSQL, DataFrames, and DataSets
Uso de DataFrames, consultas SQL distribuídas e criação de Datasets tipados para análise estruturada de dados.

### 4. Advanced Examples of Spark Programs
Casos complexos de análise, incluindo sistemas de recomendação (MovieLens) e análise de grafos sociais.

### 5. Running Spark on a Cluster
Execução de jobs em ambiente distribuído, incluindo configuração e deploy em AWS EMR.

### 6. Machine Learning with Spark ML
Introdução ao Spark MLlib para algoritmos de clustering, regressão e classificação em escala.

### 7. Spark Streaming, Structured Streaming, and GraphX
Processamento de dados em tempo real e exploração de relacionamentos complexos com GraphX.

### 8. Next Steps
Conclusão do curso e direcionamentos para aplicação profissional do conhecimento adquirido.

---

## Conjuntos de Dados

Principais datasets utilizados nos notebooks:

| Dataset | Descrição |
|---------|-----------|
| **MovieLens 100k** | Análise de avaliações e sistemas de recomendação de filmes |
| **FakeFriends.csv** | Estudo de correlação entre idade e número de amigos |
| **Customer-Orders.csv** | Cálculo de valores totais gastos por cliente |
| **Book.txt** | Processamento de texto, word count e análise de frequência |
| **Temperature Data (1800.csv)** | Identificação de temperaturas mínimas e máximas por estação |

---

## Execução via Docker

O arquivo `docker-compose.yaml` permite iniciar um ambiente Spark completo e containerizado:

```bash
docker-compose up -d
```

Após a inicialização, acesse:
- **Jupyter Notebook:** `http://localhost:8888`
- **Spark UI:** `http://localhost:4040` (quando um job estiver rodando)

---

## Objetivo do Repositório

Este repositório serve como:

- **Material de referência** para conceitos fundamentais e avançados de Big Data com Spark
- **Código prático** para experimentação e aprendizado hands-on
- **Base de consulta** para revisão de técnicas, padrões e boas práticas
- **Ponto de partida** para desenvolvimento de projetos próprios com PySpark

---

## Próximos Passos e Melhorias Futuras

Possíveis expansões planejadas para o projeto:

- [ ] Adicionar notebooks com exemplos práticos de **Spark Streaming** em tempo real
- [ ] Implementar pipelines completos de **Machine Learning** com Spark MLlib
- [ ] Criar casos de uso com dados reais obtidos de APIs públicas
- [ ] Adicionar exemplos de otimização de performance (particionamento, cache, broadcast variables)
- [ ] Integração com ferramentas de visualização (Plotly, Matplotlib, Seaborn)
- [ ] Exemplos de deploy e execução em diferentes clouds (AWS EMR, Azure HDInsight, GCP Dataproc)
- [ ] Documentação de troubleshooting e resolução de problemas comuns

---

## Como Contribuir

Contribuições são bem-vindas! Se você deseja adicionar exemplos, corrigir bugs ou melhorar a documentação:

1. Faça um **fork** do projeto
2. Crie uma **branch** para sua feature (`git checkout -b feature/NovoExemplo`)
3. **Commit** suas mudanças (`git commit -m 'Adiciona novo exemplo de Streaming'`)
4. Faça o **push** para a branch (`git push origin feature/NovoExemplo`)
5. Abra um **Pull Request**

---

## Licença e Observações

- Este projeto foi desenvolvido **para fins educacionais**, baseado nos exemplos práticos do curso **"Taming Big Data with Apache Spark 4 and Python – Hands On!"**
- Os notebooks podem ser adaptados e utilizados em diferentes ambientes Spark (local, cluster ou cloud)
- Todo o código é livre para estudo, experimentação e adaptação pessoal

---

## Créditos

**Curso:** Taming Big Data with Apache Spark 4 and Python – Hands On!  
**Oferecido por:** Sundog Education Team  
**Desenvolvido por:** Henrique Mourão

---

## 📫 Contato

- **GitHub:** [Henrique-Mourao](https://github.com/Henrique-Mourao)
- **LinkedIn:** [Henrique Mourão](https://www.linkedin.com/in/henrique-mour%C3%A3o/)
- **Email:** henriquegmour4@gmail.com

---
