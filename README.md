# Projeto-ETL-com-IA---Gerador-de-mensagens-IA-para-vagas.
O Projeto consiste na pratica aplicada de conceitos ETL amplamente usado na área de dados como metodologia de passos essenciais no tratamento de dados e seus respectivos destinos, este projeto incorpora APIs de IA que geram a mensagem com uma simples engenharia de prompt e bibliotecas essenciais do Python para analise de dados, referencias DIO .

# 👩‍💻 Mentor de IA - Pipeline de ETL e Recomendação de Vagas

Este projeto recria originalmente um projeto de um bootcamp da DIO que utiliza swagger de uma API do SantanderDevWeek2023 e API do ChaatGPT.
O Projeto é um pipeline completo de **ETL (Extract, Transform, Load)** que utiliza a Inteligência Artificial (Google Gemini foi escolhido por mim como alternativa ao ChatGPT) para analisar perfis de candidatos e recomendar as vagas de dados mais compatíveis, gerando mensagens de mentoria personalizadas.

## 🛠️ Tecnologias Utilizadas

*   **Python**: Linguagem principal.
*   **Pandas**: Manipulação e transformação de dados (ETL).
*   **Google Gemini API**: Geração de conteúdo inteligente e análise de perfil.

## 🔄 O Processo de ETL

1.  **Extract (Extração)**: Leitura de bases de dados em CSV (`jobs.csv` e `users.csv`).
OBS: Como a API da SantanderDevWeek2023 foi descontinuada, optei por armazenar os dados em um arquivo simples em CSV para que fosse a referencia de dados so projeto.   
3.  **Transform (Transformação)**:
    *   Filtragem de vagas específicas para a área de dados.
    *   Cálculo de score de compatibilidade baseado em competências (Skills).
    *   Processamento de linguagem natural via IA para criar conselhos de carreira.
4.  **Load (Carregamento)**: Exportação dos resultados em arquivos de texto individuais.

## 🚩 Como Executar o Projeto

1.  Clone o repositório:
    ```bash
    git clone https://github.com/seu-usuario/seu-repositorio.git
    ```
2.  Instale as dependências:
    ```bash
    pip install -r requirements.txt
    ```
3.  Configure sua `API_KEY` do Google Gemini no código.
4.  Execute o notebook ou script principal para gerar as mensagens na pasta `output/`.

## 📂 Estrutura de Arquivos

*   `data/`: Contém os arquivos CSV de entrada.
*   `output/messages/`: Local onde as mentorias personalizadas são salvas.
*   `main.ipynb`: Código principal do pipeline.

---
Desenvolvido por Yago Alves Toledo (https://github.com/yagoalt54)
