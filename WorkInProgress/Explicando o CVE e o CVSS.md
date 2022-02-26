[Home](https://aiqon.com.br/blog) » [Cyber Security](https://aiqon.com.br/blog/category/cybersecurity/) » [Patch Management](https://aiqon.com.br/blog/category/cybersecurity/patch-management/) » Explicando o CVE e o CVSS

![img](https://sp-ao.shortpixel.ai/client/to_auto,q_lossy,ret_img,w_1000,h_500/https://aiqon.com.br/blog/wp-content/uploads/2020/02/cve-e-cvss-1.jpg)

[PATCH MANAGEMENT](https://aiqon.com.br/blog/category/cybersecurity/patch-management/)

# Explicando o CVE e o CVSS

Publicado

 

###### O CVE E O CVSS ESTÃO ENTRE OS ASPECTOS MAIS INCOMPREENDIDOS DE *PATCHING* HOJE EM DIA. EXPLORE AS DIFERENÇAS E VEJA COMO ELES AFETAM A SUA ESTRATÉGIA DE *PATCHING*.

Apesar de muitos gerentes de T.I estarem familiarizados com esses termos, CVE e CVSS estão entre os aspectos mais incompreendidos em *patching* hoje em dia. Essas duas terminologias diferentes são sinônimos de sistemas operacionais, vulnerabilidades de *software* e *patching*. Por isso resolvemos explicar o CVE e o CVSS.

## O que é o CVE?

O número do CVE (sigla em inglês para *Common Vulnerabilities and Exposures*, traduzido para Exposições e vulnerabilidades comuns) é um identificador usado por fornecedores como a Microsoft, RedHat e Adobe para catalogar vulnerabilidades individuais dos quais patches são providos como solução. Por exemplo, toda página de um livro tem um único número, isto resolve o problema sobre precisar achar uma informação específica de uma página rapidamente.

Normalmente, todos os números de CVE seguem este padrão: CVE-nnnn-nnnn. Como podemos ver, há escopo para milhões de vulnerabilidades.

“Nossos clientes devem se sentir confiantes de que seus números CVE não pertencem a nenhum fornecedor de software específico.” Disse Robert Brown, Diretor de Serviços da Verismic Software.” Portanto, é um banco de dados imparcial e independente para que todos os fornecedores publiquem suas vulnerabilidades.”

Isso significa também que os fornecedores precisam publicar conteúdos transparentemente para os bancos de dados. Isso oferece pelo menos uma garantia da precisão dos dados. Cada companhia que deseja publicar seus anúncios de vulnerabilidade precisam se tornar um CNA (sigla em inglês para CVE Numbering Authority, traduzido para Autoridade de Numeração CVE) antes de sua participação ser considerada confiável.

Os fornecedores devem incluir o máximo de informações possíveis para cada registro de CVE. Por exemplo:

- Número CVE
- Descrição da vulnerabilidade
- Severidade
- Referências a outros registros de CVE (conhecidos como *supersession*)
- Histórico de mudanças
- Data de publicação

## O que é a pontuação CVSS?

O CVSS (sigla em inglês para Common Vulnerability Scoring System) é uma pontuação atribuída independentemente (de 0 à 10) na qual é baseada em uma grande quantidade de fatores para determinar a importância da vulnerabilidade. Para comparar a pontuação de CVSS, vamos ver como a Microsoft pontua suas vulnerabilidades.

O sistema de avaliação é relativamente simples:

1. **Crítico** – Uma vulnerabilidade que pode permitir a execução de código remoto sem a interação do usuário ou onde os código são executados sem avisos ou prompts.
2. **Importante** – Vulnerabilidades onde o cliente é comprometido com avisos ou prompts e cuja exploração pode resultar em comprometimento de dados.
3. **Moderada** – O impacto é mitigado por uma série de fatores como autenticação ou aplicativos não nativos sendo afetados.
4. **Baixa** – O impacto é mitigado de forma abrangente pelas características do componente mitigado.
5. **N/D** – Não disponível

Contudo, a abordagem da Microsoft alto certifica vulnerabilidades em seus produtos.

Gerar uma pontuação CVSS é bem complexa, mas leva em consideração algumas questões importantes:

1. Quão provável é da vulnerabilidade ser explorada? Você precisará de acesso físico ou pela rede? E você precisará de privilégios elevados?
2. Você pode explorá-lo pela internet ou você precisará de acesso físico?
3. Um software ou uma configuração específica de software será necessário?
4. Quanto de interação do usuário final é necessário?

Cada uma das questões acima (e muitas outras) são organizadas em uma sub-pontuação calculada. A pontuação então é calculada em uma nota que vai de 0 à 10. Os especialista do setor acreditam que isso oferece uma forma mais precisa de determinar a rapidez com que você deve agir caso haja alguma dessas vulnerabilidades em seu ambiente.

|               |                    |
| ------------- | ------------------ |
| **Pontuação** | **Pontuação CVSS** |
| Nenhuma       | 0.0                |
| Baixa         | 0.1 – 3.9          |
| Média         | 4.0 – 6.9          |
| Alta          | 7.0 – 8.9          |
| Crítica       | 9.0 – 10.0         |

## As pontuações CVSS são realmente necessárias? Prove!

Vamos pegar alguns updates do Patch Tuesday de agosto de 2019 e alguns outros para comparar

| **FORNECEDOR**          | **NOME DO PATCH**     | **SEGURANÇA DO FORNECEDOR** | **PONTUAÇÃO CVSS** |
| ----------------------- | --------------------- | --------------------------- | ------------------ |
| Google                  | Chrome_v76.0.3809.100 | N/D                         | Alto – 8.8         |
| Microsoft               | KB4462137             | Crítico                     | Alto – 7.8         |
| Microsoft               | KB4474419             | N/D                         | Crítico – 9.8      |
| Microsoft               | KB4508433             | N/D                         | Crítico – 9.8      |
| The Document Foundation | LibreOffice_v6.2.5    | N/D                         | Crítico – 9.8      |

Como podemos ver no exemplo acima, a severidade do fornecedor e da pontuação CVSS nem sempre estão alinhadas. Se você pegar a avaliação de severidade da Microsoft pelo valor nominal, você potencialmente estará desperdiçando dois dos ativos mais preciosos que você tem – tempo e recurso. Lançar muitos patches através de um enorme ambiente de T.I distribuído leva tempo.

Quanto mais tempo uma vulnerabilidade é deixada sem um patch de correção, maior o risco de dela ser explorada por um atacante. Evidências sugerem que ataques contra vulnerabilidades conhecidas tem um pico nas horas ou dias após o lançamento dos patches – por isso é importante saber o quão urgente uma vulnerabilidade é.

## Qual a solução?

Pegue qualquer vulnerabilidade e comece a analisar as pontuações avaliadas independentemente, como o CVSS. Todo mês a US-CERT / NIST usa o CVSS para avaliar a maioria dos patches no mesmo dia em que eles são lançados. Isso dá uma melhor ideia do nível de risco de uma vulnerabilidade em particular para o seu negócio.

Baixa disponibilidade pode ser extremamente custosa para um negócio. A melhor abordagem para aplicar patches é ter uma janela dedicada de tempo de inatividade todos os meses para atualizar os sistemas. Caso tenha algum problema de compatibilidade com um patch e os sistemas precisam ser revertidos ao estado anterior, isso acaba aumentando o tempo de indisponibilidade de um serviço e pode impactar o funcionamento do negócio de uma forma geral.

Entretanto, este é um serviço que oferecemos com o cliente. Nós analisamos o código binário de cada atualização de patch e começamos a fase de testes e piloto do update antes de implementá-los via Syxsense. Isso nos permite descobrir quaisquer problemas com as atualizações de patch antes delas serem implementadas.

Patching é sobre melhorar sua postura de segurança. Adotando uma abordagem calculada e usando pontuações avaliadas de forma independente, você pode confidentemente priorizar quais patches você precisa implementar em seu ambiente.

[![CVE CVSS](https://sp-ao.shortpixel.ai/client/to_auto,q_lossy,ret_img,w_1000,h_250/https://aiqon.com.br/blog/wp-content/uploads/2019/12/syxsense-trial-bottom.jpg)](https://lps.aiqon.com.br/syxsense_trial)

 

Saiba mais: [Como criar uma estratégia de patching para o seu ambiente](https://aiqon.com.br/blog/estrategia-para-gerenciamento-de-patch/)

### Compartilhe

- [Clique para compartilhar no Twitter(abre em nova janela)](https://aiqon.com.br/blog/explicar-o-cve-e-o-cvss/?share=twitter&nb=1)
- [Clique para compartilhar no Facebook(abre em nova janela)](https://aiqon.com.br/blog/explicar-o-cve-e-o-cvss/?share=facebook&nb=1)
- [Clique para compartilhar no LinkedIn(abre em nova janela)](https://aiqon.com.br/blog/explicar-o-cve-e-o-cvss/?share=linkedin&nb=1)
- [Clique para compartilhar no WhatsApp(abre em nova janela)](https://aiqon.com.br/blog/explicar-o-cve-e-o-cvss/?share=jetpack-whatsapp&nb=1)
- [Clique para compartilhar no Telegram(abre em nova janela)](https://aiqon.com.br/blog/explicar-o-cve-e-o-cvss/?share=telegram&nb=1)
- 

### Curtir isso:

<iframe class="post-likes-widget jetpack-likes-widget" name="like-post-frame-172206828-329-621a25699b32d" src="https://widgets.wp.com/likes/#blog_id=172206828&amp;post_id=329&amp;origin=aiqon.com.br&amp;obj_id=172206828-329-621a25699b32d" height="55px" width="100%" frameborder="0" scrolling="no" title="Curtir ou reblogar" style="box-sizing: border-box; max-width: 100%; margin: 0px; border-width: 0px; display: block;"></iframe>





- [patch](https://aiqon.com.br/blog/tag/patch/)
- [segurança](https://aiqon.com.br/blog/tag/seguranca/)
- [syxsense](https://aiqon.com.br/blog/tag/syxsense/)

### ARTIGOS RECOMENDADOS