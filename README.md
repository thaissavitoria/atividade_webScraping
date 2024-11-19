# Mini Atividade 1

Este projeto consiste em resolver três questões que envolvem extração de dados e manipulação automatizada de informações utilizando Python.

---

## **Questão 1**
**Tarefa**:  
Efetuar a extração de 500 cursos de pós-graduação do link [Sucupira Capes](https://sucupira.capes.gov.br/programas/detalhamento/2099).  
### **Informações a serem extraídas**:
- Código
- Área Básica
- Área de Avaliação
- Situação
- Cidade
- CEP
- Data de Início
- Universidade
- Mestrado 
  - Nota
  - Situação
  - Código
- Doutorado 
  - Nota
  - Situação
  - Código
---
Os dados foram exportados em um arquivo csv.

## **Questão 2**
**Tarefa**:  
Efetuar a extração de dados de duas URLs diferentes utilizando Python.  
A saída deve ser dois arquivos CSV contendo todos os dados coletados.

### **Escolha dos sites**:
1. **[IMDb](https://www.imdb.com/chart/top/)**:
   - **Objetivo**: Extrair informações dos melhores filmes mais bem avaliados de todos os tempos.
   - **Dados extraídos**:
     - Título
     - Nota
     - Duração
     - Classificação indicativa
   - O código foi estruturado para tratar exceções como falta de informações em algumas colunas e garantir a criação do CSV.

2. **[Wikipedia - 2024 no Cinema](https://pt.wikipedia.org/wiki/2024_no_cinema)**:
   - **Objetivo**: Extrair a tabela de filmes com maior bilheteria do ano de 2024.
   - **Dados extraídos**:
     - Ranque
     - Título
     - Produtor
     - Bilheteria Global
   - Foi necessário tratar casos em que o HTML da tabela apresentava linhas sem todos os dados, garantindo consistência no CSV final.

### **Saída**:
- Arquivo `imdb_top_movies.csv` com os melhores filmes.
- Arquivo `bilheteria_2024.csv` com a bilheteria global dos filmes de 2024.

---

## **Questão 3**
**Tarefa**:  
Criar um programa para fazer o download das tirinhas do site [XKCD](http://xkcd.com/) seguindo o botão "Previous Comic" até alcançar a primeira tirinha.

### **Funcionamento**:
- O programa navega pela página inicial do XKCD, salva a imagem da tirinha exibida, segue o link "Previous Comic" e repete até a primeira tirinha.
- Para salvar as tirinhas, foi usada a função `iter_content()` do módulo `requests`.

### **Observação**:
- Durante a execução, foi identificado que a tirinha 2198 não é uma imagem, mas um HTML com elementos visuais. Como o objetivo era baixar apenas imagens, o programa foi ajustado para pular esses casos e continuar o download normalmente.

---

## **Execução**
Todas as atividades foram desenvolvidas e testadas no **Jupyter Notebook**.
Os arquivos CSV e as imagens foram gerados corretamente no diretório de trabalho.

---
