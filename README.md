# 📘 Criação e Configuração de Bancos de Dados SQL no Azure

## 🛠️ 1. Criando um Banco de Dados SQL no Portal do Azure

### Etapas Básicas:
1. Acesse o [Portal do Azure](https://portal.azure.com).
2. Navegue até **Bancos de Dados SQL** e clique em **Criar**.
3. Preencha as informações necessárias:
   - **Assinatura** e **Grupo de Recursos**.
   - **Nome do Banco de Dados** e **Servidor** (crie um novo ou selecione um existente).
   - **Camada de Preço** conforme a carga de trabalho esperada.
4. Configure as opções de **Redundância de Backup** e **Configurações de Segurança**.
5. Revise as configurações e clique em **Criar** para implantar o banco de dados.

> ℹ️ Para mais detalhes, consulte o [Guia de Criação de Banco de Dados SQL no Azure](https://learn.microsoft.com/pt-br/azure/azure-sql/database/single-database-create-quickstart?view=azuresql).

---

## 🧩 2. Conectando-se ao Banco de Dados

### Usando o Azure Data Studio:
1. Abra o Azure Data Studio.
2. Clique em **Nova Conexão** e insira as informações:
   - **Tipo de Conexão**: Microsoft SQL Server.
   - **Nome do Servidor**: nome_do_servidor.database.windows.net.
   - **Tipo de Autenticação**: Autenticação do SQL Server ou Microsoft Entra ID.
   - **Nome de Usuário** e **Senha**.
3. Clique em **Conectar**.

> 🔗 Saiba mais: [Conectar-se ao Banco de Dados SQL do Azure com Azure Data Studio](https://learn.microsoft.com/pt-br/azure-data-studio/quickstart-sql-database).

---

## 🔒 3. Práticas Recomendadas de Segurança

- **Atualizações Regulares**: Mantenha o sistema operacional e aplicativos atualizados.
- **Controle de Acesso**: Utilize o Azure Active Directory e atribua permissões mínimas necessárias.
- **Criptografia**:
  - Ative a criptografia de dados em repouso com Transparent Data Encryption (TDE).
  - Utilize o Azure Key Vault para gerenciamento de chaves.
- **Monitoramento**:
  - Habilite a Auditoria para rastrear eventos de banco de dados.
  - Configure alertas para atividades suspeitas.

> 🔗 Consulte: [Melhores Práticas de Segurança para o Banco de Dados SQL do Azure](https://learn.microsoft.com/pt-br/azure/azure-sql/database/security-overview?view=azuresql).

---

## 📈 4. Monitoramento e Otimização

- **Azure Monitor**: Coleta métricas e logs para análise de desempenho.
- **Query Store**: Armazena informações sobre execução de consultas para ajudar na otimização.
- **Azure Advisor**: Fornece recomendações para otimizar custos, desempenho e segurança.

> 🔗 Mais informações: [Ajustar Aplicativos e Bancos de Dados para Desempenho no Banco de Dados SQL do Azure](https://learn.microsoft.com/pt-br/azure/azure-sql/database/performance-guidance?view=azuresql).

---

## 💡 Dicas Finais

- **Automatização**: Utilize scripts ARM, Azure CLI ou PowerShell para automatizar a criação e configuração de bancos de dados.
- **Backups**: Configure backups automáticos e retenção de dados conforme necessário.
- **Redundância**: Considere a replicação geográfica para alta disponibilidade.
- **Custos**: Monitore o uso de recursos e ajuste as camadas de preço conforme necessário para otimizar custos.

