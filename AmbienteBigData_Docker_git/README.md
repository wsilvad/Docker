Este proejto visa utilizar a API do Yahoo Finanças para extrair os dados da bolsa de valores de algumas ações, utilizar o Nifi para criar o fluxo de coleto, salvar estes dados no Elasticsearch e exibir gráficamente utilizando o Kibana. Os dados não foram tratados após coleta, mas podem ser manipulados com a aplicação do Anaconda que foi instalado na mesma imagem.

Ferramentas utilizadas
    - WEB Flask
    - Zookeeper (hadoop)
    - Nifi 
    - Elasticsearch
    - Kibana
    - Anaconda

Para utilização do Correta do Projeto devem se seguir os seguintes passos:
    1. Instalação do Docker
    2. Instalação do GitHub
    3. Clonar este projeto pela sua máquina
    4. Abrir pasta com o terminal ou VS Code
    5. Executar o comando docker-compose -f docker-compose.yml up -d para iniciar a instalação das imagens e iniciar os serviços
    6. Após a instalação acessar o Nifi > clicar com o botão direito > upload template > utilizar o template disponibilizado na basta doc_auxiliares > inserir o modo de template e utilizar o template carregado

Portas para acesso aos APPs
- 5001: Yahoo Finanças API
- 8080: Nifi
- 9200: Elasticsearch
- 9300: Elasticsearch transmission port
- 5601: Kibana
- 8888: Anaconda/Jupyter

