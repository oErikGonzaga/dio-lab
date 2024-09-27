# Benefícios da Computação na Nuvem

> *“A nuvem é uma ambiente virtualizado, que eu pago conforme o uso e se eu não quiser mais eu paro de pagar e pronto".*
> 

Seria bom se fosse fácil assim. Mas existem bem mais detalhes no processo e isso precisa ser explicado.

É bom saber quais os benefícios, quais são e como são aplicados no dia a dia.

Entre eles: Alta disponibilidade, escalabilidade, confiabilidade, previsibilidade, segurança, governança e gerenciamento na nuvem.

**Alta disponibilidade**

---

Aqui se trata de um sistema que esta altamente disponível sempre que necessário, mas este beneficio esta principalmente relacionado ao **SLA** (*Service Level Agreement (Acordo de Nível de Serviço)*). 

Neste caso a Microsoft fornece um contrato que garante o funcionamento de seus produtos e serviços dentro de uma *porcentagem de tempo contratada*, o que significa que caso o exista uma quebra desse garantia, ou seja se um serviço exceda o tempo de inatividade ela gerará um voucher como ressarcimento baseado no tempo de serviço que ficou inativo. 

| SLA | Tempo de inatividade por semana | Tempo de inatividade por mês | Tempo de inatividade por ano |
| --- | --- | --- | --- |
| 99% | 1,68 hora | 7,2 horas | 3,65 dias |
| 99,9% | 10,1 minutos | 43,2 minutos | 8,76 horas |
| 99,95% | 5 minutos | 21,6 minutos | 4,38 horas |
| 99,99% | 1,01 minuto | 4,32 minutos | 52,56 minutos |
| 99,999% | 6 segundos | 25,9 segundos | 5,26 minutos |

Quando uma falha acontece o suporte é constantemente atualizado em relação a falha e até mesmo ao tipo de falha, que podem ser : falhas transitórias ou falhas duradouras. Assim também como falhas de escopo que podem atingir (do menor para o maior) : Maquinas, Serviço e de Região.

![image.png](https://github.com/oErikGonzaga/dio-lab/blob/main/images/region_services_machines.png?raw=true)

A alta disponibilidade foca em garantir a disponibilidade maxima, independente dos eventos que ocorram. Mas para isso existem serviços que garantem esse alta disponibilidade, como alguns serviços de redundância ou região.

**Escalabilidade**

---

É a capacidade de ajustar recursos para atender uma demanda, o que significa que no aumento de demanda haverá como adicionar ou remover recursos conforme a necessidade, fazendo assim com que só haja cobrança pelo que uso (Pay as you go).

Um exemplo é a escala vertical que, supondo que o desenvolvimento de um app precise de mais capacidade de processamento, a escala vertical adicionará mais CPUs ou RAM à Maquina Virtual.

**Elasticidade**

---

Um dos melhores exemplos para elasticidade é o Evento de Black Friday, aonde acontece um aumento repentino na demanda de requisições de uma loja virtual, fazendo com que a aplicação saísse fora do ar. Já que era esperado uma quantidade de acesso X no dia do evento e a contratação do serviço era uma quantidade Y fazendo que ou no excesso de acesso a aplicação caísse, ou na expectativa de alta demanda não fosse atingida. 

Na elasticidade há um adição de maquinas virtuais ou containers por meio de Expansão e havendo o contrario os recursos são reduzidos Horizontalmente de forma automática ou manual.

**Confiabilidade**

---

Através do design descentralizado (regiões em países que o provider tem acesso) o que gera um suporte de infraestrutura resiliente e confiável (associada a resiliência de um sistema que se recupera de falhas e continua funcionando), permitindo o acesso a recursos implantados em diversas regiões do mundo, atrelado a recursos *Altamente Disponíveis,* como o Disaster Recovery e ou Replicações, isso obviamente atrelado as regras do SLA.

**Previsibilidade**

---

Se diz a respeita da permissão de que um cliente que precisa de um avanço tecnológico no qual a nuvem entregará esse suporte para que ele  chegue aonde almeja. 

**Exemplo**: uma empresa cujo a infra é pequena e privada mas a demanda desta necessita de mais recursos e a nuvem consegue dar esse suporte de transição fazendo com que a empresa alcance o sucesso.

**Segurança**

---

Na nuvem as responsabilidades são compartilhadas, o provider oferece ferramentas de segurança, mas a implementação de muitas delas é por parte do cliente e não responsabilidade do provider. Isso dependendo da implantação escolhida: IaaS, PaaS ou SaaS. 

**Governança**

---

Trata de cumprimentos de regras estabelecidas de acordo com o seguimento da empresa para que sejam cumpridas devidamente, com transparência, responsabilidade, equidade para uma melhor proteção, atualização e gerenciamento da nuvem. Isso através de uma auditoria que auxilia na sinalização de recursos fora dos padrões corporativos.

**Gerenciabilidade**

---

Forma ao qual criamos nossas implantações através dos painéis da **Portal Web** do provider ou através de L**inhas de Comando** de código e ou scripts, **APIs** ou **PowerShell**.
