# Projeto Machine Learning no Azure ML - DIO

Segue o passo a passo do Trabalhando com Machine Learning na Prática no Azure ML da DIO, com o objetivo de criar um modelo de previsão com seus devidos pontos de extremidades configurados.

Passo 1:
1. Criar um Workspace no Azure Machine Learning:
- Acessei o portal do Azure e na página princial busquei por criar recurso, pesquisando sobre Azure Machine Learning no Marketplace. Em seguida, acessar o recurso para criar um workspace do Machine Learning. Os passo seguintes utilizei o documento da Microsoft para auxiliar (Fonte: https://microsoftlearning.github.io/mslearn-ai-fundamentals/Instructions/Labs/01-machine-learning.html)
![image](https://github.com/Andrelpavan/ProjetoAzureML/assets/69944259/9d233139-34be-433b-8a4b-267ec069d3e8)

2. O segundo passo é configurar o Workspace:
- Escolhi uma assinatura do Azure onde deseja criar o Workspace.
- Criei um novo grupo de recursos ou use um existente.
- Insiri um nome para o Workspace.
- Selecionei a região onde deseja hospedar o Workspace.
- Estando tudo certo cliquei em "Revisar + criar".

3. Revisar e Criar o Workspace:
- Revisei as configurações do Workspace para garantir que estejam corretas.
- Cliquei em "Criar" para iniciar o processo de criação do Workspace.

4. Aguardar a conclusão da criação:
- O Azure levará alguns minutos para criar o Workspace.
- Você receberá uma notificação quando o processo estiver concluído.
![image](https://github.com/Andrelpavan/ProjetoAzureML/assets/69944259/47fc2d15-8908-43b2-80c5-443afc359f89)

Este é o processo é para criar um Workspace no Azure Machine Learning. Uma vez que o Workspace tenha sido criado, começei a utilizar as suas capacidades para desenvolver e implantar um modelo de Machine Learning.

5. Acessar o Workspace:
- No local de Trabalhar com seus modelos no Estúdio do Azure Machine Learning clicar no inica o Studio para acessar a página inicial do estúdio de aprendizagem da máquina.
![image](https://github.com/Andrelpavan/ProjetoAzureML/assets/69944259/ee080de2-6077-408b-8624-668cd99a0622)

Passo 2: 

1.Criando o modelo:
- No portal do Azure Machine Learning Studio, cliquei em "ML automatizado" no menu lateral.
- Na página que abriu selecionei em o item da aba "Novo trabalho de ML automatizado".
![image](https://github.com/Andrelpavan/ProjetoAzureML/assets/69944259/b9114914-3104-4869-976e-f366b9ca7eca)

2.Definindo as Configurações de Automação:
- Nas "Configurações básicas" preenchi os campos "Novo nome do experimento" e "Descrição". Após cliquei em "Avançar".
- No item "Tipo de tarefa e dados" foi selecionado o tipo de tarefa como Regressão, em seguida em "Selecionar dados", cliquei em "Criar".
  ![image](https://github.com/Andrelpavan/ProjetoAzureML/assets/69944259/707e42a5-12c5-49f4-a35e-417dc5915ba8)

3. Definir o nome e o tipo do ativo de dados:
- Na próxima janela aberta em "Tipos de dados", preenchi os campos "Nome", "Descrição" e "Tipo" foi escolhido como Tabular.
  Avançando para a próxima etapa "Fonte de dados", foi escolhido "De arquivos da Web", cliquei em avançar novamente.
  ![image](https://github.com/Andrelpavan/ProjetoAzureML/assets/69944259/9f133e36-d104-409c-ab8e-d3545a4db480)

- Na "URL da Web" informei a URL https://aka.ms/bike-rentals onde o conjunto de dados a ser trabalhado se encontra. Aguardar a validação.
- No passo "Configurações", onde determinam como os dados são analisados. Após avançar para "Esquema", verifiquei os tipos de dados conforme documentação. E para terminas avançar para "Examinar", verifiquei as configurações de dados e em seguida cliquei em criar para avança para o "Tipo de tarefa e dados".
![image](https://github.com/Andrelpavan/ProjetoAzureML/assets/69944259/3dcbf04b-714f-48ed-94ce-051353d8362e)

4. Configuração de tarefa:
- Nestas configurações de tarefa utilizei os dados do documento (Fonte:https://microsoftlearning.github.io/mslearn-ai-fundamentals/Instructions/Labs/01-machine-learning.html)
- Após preenchimento dos campos, clicar em "Enviar trabalho de treinamento" para ser examinado e terminar o processo (demora alguns minutos).
![image](https://github.com/Andrelpavan/ProjetoAzureML/assets/69944259/99d69ffa-5b5f-485f-a9ad-49d21addba32)

5. Validar as métricas:
- Após concluir o trabalho de treinamento, analisei as métricas e em seguida precisei criar o modelo para ficar acessivel na aba "Modelo".
![image](https://github.com/Andrelpavan/ProjetoAzureML/assets/69944259/7f927e39-b153-4c7d-b8fd-8def2688fc24)

6. Registrar e Implentar o Modelo:
- Uma vez que tenha identificado o melhor modelo, registrei no Workspace.
- Após o registro do modelo, acessar o "Ponto de extremidade" na aba lateral para poder  implantar como um serviço web.
  ![image](https://github.com/Andrelpavan/ProjetoAzureML/assets/69944259/c28b6ad8-e144-49eb-89f7-4a0d1d23705e)

7.Teste da implementação:
- Nesta etapa acessei a aba "Testar" do ponto de extremidade criado para o meu modelo. Busquei os codigos junto a documentação para realizar os testes.
- Em seguida acessei a aba "Testar" do ponto de extremidade para realizar o teste abaixo.
![image](https://github.com/Andrelpavan/ProjetoAzureML/assets/69944259/578706f8-ea4a-4bb2-aece-a528b4dab260)

8.Conclusão:
- O resultado final do teste, que incluem um número previsto de aluguéis com base nos recursos de entrada, resultou em: 368.12.


