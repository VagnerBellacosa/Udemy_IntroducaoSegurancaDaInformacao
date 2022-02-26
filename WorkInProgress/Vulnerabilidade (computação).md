# Vulnerabilidade (computação)

Origem: Wikipédia, a enciclopédia livre.

| [![Wikitext.svg](https://upload.wikimedia.org/wikipedia/commons/thumb/c/ce/Wikitext.svg/40px-Wikitext.svg.png)](https://pt.wikipedia.org/wiki/Wikipédia:Wikificação) | **Esta página ou se(c)ção precisa ser [formatada para o padrão wiki](https://pt.wikipedia.org/wiki/Wikipédia:Wikificação).** Por favor ajude a [formatar](https://pt.wikipedia.org/wiki/Ajuda:Guia_de_edição/Formatação) esta página de acordo com as [**diretrizes**](https://pt.wikipedia.org/wiki/Wikipédia:Wikificação#Como_ajudar) estabelecidas. *(Novembro de 2017)* |
| ------------------------------------------------------------ | ------------------------------------------------------------ |
|                                                              |                                                              |

| [![Portal](https://upload.wikimedia.org/wikipedia/commons/thumb/c/c9/Portal.svg/36px-Portal.svg.png)](https://pt.wikipedia.org/wiki/Ficheiro:Portal.svg) | A Wikipédia tem o portal:[Portal das tecnologias de informação](https://pt.wikipedia.org/wiki/Portal:Tecnologias_de_informação) |
| ------------------------------------------------------------ | ------------------------------------------------------------ |
|                                                              |                                                              |

Em [segurança de computadores](https://pt.wikipedia.org/wiki/Segurança_de_computadores), uma **vulnerabilidade ou falha de segurança** é uma fraqueza que permite que um [atacante](https://pt.wikipedia.org/wiki/Hacker) reduza a [garantia da informação (Integridade)](https://pt.wikipedia.org/wiki/Integridade_de_dados) de um sistema. **Vulnerabilidade** é a interseção de três elementos: uma suscetibilidade ou falha do sistema, acesso do atacante à falha e a capacidade do atacante de explorar a falha.[[1\]](https://pt.wikipedia.org/wiki/Vulnerabilidade_(computação)#cite_note-1) Para explorar uma vulnerabilidade, uma atacante deve ter pelo menos uma ferramenta ou técnica aplicável que possa conectar a uma fraqueza do sistema. Desta forma, vulnerabilidade também é conhecida como [superfície de ataque](https://pt.wikipedia.org/w/index.php?title=Superfície_de_ataque&action=edit&redlink=1).

**Vulnerabilidade** é definida como uma condição que, quando explorada por um atacante, pode resultar em uma violação de segurança. Exemplos de vulnerabilidades são falhas no projeto, na implementação ou na configuração de programas, serviços ou equipamentos de rede. Um ataque de exploração de vulnerabilidades ocorre quando um atacante, utilizando-se de uma vulnerabilidade, tenta executar ações maliciosas, como invadir um sistema, acessar informações confidenciais, disparar ataques contra outros computadores ou tornar um serviço inacessível.[[2\]](https://pt.wikipedia.org/wiki/Vulnerabilidade_(computação)#cite_note-2)

[Gerenciamento de vulnerabilidade](https://pt.wikipedia.org/w/index.php?title=Gerenciamento_de_vulnerabilidade&action=edit&redlink=1) é a prática cíclica de identificar, classificar, remediar e mitigar vulnerabilidades.[[3\]](https://pt.wikipedia.org/wiki/Vulnerabilidade_(computação)#cite_note-3) Esta prática geralmente refere-se a [vulnerabilidades de software](https://pt.wikipedia.org/w/index.php?title=Vulnerabilidades_de_software&action=edit&redlink=1) nos sistemas de computador.

Esta mesma pode ser explorada em um determinado sistema ou serviço vulnerável que esteja rodando na máquina.

As vulnerabilidades mais exploradas nos dias de hoje, são as do tipo [buffer overflow](https://pt.wikipedia.org/wiki/Buffer_overflow), que muitas vezes pode dar privilégios de [administrador](https://pt.wikipedia.org/wiki/Superusuário) para o invasor, rodar códigos maliciosos remotamente, burlar particularidades de cada sistema, ataques de Negação de Serviços ([DDoS](https://pt.wikipedia.org/wiki/DDoS)), e acesso irrestrito ao sistema.

Além dessas, outra vulnerabilidade bastante recorrente nos sistemas é a **enumeração de usuários**. Essa vulnerabilidade será apresentada a seguir.

## Índice



- [1Vulnerabilidade: enumeração de usuários](https://pt.wikipedia.org/wiki/Vulnerabilidade_(computação)#Vulnerabilidade:_enumeração_de_usuários)
- [2Ferramentas para exploração de vulnerabilidades](https://pt.wikipedia.org/wiki/Vulnerabilidade_(computação)#Ferramentas_para_exploração_de_vulnerabilidades)
- [3Referências](https://pt.wikipedia.org/wiki/Vulnerabilidade_(computação)#Referências)
- [4Ver também](https://pt.wikipedia.org/wiki/Vulnerabilidade_(computação)#Ver_também)

## Vulnerabilidade: enumeração de usuários

A enumeração de [usuário](https://pt.wikipedia.org/wiki/Usuário_(computação)) é uma prática utilizada para identificar os usuários ativos em um determinado sistema. Geralmente ela é utilizada para viabilizar ataques de [Força bruta](https://pt.wikipedia.org/wiki/Força_Bruta). A constatação da vulnerabilidade se dá através da possibilidade de discernir entre usuário válidos e inválidos em uma aplicação. Existem várias falhas nas aplicações que permitem a exploração dos usuários, no entanto, esse tipo de falha é mais comum ser encontradas nos mecanismo de [autenticação](https://pt.wikipedia.org/wiki/Autenticação).

Comumente, um atacante irá interagir com o mecanismo de autenticação da aplicação na tentativa de identificar o comportamento do sistema em resposta às requisições efetuadas em diferentes cenários de autenticação, por exemplo, utilizando um usuário válido e outro inválido. Em alguns casos, as aplicações fornecem respostas que revelam se um determinado usuário existe na [base de dados](https://pt.wikipedia.org/wiki/Banco_de_dados) quando uma credencial inválida é utilizada na requisição de autenticação.

Os testes de enumeração de usuários valida se a aplicação fornece, direta ou indiretamente, alguma informação que permita a distinção entre usuários válidos de uma aplicação. Abaixo serão apresentadas algumas abordagens que podem ser utilizadas para nortear os testes no sentido de verificar a vulnerabilidade da aplicação quanto à segurança da informação.

**Cenários de teste para a enumeração de usuários com base nas respostas das páginas**













**Enumeração de usuários com base nos códigos de erros das páginas de login**

Algumas aplicações web apresentam códigos de erros ou mensagens específicas que podem ser analisadas pelos atacantes;

**Enumeração de usuários com base em URLs**

Algumas aplicações web realizam redirecionamento de página quando falhas de autenticação acontecem. As URLs utilizadas para redirecionamentos podem ser analisadas para identificar os usuários válidos.



**Enumeração de usuários com base nos códigos de respostas do servidor (Response Code)**

Geralmente os servidores de aplicação, quando não são configurados de forma adequada, acabam apresentando mensagem de erro padrão para requisição recursos/diretórios. Esses response na maioria das vezes são:



Algumas aplicações são desenvolvidas utilizando princípios [REST](https://pt.wikipedia.org/wiki/REST), permitindo assim que os recursos da aplicação, como a conta do usuário, possam ser associados à URLs. (Exemplo: A URL **http:// www.teste.com.br/usuario01** faz referencia à conta do usuário 01). Dessa forma, um atacante pode utilizar os response code retornado pelo servidor para enumerar os usuários da aplicação.



No primeiro caso o usuário existe mas a página não é exibida visto que o servidor responde com o código **”403 Forbidden”**. Já no segundo caso, o código **”404 Not Found”** indica que o usuário não existe na base da aplicação. Com essas informações é possível a enumeração dos usuários da aplicação por um atacante.

Nota: Nem sempre o servidor apresenta um response code **404 Not Found** quando um recurso não existente for solicitado. Ao invés, ele responde com o response code **200 OK** mas com um imagem que representa o erro. Para esses casos, um atacante atente associará a imagem de erro à um usuário não existente. Esse mesmo raciocínio pode ser utilizado para qualquer resposta enviado pelo servidor, bastando diferenciar qual tipo de resposta representa um usuário válido e qual representa um usuário inválido.

**Enumeração de usuários com base nas funcionalidades de recuperação de senha**

Aplicações que disponibilizam funcionalidades de recuperação de senhas, muitas vezes permitem que os usuários possam ser enumerados com base nas mensagens que apresentam:



## Ferramentas para exploração de vulnerabilidades

Existem ferramentas específicas para se explorar as vulnerabilidades, cada ferramenta para a sua respectiva vulnerabilidade a ser explorada (na maioria das vezes escritas em [linguagem C](https://pt.wikipedia.org/wiki/Linguagem_C) e [Assembly](https://pt.wikipedia.org/wiki/Assembly)), essas ferramentas são chamadas de [exploits](https://pt.wikipedia.org/wiki/Exploit).

## Referências

1. [↑](https://pt.wikipedia.org/wiki/Vulnerabilidade_(computação)#cite_ref-1) [«The Three Tenents of Cyber Security»](https://web.archive.org/web/20090605095435/http://spi.dod.mil/tenets.htm). U.S. Air Force Software Protection Initiative. Consultado em 15 de dezembro de 2009. Arquivado do [original](http://www.spi.dod.mil/tenets.htm) em 5 de junho de 2009
2. [↑](https://pt.wikipedia.org/wiki/Vulnerabilidade_(computação)#cite_ref-2) [«Cartilha de Segurança -- Ataques na Internet»](https://cartilha.cert.br/ataques/). *cartilha.cert.br*. Consultado em 20 de junho de 2021
3. [↑](https://pt.wikipedia.org/wiki/Vulnerabilidade_(computação)#cite_ref-3) Foreman, P: *Vulnerability Management*, page 1. Taylor & Francis Group, 2010. [ISBN 978-1-4398-0150-5](https://pt.wikipedia.org/wiki/Especial:Fontes_de_livros/9781439801505)

## Ver também

- [Exploit](https://pt.wikipedia.org/wiki/Exploit)

| [![Ícone de esboço](https://upload.wikimedia.org/wikipedia/commons/thumb/d/d7/Computer.svg/30px-Computer.svg.png)](https://pt.wikipedia.org/wiki/Ficheiro:Computer.svg) | *Este artigo sobre [informática](https://pt.wikipedia.org/wiki/Informática) é um [esboço](https://pt.wikipedia.org/wiki/Wikipédia:Esboço). Você pode ajudar a Wikipédia **[expandindo-o](https://pt.wikipedia.org/w/index.php?title=Vulnerabilidade_(computação)&action=edit)**.* |
| ------------------------------------------------------------ | ------------------------------------------------------------ |
|                                                              |                                                              |

- [![img](https://upload.wikimedia.org/wikipedia/commons/thumb/d/d7/Crystal_Clear_app_ktalkd.png/25px-Crystal_Clear_app_ktalkd.png)](https://pt.wikipedia.org/wiki/Ficheiro:Crystal_Clear_app_ktalkd.png) **[Portal das tecnologias de informação](https://pt.wikipedia.org/wiki/Portal:Tecnologias_de_informação)**

[Categorias](https://pt.wikipedia.org/wiki/Especial:Categorias): 

- [Terminologia informática](https://pt.wikipedia.org/wiki/Categoria:Terminologia_informática)
- [Segurança da informação](https://pt.wikipedia.org/wiki/Categoria:Segurança_da_informação)
- [Crackers](https://pt.wikipedia.org/wiki/Categoria:Crackers)
- [Falhas em segurança de computadores](https://pt.wikipedia.org/wiki/Categoria:Falhas_em_segurança_de_computadores)
- [Cibersegurança](https://pt.wikipedia.org/wiki/Categoria:Cibersegurança)

- Esta página foi editada pela última vez às 16h06min de 22 de dezembro de 2021.