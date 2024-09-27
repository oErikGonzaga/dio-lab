# Tipos de Serviço de Nuvem

> *“Com grandes poderes vêm grandes responsabilidades” Tio Ben. 
Explicando um pouco sobre o Modelo de Responsabilidade Compartilhada.*
> 

Existe um conceito generico que se aplica a todos os providers que mais conhecemos, o **IaaS -** Infraestrutura como Serviço, **PaaS** - Plataforma como Serviço e **SaaS** - Software como Serviço.

![iaas_paas_saas.png](https://github.com/oErikGonzaga/dio-lab/blob/main/images/iaas_paas_saas.png?raw=true)

**IaaS - Infraestrutura como Serviço**

---

Na **IaaS**, trata-se de um serviço em que o cliente tem mais acesso ao recurso final, assumindo responsabilidades como monitoramento, configuração e backups, o que permite maior controle sobre esses recursos. No caso da criação de uma máquina virtual, as configurações de assinatura, nome, backup, grupo de recursos, modelo de acesso e redes são etapas que devem ser realizadas pelo cliente. Mesmo após essas configurações, atualizações e monitoramento precisam ser acompanhados de perto. Esse modelo oferece "liberdade", porém a responsabilidade é inteiramente do cliente.

**PaaS**

---

Já neste modelo, algumas configurações não são mais necessárias, e o cliente não precisa lidar com os elementos complexos de configuração da máquina. O envolvimento ocorre sobre o que será utilizado, como bancos de dados, armazenamento ou serviços. O foco não está no gerenciamento da infraestrutura, mas sim em criar, testar e implantar aplicativos.

**SaaS**

---

Neste último modelo, um bom exemplo é o Microsoft 365. O acesso aos produtos é definido por licenças. Com uma licença básica, os recursos disponíveis são limitados; com uma licença intermediária, há acesso a mais funcionalidades; e com uma licença premium, todos os recursos da plataforma estão disponíveis. A licença determina o que cada usuário pode acessar, permitindo personalizar as funcionalidades conforme as necessidades da organização. Aqui, a aplicação já está pronta, e o que define a experiência do usuário é a licença adquirida. A responsabilidade do cliente se limita às configurações dos grupos de usuários.

**Modelo de responsabilidade Compartilhada**

---

![modelo_responsabilidade_compartilhada.png](https://github.com/oErikGonzaga/dio-lab/blob/main/images/modelo_responsabilidade_compartilhada.png?raw=true)

Acompanhando o gráfico acima, no modelo **No Local** (**On Premise**), é possível ver que toda a responsabilidade é dada ao cliente, desde um cabo de rede danificado até a criação de um usuário, tudo fica por conta do cliente. Lembrando que, neste caso, trata-se de uma nuvem privada.

Já no caso da nuvem, observa-se que, em IaaS, PaaS ou SaaS, a responsabilidade sobre o datacenter físico, a rede física e os hosts físicos recai sobre o provedor. No modelo **IaaS**, apenas esses três aspectos são de responsabilidade do provedor, enquanto os demais ficam a cargo do cliente. No modelo **PaaS**, isso muda: o sistema operacional passa a ser responsabilidade do provedor, e as outras três áreas se tornam responsabilidades compartilhadas, onde o provedor gerencia uma parte, e o cliente preenche as lacunas. Por último, no modelo **SaaS**, todos os dados e informações, dispositivos, contas e identidades são de responsabilidade do cliente, enquanto a infraestrutura de identidade e diretório é compartilhada; o restante é gerido pelo provedor.

Olhando para esse cenário, fica claro que, conforme o nível de gestão aumenta, mais tempo e esforço dos colaboradores são demandados. Imagine a necessidade de se preocupar com atualizações, patches, backups e possíveis problemas em 100, 500 ou até 1000 máquinas. Esse tipo de responsabilidade é significativamente maior em ambientes **On Premise**. Nos modelos de nuvem, como IaaS, PaaS e SaaS, essa carga de trabalho diminui gradativamente à medida que mais responsabilidades são transferidas para o provedor, o que reflete em um custo maior pelos serviços, mas também em uma redução da complexidade de gestão para o cliente.

Dessa forma, podemos dizer que o modelo **IaaS** é um serviço de nuvem mais flexível, pois o cliente gerencia o hardware para o aplicativo; o **PaaS** é mais focado no desenvolvimento de aplicativos, já que a plataforma é gerenciada pelo provedor; e o **SaaS** é um modelo de pagamento conforme o uso, no qual os usuários pagam pelo software por meio de um modelo de assinatura.
