## Links úteis

- [Nuvem híbrida aberta](https://www.redhat.com/pt-br/products/open-hybrid-cloud)
- [Suporte](https://access.redhat.com/)
- [Desenvolvedores](https://developers.redhat.com/)
- [Parceiros](https://www.redhat.com/pt-br/partners)
- [Comece já a avaliação](https://www.redhat.com/pt-br/products/trials)



- [Skip to content](https://www.redhat.com/pt-br/topics/security/what-is-cve#rh-main-content)



- [Produtos](https://www.redhat.com/pt-br/technologies)
- [Soluções](https://www.redhat.com/pt-br/solutions)
- [Serviços e suporte](https://www.redhat.com/pt-br/services)
- [Recursos](https://www.redhat.com/pt-br/resources)
- [Red Hat e o open source](https://www.redhat.com/pt-br/about)



[Português](https://www.redhat.com/pt-br/selecione-um-idioma)



[Pesquisar](https://www.redhat.com/pt-br/search)



[Login](https://sso.redhat.com/auth/realms/redhat-external/protocol/saml/clients/legacy-idp-servlets)



[Contato](https://www.redhat.com/pt-br/contact)



- [Tópicos ](https://www.redhat.com/pt-br/topics)
- [ Introdução à segurança da TI ](https://www.redhat.com/pt-br/topics/security)
-  O que é CVE?

# O que é CVE?

Atualizado 25 de novembro de 2020•6 minutos (tempo de leitura)



Copiar URL

IR PARA SEÇÃO

- [Visão geral](https://www.redhat.com/pt-br/topics/security/what-is-cve#visão-geral)
- [Como isso funciona?](https://www.redhat.com/pt-br/topics/security/what-is-cve#como-isso-funciona)
- [O que qualifica um CVE?](https://www.redhat.com/pt-br/topics/security/what-is-cve#o-que-qualifica-um-cve)
- [O que é o CVSS?](https://www.redhat.com/pt-br/topics/security/what-is-cve#o-que-é-o-cvss)
- [O que é a API de dados de segurança?](https://www.redhat.com/pt-br/topics/security/what-is-cve#o-que-é-a-api-de-dados-de-segurança)

## Visão geral

O CVE, sigla inglesa para vulnerabilidades e exposições comuns, é uma lista pública de falhas de segurança. Quando alguém se refere a um CVE, isso significa uma falha de segurança atribuída a um número de ID correspondente.

Os fornecedores e pesquisadores quase sempre mencionam pelo menos um ID CVE nos relatórios de segurança. Os CVEs ajudam os profissionais de TI a trabalharem em conjunto para priorizar e solucionar essas vulnerabilidades, a fim de tornar os sistemas de computadores mais seguros.

[Ebook: leia sobre a segurança da nuvem híbrida](https://www.redhat.com/pt-br/engage/boost-hybrid-cloud-security)

## Como funciona o sistema CVE?

O CVE é administrado pela [MITRE Corporation](https://cve.mitre.org/) e financiado pela Agência de Segurança Cibernética e de Infraestrutura, que integra o Departamento de Segurança Interna dos EUA.

As entradas do CVE são curtas. Não incluem dados técnicos, nem informações sobre riscos, impactos ou correções. Essas informações aparecem em outros bancos de dados, como o [National Vulnerability Database (NVD) dos Estados Unidos](https://nvd.nist.gov/), o [Vulnerability Notes Database do CERT/CC](https://www.kb.cert.org/vuls/) e várias listas criadas por fornecedores e outras organizações. Nesses vários sistemas, os IDs CVE oferecem aos usuários uma forma confiável de diferenciar as falhas de segurança.

### Sobre os identificadores CVE

Os identificadores CVE são atribuídos por uma Autoridade de numeração CVE (CNA). Há [aproximadamente 100 CNAs](https://cve.mitre.org/cve/request_id.html) que representam os principais fornecedores de TI, empresas de segurança e organizações de pesquisa. A MITRE também emite CVEs diretamente.

As CNAs recebem blocos de CVEs, que são reservados para atribuição aos novos problemas que forem descobertos. Milhares de [IDs CVE](https://www.cvedetails.com/browse-by-date.php) são emitidos todos os anos. Uma única solução complexa, como sistemas operacionais, por exemplo, pode acumular centenas de CVEs.

Relatórios de CVEs podem surgir de várias fontes. Um fornecedor, um pesquisador ou um usuário astuto podem descobrir uma falha e informar alguém a respeito. Muitos fornecedores oferecem [recompensas por bugs](https://en.wikipedia.org/wiki/Bug_bounty_program) para encorajar a divulgação responsável de falhas de segurança. Se você encontrar alguma vulnerabilidade em um [software open source](https://www.redhat.com/pt-br/topics/open-source/what-is-open-source-software), [informe à comunidade](https://opensource.com/article/19/3/bug-reporting).

De uma forma ou de outra, informações sobre a falha acabam chegando às CNAs. A CNA atribui um ID CVE à informação e cria uma breve descrição com referências. Depois, essa entrada é publicada no site do CVE.

Muitas vezes, o ID CVE é atribuído antes da disponibilização pública do relatório de segurança. É comum fornecedores manterem falhas de segurança em segredo até desenvolverem e testarem uma correção. Isso reduz as chances de invasores explorarem as falhas não corrigidas.

Depois de publicada, a entrada inclui o ID CVE (no formato "CVE-2019-1234567"), uma descrição breve da exposição ou vulnerabilidade de segurança e referências, que podem trazer links para relatórios de vulnerabilidades e avisos.

## O que qualifica um CVE?

Os IDs CVE são atribuídos a falhas que atendem a certos critérios. Elas devem ser:

##### **1. Corrigíveis de forma independente.**

A falha pode ser corrigida independentemente de outros bugs.

##### 2. **Reconhecidas pelo fornecedor afetado OU documentadas.**

O fornecedor do software ou hardware reconheceu o bug e admitiu o impacto negativo à segurança. Ou ele compartilhou um relatório de vulnerabilidade que demonstra o impacto negativo do bug e a violação da política de segurança do sistema afetado.

##### 3. **Afetam apenas uma base de código.**

Falhas que impactam mais de uma solução recebem CVEs separados. No caso de bibliotecas, protocolos ou padrões compartilhados, a falha recebe um único CVE apenas se não for possível usar o código compartilhado sem se tornar vulnerável. Caso contrário, cada base de código ou solução afetada recebe um CVE único.

Adaptado de https://cve.mitre.org/cve/cna/rules.html#Section_4_1_qualifications

Fique por dentro de tudo sobre a segurança da Red Hat.

[Leia o nosso guia](https://www.redhat.com/pt-br/technologies/guide/it-security)

## O que é o Sistema de Pontuação de Vulnerabilidade Comum?

Existem várias formas de avaliar a gravidade de uma vulnerabilidade. Uma delas é o [Sistema de pontuação de vulnerabilidades comuns (CVSS)](https://www.first.org/cvss/), um conjunto de padrões abertos usado para atribuir um número a uma vulnerabilidade de acordo com sua gravidade. O NVD, CERT e outros bancos de dados usam essas pontuações para avaliar o impacto das vulnerabilidades. A pontuação vai de 0 a 10; quanto maior o número, mais grave. Muitos fornecedores de segurança criaram seus próprios sistemas de pontuação.

##### **Três principais conclusões** 

**Conheça as suas implantações** O fato de haver um CVE não quer dizer que o risco se aplique ao seu ambiente ou implantação específicos. Certifique-se de ler cada CVE para saber se seu ambiente foi afetado. Verifique a relação (total ou parcial) com o sistema operacional, aplicação, módulos e configurações instaladas no seu ambiente.

**Faça o gerenciamento de vulnerabilidades.** O [gerenciamento de vulnerabilidades](https://en.wikipedia.org/wiki/Vulnerability_management) é um processo iterativo para identificar, classificar, priorizar, remediar e mitigar vulnerabilidades. Isso significa entender como um risco se aplica à sua organização para priorizar corretamente as vulnerabilidades pendentes que precisam ser resolvidas.

**Esteja pronto para se comunicar** CVEs impactam os sistemas da sua empresa, tanto pelas próprias vulnerabilidades quanto pelo tempo de inatividade necessário para resolvê-las. Comunique-se e coordene-se com seus clientes internos e compartilhe as vulnerabilidades com a gestão da central de riscos da sua organização.

### Como a Red Hat trabalha com CVEs

Como uma das principais colaboradoras do software [open source](https://www.redhat.com/pt-br/topics/open-source/what-is-open-source), a Red Hat está sempre envolvida na comunidade de segurança. Nós somos uma [Autoridade de numeração CVE (CNA)](https://cve.mitre.org/cve/cna.html) e usamos IDs CVE para rastrear vulnerabilidades de segurança. A Red Hat Security mantém um [banco de dados de atualizações de segurança](https://access.redhat.com/security/security-updates/#/cve) aberto que você pode consultar pelo número do CVE.

[Explore o banco de dados CVE da Red Hat](https://access.redhat.com/security/security-updates/#/cve)

## O que é a API de dados de segurança da Red Hat?

O Red Hat Product Security oferece acesso a dados brutos de segurança na [página Dados de segurança](https://www.redhat.com/security/data/metrics/) e em formatos compatíveis com máquinas por meio da API.

Além das métricas e relatórios de segurança que a Red Hat oferece, os clientes podem usar esses dados para gerar as próprias métricas de acordo com seus casos.

A API de dados de segurança inclui definições de Linguagem de avaliação e vulnerabilidade aberta (OVAL), documentos de Framework de relatórios de vulnerabilidades comuns (CVRF) e dados de CVE. Os dados estão disponíveis no formato XML e JSON.

[Acesse a documentação sobre a API de segurança de dados da Red Hat](https://access.redhat.com/documentation/en-us/red_hat_security_data_api/1.0/html/red_hat_security_data_api/index)

##### EBOOK EM DESTAQUE

### Aumente a segurança em nuvem híbrida

Veja como proteger seus negócios com abordagens de segurança nativas em nuvem.

[Faça o download do ebook](https://www.redhat.com/pt-br/engage/boost-hybrid-cloud-security)

#### Saiba mais sobre segurança

- Guia: [Abordagem da Red Hat para a segurança em nuvem híbrida](https://www.redhat.com/pt-br/topics/security/hybrid-cloud-security-approach)
- Artigo: [Introdução à segurança da TI](https://www.redhat.com/pt-br/topics/security)
- Artigo: [O que é automação da segurança?](https://www.redhat.com/pt-br/topics/automation/what-is-security-automation)
- Artigo: [Modernize e proteja aplicações com DevSecOps](https://www.redhat.com/pt-br/partners/devsecops)

#### Recursos em destaque

- [Banco de dados CVE da Red Hat](https://access.redhat.com/security/security-updates/#/cve )
- [Centro de segurança de soluções da Red Hat](https://access.redhat.com/security/)
- [Dados de segurança da Red Hat](https://www.redhat.com/security/data/metrics/)
- [Respostas a vulnerabilidades da Red Hat](https://access.redhat.com/security/vulnerabilities)
- [API de dados de segurança da Red Hat](https://access.redhat.com/documentation/en-us/red_hat_security_data_api/1.0/html/red_hat_security_data_api/index)

### Explore a infraestrutura da Red Hat

[![img](https://www.redhat.com/cms/managed-files/styles/xlarge/s3/Logo-Red_Hat-Enterprise_Linux-A-Standard-RGB-360x75.png?itok=Q8EQEro9)](https://www.redhat.com/pt-br/technologies/linux-platforms/enterprise-linux)

O Red Hat Enterprise Linux é uma base estável e comprovada, versátil o suficiente para distribuir novas aplicações, virtualizar ambientes e criar uma nuvem híbrida segura. Tudo isso com a assistência do nosso suporte premiado.

[Saiba mais](https://www.redhat.com/pt-br/technologies/linux-platforms/enterprise-linux)

[![img](https://www.redhat.com/cms/managed-files/styles/xlarge/s3/Logo-Red_Hat-Satellite-A-Standard-RGB-360x75.png?itok=PvB4b1ql)](https://www.redhat.com/pt-br/technologies/management/satellite)

O jeito mais fácil de gerenciar a infraestrutura Red Hat para garantir operações de TI eficientes e em conformidade. Estabeleça processos e repositórios de conteúdo confiáveis para criar um ambiente seguro e baseado em padrões.

[Saiba mais](https://www.redhat.com/pt-br/technologies/management/satellite)



![Illustration - mail](https://www.redhat.com/cms/managed-files/illustration-mail.png)



#### Get more content like this

Sign up for our free newsletter, Red Hat Shares.

[Continue](https://engage.redhat.com/Global-Preference-Center?newsletter=RH-Shares&intcmp=7013a000002w0nSAAQ)

#### Trust Red Hat

Learn about Red Hat’s commitment to protecting customer data and privacy

[Read more](https://www.redhat.com/en/trust)

### SOBRE A RED HAT

A Red Hat é líder mundial no fornecimento de soluções empresariais open source. Utilizando uma abordagem de parceria com as comunidades, a Red Hat oferece tecnologias confiáveis e de alto desempenho em Linux, nuvem, containers e Kubernetes. Com serviços premiados de consultoria, treinamento e suporte, ajudamos nossos clientes a definir padrões entre diferentes ambientes, desenvolver aplicações nativas em nuvem, além de integrar, automatizar, proteger e gerenciar ambientes complexos.

- [Informações institucionais](https://www.redhat.com/pt-br/about/company)
- [Oportunidades de emprego](https://www.redhat.com/pt-br/jobs-overview)
- [Escritórios](https://www.redhat.com/pt-br/about/office-locations)
- [Modelo de desenvolvimento](https://www.redhat.com/pt-br/about/development-model)
- [Eventos](https://www.redhat.com/pt-br/events)
- [Sala de imprensa](https://www.redhat.com/pt-br/about/newsroom)
- [Blog](https://www.redhat.com/pt-br/blog)
- [Cool Stuff Store](https://coolstuff.redhat.com/)
- [Diversidade, equidade e inclusão](https://www.redhat.com/pt-br/about/our-culture/diversity-equity-inclusion/statement)
- 

### PRODUTOS

- [Red Hat Ansible Automation Platform](https://www.redhat.com/pt-br/technologies/management/ansible)
- [Red Hat Enterprise Linux](https://www.redhat.com/pt-br/technologies/linux-platforms/enterprise-linux)
- [Red Hat OpenShift](https://www.redhat.com/pt-br/technologies/cloud-computing/openshift)
- [Red Hat OpenShift Data Foundation](https://www.redhat.com/pt-br/technologies/cloud-computing/openshift-container-storage)
- [Red Hat OpenStack Platform](https://www.redhat.com/pt-br/technologies/linux-platforms/openstack-platform)
- [Veja todos os produtos](https://www.redhat.com/pt-br/technologies/all-products)

### FERRAMENTAS

- [Minha conta](https://sso.redhat.com/)
- [Suporte ao cliente](https://access.redhat.com/)
- [Recursos para parceiros](https://connect.redhat.com/)
- [Recursos para desenvolvedores](https://developers.redhat.com/)
- [Treinamento e certificação](https://www.redhat.com/pt-br/services/training-and-certification)
- [Comunidade de aprendizagem](https://learn.redhat.com/)
- [Red Hat Ecosystem Catalog](https://catalog.redhat.com/)
- [Biblioteca de recursos](https://www.redhat.com/pt-br/resources)

### EXPERIMENTE, COMPRE, VENDA

- [Central de avaliação de produtos](https://www.redhat.com/pt-br/products/trials)
- [Red Hat Store](https://www.redhat.com/en/store)
- [Red Hat Marketplace](https://marketplace.redhat.com/)
- [Comprar online (Japão)](https://www.redhat.com/pt-br/about/japan-buy)
- [Encontre um parceiro](http://redhat.force.com/finder/)
- [Contate o setor de vendas](https://www.redhat.com/pt-br/contact)
- [Contate o setor de treinamento](https://www.redhat.com/pt-br/services/training-and-certification/contact-us)
- [Contate a Red Hat Consulting](https://www.redhat.com/pt-br/services/consulting-overview#contact-us)

### COMUNICAÇÃO

- [Entre em contato](https://www.redhat.com/pt-br/contact)
- [Comentários e feedback](https://www.redhat.com/pt-br/feedback-sobre-o-site)
- [Redes sociais](https://www.redhat.com/pt-br/about/social)
- [Newsletter](https://engage.redhat.com/Global-Preference-Center?newsletter=RH-Shares&intcmp=7016000000154xCAAQ)

[![Red Hat](https://www.redhat.com/profiles/rh/themes/redhatdotcom/img/logo.svg)](https://www.redhat.com/pt-br)

© 2022 Red Hat, Inc.

- [Declaração de Privacidade](https://www.redhat.com/pt-br/about/privacy-policy)
- [Termos de uso](https://www.redhat.com/pt-br/about/terms-use)
- [Todas as políticas e diretrizes](https://www.redhat.com/pt-br/about/all-policies-guidelines)
- [Acessibilidade digital](https://www.redhat.com/pt-br/about/digital-accessibility)
- |Preferências de Cookies

[![Red Hat Summit](https://www.redhat.com/cms/managed-files/Logo-Red_Hat-Summit-A-Standard-RGB-02_0.svg)](http://www.redhat.com/summit/)

<iframe class="drift-frame-chat" scrolling="no" title="Drift Widget Chat Window" allow="autoplay; encrypted-media; fullscreen;" frameborder="0" src="https://js.driftt.com/core/chat?region=US&amp;driftEnableLog=false&amp;pageLoadStartTime=1645880669627" style="box-sizing: border-box; display: block; min-width: 0px; max-width: 100%; min-height: 0px; max-height: none; border: none; background: transparent; width: 400px !important; height: 0px;"></iframe>

<iframe class="drift-frame-controller" scrolling="no" title="Drift Widget Icon" allow="autoplay; encrypted-media; fullscreen;" frameborder="0" src="https://js.driftt.com/core?embedId=vtgnfrnufv54&amp;region=US&amp;forceShow=false&amp;skipCampaigns=false&amp;sessionId=5caed88e-335f-451b-af5f-8ccc61314e2d&amp;sessionStarted=1645881268.288&amp;campaignRefreshToken=8f579610-f179-4eca-8112-da95fba17ec8&amp;hideController=false&amp;pageLoadStartTime=1645880669627&amp;mode=CHAT&amp;driftEnableLog=false" style="box-sizing: border-box; display: block; min-width: 0px; max-width: 100%; min-height: 0px; max-height: none; bottom: 24px; border: none; background: transparent; width: 75.9943px; height: 0px;"></iframe>