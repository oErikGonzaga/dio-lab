# Construindo Arquiteturas Azure

### Passo a passo para criação de um Grupo de Recursos e um Banco de Dados SQL

---

**Criando um Grupo de Recursos**

1. Entre no **Portal Azure** com sua conta.
2. No painel de menu à esquerda (ou pesquise na barra de pesquisa localizada na parte superior), selecione a opção **Grupo de Recursos**.
3. Clique em **Criar**.
4. Na aba **Básico**, você verá as seções **Detalhes do Projeto** e **Detalhes do Recurso**.
5. Em **Detalhes do Projeto**, preencha o campo **Grupo de Recursos** com um nome para o grupo.
6. Em **Detalhes do Recurso**, selecione a **Região** onde deseja criar seus recursos.
7. Prossiga para a aba **Marcações** ou clique em **Avançar** no rodapé da página.
   - *Na aba **Marcações**, você verá os campos **Chave** e **Valor**. É possível usá-los para organizar logicamente o grupo de recursos ou ignorá-los.*
8. Clique na aba **Revisar + Criar** ou em **Avançar** no rodapé da página.
9. Na aba **Revisar + Criar**, revise os dados e clique em **Criar**.

---

**Criando um Servidor e um Banco de Dados SQL**

1. Retorne à página inicial.
2. Na barra de pesquisa, busque por **SQL Database** (Banco de Dados SQL) e clique.
3. Clique em **Criar**.
4. Na aba **Básico**, você verá as seções **Detalhes do Projeto** e **Detalhes do Banco de Dados**.
5. Em **Detalhes do Projeto**, selecione o **Grupo de Recursos** que você acabou de criar.
6. Em **Detalhes do Banco de Dados**, dê um nome para o seu **Banco de Dados** e clique em **Criar novo** para o **Servidor**.
7. Em **Nome do Servidor**, insira um nome e selecione a **Localização**.
8. Em **Método de Autenticação**, selecione *Usar autenticação SQL*, crie um nome para o **Logon de Administrador**, insira uma senha e clique em OK.
9. De volta à tela de criação do banco de dados, com o **Servidor** selecionado, marque *Não* em **Deseja usar o pool elástico SQL**, selecione *Desenvolvimento* em **Ambiente de Carga de Trabalho** e escolha *Armazenamento de backup com redundância local* em **Redundância**. Em seguida, clique em **Avançar: Rede**.
10. Na aba **Rede**, selecione **Ponto de Extremidade Público** em **Método de Conectividade** e clique em **Revisar + Criar**.
11. Na aba **Revisar + Criar**, revise os dados e clique em **Criar**.
* ***Obs.:** Na aba **Básico**, para evitar custos desnecessarios na opção **Computação + Armazenamento** escolha o de menor custo.*

---

**Criando uma Conexão com o Servidor e Banco de Dados**

1. Com o Servidor e o Banco de Dados criados, para estabelecer uma conexão com o banco de dados SQL no Azure, baixe e instale o **Azure Data Studio**.
   - Link: [Azure Data Studio](https://azure.microsoft.com/pt-br/products/data-studio)
2. Após a instalação, abra o **Azure Data Studio** e clique em **Create a Connection**.
3. Preencha o campo **Server** com o endereço do servidor que você criou anteriormente, selecione *SQL Login* em **Authentication Type**, insira o nome de usuário e a senha criados e clique em OK.

---

* **Obs.:** Imagens do passo a passo no Link: [Imagens do passo a passo](https://github.com/oErikGonzaga/dio-lab/blob/main/Resumos/passo_a_passo_arquitetura_azure.md)
