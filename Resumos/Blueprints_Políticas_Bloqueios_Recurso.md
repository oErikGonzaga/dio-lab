### Blueprints, Políticas e Bloqueios de Recurso: A Arte da Governança na Nuvem

> *“"A verdade é a única arma que você tem." — Superman.*
> Políticas transparentes e bem definidas são essenciais para a segurança na nuvem..*

No universo da computação em nuvem, a governança e a conformidade são essenciais para garantir que os recursos sejam utilizados de maneira eficaz e segura. Neste contexto, **Blueprints**, **Políticas** e **Bloqueios de Recurso** desempenham papéis cruciais na organização e proteção dos ativos digitais. Vamos explorar como essas ferramentas funcionam e como podem ser aplicadas no Azure.

**O que são Blueprints, Políticas e Bloqueios de Recursos?**

Esses três elementos são fundamentais para a gestão e proteção de recursos no Azure. Enquanto os **Blueprints** permitem a criação de padrões para a implementação de recursos, as **Políticas** ajudam a impor conformidade e segurança em escala. Os **Bloqueios de Recurso** protegem os ativos contra exclusões ou modificações acidentais, garantindo que tudo funcione conforme o esperado.

**Azure Policy: Aguardando a Conformidade**

A **Azure Policy** atua como um guardião que impõe padrões organizacionais em toda a infraestrutura. Se uma regra é estabelecida, ela deve ser aplicada independentemente de quem esteja executando uma ação. Essa governança assegura a consistência dos recursos, promovendo conformidade regulatória, segurança e gerenciamento de custos. Além disso, a Azure Policy avalia e identifica recursos que não atendem aos padrões estabelecidos.

- **Modify Effect**: Os recursos existentes que não estão em conformidade não são afetados pelas novas regras, mas novos recursos devem se alinhar às diretrizes.
- **Non-Compliant**: Recursos antigos não afetados pelas regras.
- **Remediation**: Requer que os recursos em não conformidade sejam ajustados, como a inserção obrigatória de tags em novos recursos.
- **Compliant**: Todos os recursos estão de acordo com as políticas estabelecidas.

**Bloqueios de Recursos: Proteção em Camadas**

Os **Bloqueios de Recursos** fornecem uma camada extra de proteção contra exclusão ou modificação acidental. No portal do Azure, é possível gerenciar bloqueios em níveis de assinatura, grupo de recursos ou em recursos individuais. Essa proteção garante que recursos críticos não sejam deletados ou alterados sem a devida análise.

Existem dois tipos de bloqueio:

- **Excluir**: Permite a leitura e atualização, mas impede a exclusão.
- **ReadOnly**: Permite apenas a leitura, bloqueando atualizações e exclusões.

Antes de aplicar um bloqueio, é fundamental avaliar as necessidades do recurso, pois um bloqueio indevido pode resultar em custos adicionais desnecessários.

**Portal de Confiança do Serviço**

O **Portal de Confiança do Serviço** oferece uma visão clara das normas e regulamentos que a Microsoft segue para garantir que os serviços atendam a expectativas específicas de diferentes segmentos, incluindo o setor público. Essa transparência é fundamental para estabelecer confiança nas operações de nuvem.

**Microsoft Purview: A Governança de Dados em Foco**

O **Microsoft Purview** é uma família de soluções dedicadas à governança, risco e conformidade de dados. Ele proporciona uma visão unificada dos dados, permitindo que as empresas mensurem riscos, realizem auditorias sobre o acesso aos dados e automatizem a descoberta e classificação de informações confidenciais. A linhagem de dados de ponta a ponta também é monitorada, garantindo que cada informação seja rastreável.
