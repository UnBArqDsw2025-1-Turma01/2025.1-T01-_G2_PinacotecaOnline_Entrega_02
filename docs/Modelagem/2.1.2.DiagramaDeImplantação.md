# 2.1.2. Diagrama de Implantação

## Introdução

O diagrama de implantação, definido pela UML (Unified Modeling Language), é utilizado para representar a arquitetura física de um sistema, destacando como os componentes de software são distribuídos entre os recursos de hardware. Ele mostra de forma clara e objetiva a infraestrutura necessária para a execução do sistema, como servidores, dispositivos e conexões de rede.

Por ser independente de linguagem de programação, esse diagrama é amplamente aplicável, servindo tanto para sistemas web, móveis quanto embarcados. Sua principal função é documentar a relação entre hardware e software, evidenciando onde cada parte do sistema será executada.

## Objetivo

Este documento tem como objetivo principal apresentar o diagrama de implantação no contexto do projeto, com o propósito de facilitar o entendimento dos protocolos utilizados na migração de dados entre os diferentes processos do sistema. Além disso, busca auxiliar na comunicação entre os membros do grupo e os stakeholders do projeto. Para a definição das tecnologias empregadas, foi consultado o quadro de conhecimentos, garantindo a escolha de soluções alinhadas às competências e necessidades do projeto.

## Metodologia

A construção desse diagrama de implantação segue as diretrizes da UML (Unified Modeling Language), fornecendo tanto uma notação padronizada representando os componentes de software, quanto suas interações no ambiente de execução do software. No desenvolvimento do Diagrama de Implantação foi utilizado a ferramenta draw.io. Nesse diagrama, apontamos os principais elementos de infraestrutura que são necessários para o funcionamento do sistema da Pinacoteca Online: Servidor de Bancos de Dados, Servidor de aplicação, Servidor de aplicação e o Aplicativo Web.

O processo principal envolve fazer o mapeamento da distribuição do sistema estando em um ambiente de implantação típico, conectando os componente com as interações necessárias para a execução das funcionalidades, interações essas que são: o acesso ao front-end, a lógica de negócios no back-end e a persistência de dados no banco.

## Descrição

O diagrama de implantação do sistema da Pinacoteca Online é composto pelos seguintes componentes principais: Aplicativo Web (Browser), Servidor de Aplicação Front-end (ReactJS), Servidor de Aplicação Back-end (Node.js) e Servidor de Banco de Dados (MongoDB). Esses elementos são organizados para garantir a execução eficiente das funcionalidades do sistema, desde a interação do usuário até o armazenamento e recuperação de dados.

- **Aplicativo Web (Browser)**: Representa a interface do usuário, acessada por meio de navegadores web. Ele renderiza a interface gráfica desenvolvida em **ReactJS**, permitindo interações dinâmicas e intuitivas. A comunicação com o servidor front-end ocorre via protocolo **HTTP/HTTPS**, enviando requisições e recebendo respostas para exibir conteúdos atualizados.

- **Servidor de Aplicação Front-end (ReactJS)**: Hospeda a aplicação ReactJS, que gerencia a lógica de apresentação e a experiência do usuário. Processa requisições do navegador, servindo arquivos estáticos (HTML, CSS, JavaScript) e garantindo a renderização _client-side_. Comunica-se com o back-end por meio de chamadas **API REST**, utilizando **HTTP/HTTPS**, para buscar ou enviar dados.

- **Servidor de Aplicação Back-end (Node.js)**: Implementado com **Node.js**, é responsável pela lógica de negócios. Processa requisições do front-end, executando operações como autenticação, validação de dados e gerenciamento de sessões, e se comunica com o banco de dados para persistência ou recuperação de informações. A conexão com o **MongoDB** utiliza drivers específicos, garantindo eficiência e segurança.

- **Servidor de Banco de Dados (MongoDB)**: Armazena os dados do sistema em um banco **NoSQL MongoDB**, ideal para grandes volumes de dados não estruturados. Responde às consultas do back-end, permitindo operações CRUD (criação, leitura, atualização e exclusão). A conexão é segura, utilizando autenticação e criptografia quando necessário.

## Diagrama de Implantação

<font size="2"><p style="text-align: center"><b>Figura 1:</b> Diagrama de Implantação</p></font>

<div style="text-align: center;"> 

![DiagramaImplantacaoV1](assets/images/implantaçãov1.png)

</div>

<font size="2"><p style="text-align: center"><b>Autor:</b> Renan Araújo, 2025</p></font>

## Quadro de Conhecimentos

- [Quadro de Conhecimentos](https://unbarqdsw2025-1-turma01.github.io/2025.1-T01-_G2_PinacotecaOnline_Entrega_01/#/Base/Extra/quadro-de-conhecimentos): Documento que detalha as competências e conhecimentos da equipe, utilizado como base para a escolha das tecnologias do projeto.

## Referências

> IBM. (2023). Topologies: Deployment Diagrams. Disponível em: <https://www.ibm.com/docs/pt-br/rsas/7.5.0?topic=topologies-deployment-diagrams>. Acesso em: 08/05/2025.

> BOOCH, Grady; RUMBAUGH, James; JACOBSON, Ivar. The Unified Modeling Language User Guide. 2nd ed. Boston: Addison-Wesley, 2005.

> O Guia Fácil de Diagramas de Implantação UML. Disponível em: <https://creately.com/blog/pt/diagrama/tutorial-do-diagrama-de-implantacao/>. Acesso em: 05 maio 2025.


## Histórico de Versões

| Versão | Data       | Descrição                                                         | Autor(es)                                            | Revisor(es)                                          |
| ------ | ---------- | ----------------------------------------------------------------- | ---------------------------------------------------- | ---------------------------------------------------- |
| 1.0    | 01/05/2025 | Adição da primeira versão do Diagrama                             | [Renan Araújo](https://github.com/renantfm4)         | [Lucas Heler](https://github.com/Akaeboshi)          |
| 1.1    | 05/05/2025 | Adição dos parágrafos de Objetivo e Metodologia                   | [Lucas Heler](https://github.com/Akaeboshi)          | [Mateus Cavalcante](https://github.com/mateuscavati) |
| 1.2    | 06/05/2025 | Adição do parágrafo Introdução                                    | [Mateus Cavalcante](https://github.com/mateuscavati) | [Renan Araújo](https://github.com/renantfm4)         |
| 1.3    | 06/05/2025 | Descrição do Diagrama                                             | [Renan Araújo](https://github.com/renantfm4)         | [Leandro Almeida](https://github.com/LeanArs)        |
| 1.4    | 08/05/2025 | Adição de menção ao quadro de conhecimentos e seção extra         | [Renan Araújo](https://github.com/renantfm4)         |         |
| 1.5    | 08/05/2025 | Adicionando referências      | [Renan Araújo](https://github.com/renantfm4)         |         |