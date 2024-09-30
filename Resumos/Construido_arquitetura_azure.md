# Construindo Arquiteturas Azure

### Passo a passo para criação de um Grupo de Recursos e um Banco de Dados SQL


Criano um Grupo de Recursos

- Entre no **Portal Azure** com sua conta
- No painel de menu à esquerda (ou pesquise na barra de pesquisa localizada na barra superior), selecione a opção **Grupo de Recursos**
- Clique em **Criar**
- Na aba **Básico**, você verá **Detalhes do Projeto** e **Detalhes do Recurso**
- Em **Detalhes** **do** **Projeto**, preencha o campo **Grupo de Recursos** com um nome para o Grupo
- Em **Detalhes do Recurso**, preencha o campo com a **Região** em que deseja criar seus recursos
- Prossiga para a aba **Marcações** ou clique em **Avançar** no rodapé da página
    - *Na aba **Marcações**, nos deparamos com um campo chave e valor. É possível nomeá-los para uma organização lógica do grupo de recursos, ou pode ignorar*
- Clique na aba **Revisar + Criar** ou em **Avançar** no rodapé da página
- Na aba **Criar**, revise os dados e clique em **Criar**

&nbsp;

Criano um Servidor e um Banco de Dados SQL

- Retorne à página inicial
- Na barra de pesquise busque por SQL Database (Banco de Dados SQL) e clique
- Clique em **Criar**
- Na aba **Básico**, você verá **Detalhes do Projeto** e **Detalhes de Banco de Dados**
- Em **Detalhes do Projeto**, selecione o **Grupo de Recursos** que acabou de criar
- Em **Detalhes do Banco de Dados**, dê um nome para sua **Banco de Dados** e **Servidor** clique em criar um novo;
- Em **Nome do Servidor** dê um nome para o servidor e selecione a **Localização**
- Mais abaixo em **Método de Autenticação** marque *Usar autenticação SQL,* dê um nome para o **Logon de Administrador da Empresa**, crie uma senha e dê OK
- De volta a tela de criar banco de dados, com o S**ervidor** selecionado, marque *Não* em **Deseja usar o pool elástico SQL,** marque *****Desenvolvimento* em **Ambiente de Carga de trabalho,** marque *****Armazenamento de backup com redundância local*  ****em **Redundância e clique em Avançar: Rede** ou na aba **Rede**
- Na aba **Rede**, marque Ponto de extremidade público e clique em **Método de conectividade** e depois em **Revisar e criar**
- Na aba **Revisar e Criar,** revise os dados e clique em **Criar**

  &nbsp;

  Criano uma Conexão com o Servidor e com Banco de Dados

- Com o Servidor e o Banco de Dados criado, para criarmos uma conexão com o banco de dados SQL na Azure, baixe o **Azure Data Studio** e instale em seu Sistema.
- link Azure Data Studio: https://azure.microsoft.com/pt-br/products/data-studio
- Após a instalação do Azure Data Studio com o programa aberto clique em **Create a Connection**
- preencha os campos **Server** com o endereço criado anteriormente, selecione *SQL Login* em **Authentication Type,** insira o username e senha criados anteriormente e clique em OK
- Na aba **Básico**, você verá **Detalhes do Projeto** e **Detalhes da Instância**
- Em **Detalhes do Projeto**, selecione o **Grupo de Recursos** que acabou de criar
- Em **Detalhes da Instância**, dê um nome para sua **Rede Virtual**, selecione a **Região** em que deseja criar o Recurso e clique na Aba **Revisar + Criar**
    - *No momento, não preencha os dados das abas: **Segurança**, **Endereços de IP** e **Marcas**. Deixe para que o sistema preencha automaticamente*
- Na aba **Revisar + Criar**, confira os dados que inseriu e em seguida clique em **Criar**
