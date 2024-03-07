# treinamento_azure_ml
Criação do modelo e configuração:

# Passo 01:
- Criar uma conta no azure e cadastrar um cartão de crédito
- Ir no endereço: ml.azure.com
- Realizar a consulta no Market Place informando Azure Machine Learning
- Subscrição:
    - Resource Group (Grupo de Trabalho)
- Workspace Details:
    - Inserir informações: Nome (Preencher), Região (Preencer), Storage Account, Key Vault, Application Insights, Container Registry (Manter padrão)
-  Rede: Manter public (para estudo)
-  Encriptação: Manter padrão (para estudo)
- Identidade:
- Tags: Manter padrão, mas serve para rastreabilidade
- Review + create: Clicar em create para criar o ambiente
- Acompanhar sempre o status do Deploy
# Passo 02:
- Ir em lauch studio (depois de feito o passo 01)
- Ir em ML Automatizado e criar um novo trabalho de ML automatizado
- Inserir os dados de acordo com a documentação (mslearn-bike-automl)
    - Configuração básica:
          - Nome do trabalho, Novo nome do experimento, descrição e marca
    - Tipo de tarefa e dados:
          - Regressão, nome, descrição e tipo (tabular), url, configurações (formato arquivo, delimitador, codificação, cabeçalhos de coluna e ignorar linhas), esquema (manter padrão), examinar - criar
    - Configuração de tarefas:
          - Tipo Tarefa (preenchimento automático), dados (preenchimento automático), coluna de destino (rental's), limites, validar (desmarcar as opções) e testar
    - Computação (Padrão):
    - Examinar: Enviar trabalho de treinamento
  # Passo 03:
  - Escolher o melhor modelo e selecionar implantar
  - Inserir as informações sugeridas pela documentação
  - No término da execução ir em "Pontos de Extremidade"
  - Clicar no nome do modelo
  - Na aba testar o endpoint, pode-se inserir os valores que estão na documentação e ver o resultado em JSON
