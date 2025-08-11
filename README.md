# Análise de Evasão de Clientes (Churn) - Desafio Telecom X

> Projeto de Análise de Dados desenvolvido como parte do Desafio de Data Science do Programa ONE (Oracle Next Education) em parceria com a Alura.
> **Data de Conclusão:** 11 de agosto de 2025

## 1\. Descrição do Projeto

A empresa de telecomunicações "Telecom X" enfrenta um desafio com altas taxas de evasão de clientes (churn), sem um entendimento claro das causas. Este projeto teve como objetivo realizar um processo completo de **Extração, Tratamento e Análise Exploratória de Dados (ETL & EDA)** para identificar os principais fatores e padrões de comportamento associados ao cancelamento de serviços.

A análise aqui apresentada serve como uma base investigativa inicial, fornecendo insights valiosos que podem guiar a tomada de decisões estratégicas e o desenvolvimento de modelos de machine learning preditivos para mitigar o churn.

## 2\. Estrutura do Projeto

O repositório está organizado da seguinte forma:

```
├── README.md                # Documentação do projeto (este arquivo)
├── analise_churn.ipynb      # Notebook Jupyter com todo o código da análise
├── requirements.txt         # Lista de dependências do projeto
└── graficos/                  # Pasta para armazenar os gráficos gerados
    ├── grafico_distribuicao_churn.png
    ├── grafico_churn_por_contrato.png
    └── ...
```

## 3\. Tecnologias Utilizadas

Este projeto foi desenvolvido utilizando as seguintes tecnologias e bibliotecas:

  * **Linguagem:** Python 3.10
  * **Bibliotecas Principais:**
      * **Pandas:** Para manipulação e análise de dados.
      * **Matplotlib & Seaborn:** Para visualização de dados e criação de gráficos.
      * **Requests:** Para realizar a extração dos dados da API.
  * **Ambiente:** Jupyter Notebook (executado via Google Colab ou localmente).

Excelente pergunta\! Você está absolutamente certo em questionar isso.

As instruções que eu forneci são o padrão para um **ambiente de desenvolvimento local**. Para o **Google Colab**, o processo é muito mais simples e direto, e é uma ótima ideia incluir instruções específicas para ele no seu README.

Não, as instruções de `git clone` e ambiente virtual (`venv`) **não se aplicam diretamente** da mesma forma ao Colab.

Vamos criar uma versão melhorada da seção **"Como Executar o Projeto"** do seu README, com abas ou seções separadas para cada ambiente. Isso demonstra um cuidado extra e torna seu projeto acessível a todos.

-----

## 4\. Como Executar o Projeto

Você pode replicar esta análise de duas maneiras: utilizando o Google Colab (recomendado para simplicidade) ou em um ambiente local.

### Opção 1: Google Colab (Recomendado)

O Google Colab permite executar o notebook diretamente no navegador, sem necessidade de instalação na sua máquina.

1.  **Abra o Notebook no Colab:**

      * Clique no link a seguir para abrir o arquivo `.ipynb` diretamente no ambiente do Google Colab:
      * **[https://colab.research.google.com/github/seu-usuario/nome-do-repositorio/blob/main/analise\_churn.ipynb](https://www.google.com/search?q=https://colab.research.google.com/github/seu-usuario/nome-do-repositorio/blob/main/analise_churn.ipynb)**
        *(Lembre-se de substituir `seu-usuario` e `nome-do-repositorio` pelos seus dados reais do GitHub)*

2.  **Instale as Dependências:**

      * A primeira célula do notebook já deve conter os comandos para instalar as bibliotecas necessárias. Se não, adicione uma célula no início e execute o seguinte comando:

    <!-- end list -->

    ```python
    !pip install pandas matplotlib seaborn requests
    ```

3.  **Execute a Análise:**

      * Com as dependências instaladas, basta executar as células do notebook em ordem sequencial. Você pode fazer isso clicando em "Ambiente de execução" \> "Executar tudo" no menu superior.

### Opção 2: Ambiente Local

Esta opção é para quem prefere rodar o projeto diretamente em sua máquina.

1.  **Clone o repositório:**

    ```bash
    git clone https://github.com/seu-usuario/nome-do-repositorio.git
    cd nome-do-repositorio
    ```

2.  **Crie e ative um ambiente virtual:**

    ```bash
    # Para Windows
    python -m venv venv
    .\venv\Scripts\activate

    # Para macOS/Linux
    python3 -m venv venv
    source venv/bin/activate
    ```

3.  **Instale as dependências:**

    ```bash
    pip install -r requirements.txt
    ```

4.  **Inicie e execute o Jupyter Notebook:**

    ```bash
    jupyter notebook
    ```

    Abra o arquivo `analise_churn.ipynb` e execute as células.

## 5\. Resumo da Análise e Insights

Após o processo de limpeza e tratamento dos dados, a análise exploratória revelou padrões claros sobre o perfil do cliente que tende a cancelar o serviço:

  * **Taxa de Churn Geral:** A base de dados apresenta uma taxa de evasão de aproximadamente **26.5%**.
  * **Perfil de Risco:** O cliente com maior probabilidade de churn é aquele com **pouco tempo de contrato (baixo tenure)**, um **contrato do tipo "Mês a Mês"**, serviço de **Fibra Ótica** e que realiza o pagamento via **Cheque Eletrônico**.
  * **Fatores de Retenção:** Clientes com contratos de longo prazo (1 ou 2 anos) e que utilizam métodos de pagamento automáticos (cartão de crédito, débito em conta) demonstraram uma taxa de retenção muito maior.

As visualizações detalhadas e as recomendações estratégicas baseadas nestes achados estão documentadas no relatório final dentro do notebook.

## 6\. Autor

Este projeto foi desenvolvido por:

**Paulo Junior Walbueno Dos Santos**

  * **LinkedIn:** [(https://www.linkedin.com/in/paulo-junior-ws)](https://www.linkedin.com/in/paulo-junior-ws)
  * **GitHub:** [(https://github.com/paulojunior6886)](https://github.com/paulojunior6886)]
