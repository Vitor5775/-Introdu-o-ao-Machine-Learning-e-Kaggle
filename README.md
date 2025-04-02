# Introdução ao Machine Learning e Kaggle


  Comparação de Desempenho entre DeepSeek e ChatGPT usando Machine Learning

  1. Base de Dados Escolhida:
     
    Nome: DeepSeek vs ChatGPT: Comparação de plataformas de IA
    Link no Kaggle: DeepSeek vs ChatGPT Dataset
  
  Descrição:
  O conjunto de dados contém interações sintéticas de usuários com duas plataformas de IA (ChatGPT - GPT-4-turbo e DeepSeek - DeepSeek-Chat 1.5) ao longo de 18 meses (julho/2023 a fevereiro/2025).
  
  Principais características
  
    Métricas de Desempenho:
  
    Response_Accuracy (Precisão da resposta, escala 0-1)
  
    Response_Speed_sec (Tempo de resposta em segundos)
  
    Dados de Usuários:
  
    Active_Users, New_Users, Churned_Users, Retention_Rate
  
    Contexto da Interação:
  
    Query_Type (Técnica, Geral, Criativa, etc.)
  
    Device_Type (Mobile, Desktop, Tablet)
  
    Region (País/Região do usuário)
  
  Tamanho:
  
  Mais de 10.000 linhas e 27 colunas.
  
  2. Técnica de Machine Learning Escolhida:
     
         Classificação Binária (Logistic Regression ou Random Forest)
          Justificativa:
          O objetivo é prever qual plataforma (DeepSeek ou ChatGPT) terá melhor desempenho em uma determinada interação, com base em:
  
    Tipo de consulta (Query_Type)
  
    Dispositivo (Device_Type)
  
    Região (Region)
  
    Velocidade (Response_Speed_sec)
    
    Precisão (Response_Accuracy)
  
  A classificação é adequada porque:
  
    Temos um rótulo categórico (AI_Platform: DeepSeek ou ChatGPT).
  
    Queremos identificar padrões que indiquem qual modelo de IA performa melhor em diferentes cenários.
  
  3. Objetivos da Análise
  Comparar o desempenho entre DeepSeek e ChatGPT em termos de:
  
    Precisão (Response_Accuracy)
  
    Velocidade (Response_Speed_sec)
  
    Identificar fatores que influenciam a preferência do usuário (ex.: tipo de pergunta, região, dispositivo).
  
    Construir um modelo preditivo que determine qual IA tem maior probabilidade de ser mais eficaz em uma dada situação.
  
  4. Método Proposto
  Pré-processamento:
  
    Tratar valores nulos (se houver).
  
    Codificar variáveis categóricas (Query_Type, Device_Type, Region).
  
    Normalizar variáveis numéricas (Response_Speed_sec, Response_Accuracy).
  
    Análise Exploratória (EDA):
  
    Comparar médias de Response_Accuracy e Response_Speed_sec por plataforma.
  
    Verificar distribuição de consultas por tipo e região.
  
  Modelagem:
  
    Dividir os dados em treino e teste.
    
    Treinar modelos de Regressão Logística e Random Forest.
    
    Avaliar usando Acurácia, Precisão, Recall e AUC-ROC.
    
    Resultados Esperados:
    
    Identificar em quais cenários cada IA se sai melhor.
    
    Gerar insights para otimização de plataformas de IA.
  
  5. Conclusão:
     
    Comparação objetiva entre DeepSeek e ChatGPT.
    Identificação de pontos fortes e fracos de cada modelo.
    Aplicação em recomendações para usuários (ex.: qual IA usar para perguntas técnicas vs. criativas).
