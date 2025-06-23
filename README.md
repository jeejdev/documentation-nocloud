<p align="center">
      <img src="./img/noCloud_logo.png" alt="logo noCloud" width="200">
<hr>

<span id="topo">
<p align="center">
    <a href="#sobre">Sobre</a>  |
    <a href="#backlogs">Backlogs, Épicos & User Stories</a>  |
    <a href="#tecnologias">Tecnologias</a>  |
    <a href="#equipe">Equipe</a> |
    <a href="#links">Links úteis</a>
</p>

<span id="sobre">

## :bookmark_tabs: Sobre o projeto

Em parceria com a empresa Visiona, o projeto visa desenvolver uma aplicação mobile integrada à computação em nuvem, com foco no mapeamento automático de nuvens e sombras de nuvens em imagens capturadas pelo sensor WPM, a bordo do satélite CBERS4A. Essa aplicação tem como objetivo fornecer máscaras de nuvens de alta precisão para as imagens adquiridas, facilitando o monitoramento e a análise de diversas áreas de interesse no Brasil.

## :warning: Problemática

A ausência de máscaras de nuvens nas imagens do satélite CBERS4A/WPM limita a capacidade de análise de grandes volumes de imagens em áreas extensas, especialmente em regiões tropicais com alta cobertura de nuvens. Quando realizado manualmente, esse processo é custoso e demorado, dificultando a automação de procedimentos em aplicações que exigem alta precisão e eficiência.

## :white_check_mark: Proposta de Solução

Desenvolvimento de um serviço e uma aplicação mobile em nuvem que automatiza o mapeamento de nuvens e sombras de nuvens em imagens do satélite CBERS4A/WPM, utilizando modelos de Deep Learning. A solução permitirá a definição de área e período de interesse, acesso às imagens correspondentes, mapeamento automático de nuvens e sombras, visualização dos resultados em uma interface de mapas, e download das máscaras em formato vetorial. Isso tornará o processo de análise mais eficiente, preciso e acessível para os usuários.

:pushpin: Status do Projeto: **🚧 Em andamento**

## 🏁 Entregas de Sprints

Cada entrega será realizada a partir da criação de uma **tag** em cada repositório (Front, Back), além da criação de uma branch no repositório da documentação com um relatório completo de tudo o que foi desenvolvido naquela sprint. Observe a relação a seguir:
| Sprint | Previsão de entrega | Status | Histórico |
|:--:|:----------:|:-------------------|:-------------------------------------------------:|
| 01 | 29/09/2024 | ✔️ Concluída| [Ver relatório](https://github.com/noCloud-Visiona/documentation/releases/tag/SPRINT_1) |
| 02 | 20/10/2024 | ✔️ Concluída| [Ver relatório]() |
| 03 | 10/11/2024 | ✔️ Concluída| [Ver relatório](https://github.com/noCloud-Visiona/documentation/releases/tag/SPRINT_3) |
| 04 | 01/12/2023 | 🚧 Em andamento| [Ver relatório]() |

<!--# 🚧 Em andamento -->
<!--# ✔️ Concluída -->

→ [Voltar ao topo](#topo)

<span id="backlogs">

# :dart: Backlogs, Épicos & User Stories

<div>

## Backlog

| **Sprint** | **MVP** |
|------------|---------|
| Sprint 1   | Tela de Login e Autenticação Básica, onde o usuário pode fazer login com suas credenciais e acessar a aplicação. |
| Sprint 1   | CRUD de usuário, possibilitando cadastro, edição, exclusão e visualização de dados dos usuários. |
| Sprint 1   | Primeira versão funcional do algoritmo de identificação de nuvens e sombras em uma imagem de satélite enviada pelo usuário. |
| Sprint 1   | Exibição do histórico de análises de imagens do usuário, permitindo visualizar as análises passadas. |
| Sprint 2   | Funcionalidade para atualizar e excluir descrições das imagens analisadas no histórico do usuário. |
| Sprint 2   | Consumir a API do INPE para buscar imagens com base na localização e data escolhida pelo usuário. |
| Sprint 2   | Serviço de download da imagem processada em formato PNG e geração de um PDF contendo os detalhes da análise. |
| Sprint 3   | Exibir diferentes camadas da imagem (sem nuvens, com nuvens, com sombras) para uma análise mais precisa. |
| Sprint 3   | Visualizar as imagens analisadas georreferenciadas em um mapa interativo. |
| Sprint 4   | Refatoração final, correções de bugs e preparação para o deploy em produção. |

---

## Requisitos Funcionais

| **ID**   | **Descrição** |
|----------|---------------|
| RF01     | O sistema deve permitir que o usuário faça login com suas credenciais (e-mail e senha). |
| RF02     | O sistema deve permitir o cadastro de novos usuários, além de edição e exclusão de contas existentes. |
| RF03     | O sistema deve permitir que o usuário faça o upload de imagens de satélite para análise de nuvens e sombras. |
| RF04     | O sistema deve exibir o histórico de análises de imagens do usuário, com opção de edição e exclusão. |
| RF05     | O sistema deve consumir a API do INPE para buscar imagens de satélite com base na localização e data selecionada pelo usuário. |
| RF06     | O sistema deve permitir o download da imagem processada em formato PNG e de um PDF contendo informações da análise. |
| RF07     | O sistema deve exibir diferentes camadas da imagem analisada (sem nuvens, com nuvens, com sombras) para uma análise detalhada. |
| RF08     | O sistema deve mostrar as imagens analisadas georreferenciadas em um mapa interativo. |

## Requisitos Não Funcionais

| **ID**   | **Descrição** |
|----------|---------------|
| RNF01    | O sistema deve garantir a segurança das credenciais de login, utilizando criptografia para armazenar senhas. |
| RNF02    | O sistema deve ser responsivo, funcionando tanto em dispositivos móveis quanto em navegadores web. |
| RNF03    | O sistema deve processar e responder as requisições do usuário dentro de um tempo máximo de 5 segundos. |
| RNF04    | O sistema deve ser compatível com diferentes navegadores (Chrome, Firefox, Safari). |
| RNF05    | O sistema deve garantir alta disponibilidade, com tempo de inatividade inferior a 1% por mês. |
| RNF06    | O sistema deve armazenar dados das análises de imagens em um banco de dados não relacional (ex: MongoDB ou Firebase). |
| RNF07    | O sistema deve ter suporte a até 10 mil usuários simultâneos. |

---

## User Stories

| **US**   | **Atores**        | **Ação**                                              | **Motivo**                                                    |
|----------|-------------------|-------------------------------------------------------|---------------------------------------------------------------|
| US01     | Usuário Comum      | Realizar login na aplicação                           | Para acessar as funcionalidades da aplicação.                  |
| US02     | Administrador      | Gerenciar usuários (criar, editar, excluir)           | Para manter os dados dos usuários atualizados.                 |
| US03     | Usuário Comum      | Fazer upload de imagens de satélite                   | Para analisar nuvens e sombras nas imagens.                    |
| US04     | Usuário Comum      | Visualizar histórico de análises                      | Para acessar análises passadas e gerenciar as imagens.          |
| US05     | Usuário Comum      | Editar e excluir descrições de análises               | Para manter o histórico de análises atualizado.                |
| US06     | Usuário Comum      | Buscar imagens por localização e data                 | Para encontrar imagens específicas para análise.                |
| US07     | Usuário Comum      | Fazer download da imagem processada e de um relatório | Para obter cópias locais das análises feitas na plataforma.     |
| US08     | Usuário Comum      | Visualizar diferentes camadas da imagem analisada     | Para analisar mais detalhadamente nuvens e sombras.             |
| US09     | Usuário Comum      | Visualizar as imagens georreferenciadas no mapa       | Para identificar a localização exata das imagens analisadas.    |
| US10     | Administrador      | Fazer deploy da aplicação                             | Para disponibilizar a aplicação ao público de forma estável.    |

</div>

→ [Voltar ao topo](#topo)

<span id="tecnologias">

# 🛠️ Tecnologias

Linguagens, bibliotecas e tecnologias utilizadas na construção do projeto:

<img src="https://img.shields.io/badge/Python-3776AB?style=for-the-badge&logo=python&logoColor=white" alt="Python" />
<img src="https://img.shields.io/badge/Firebase-FFCA28?style=for-the-badge&logo=firebase&logoColor=white" alt="Firebase" />
<img src="https://img.shields.io/badge/PostgreSQL-336791?style=for-the-badge&logo=postgresql&logoColor=white" alt="PostgreSQL" />
<img src="https://img.shields.io/badge/Postman-FF6C37?style=for-the-badge&logo=postman&logoColor=white" alt="Postman" />
<img src="https://img.shields.io/badge/Flutter-02569B?style=for-the-badge&logo=flutter&logoColor=white" alt="Flutter" />
<img src="https://img.shields.io/badge/TypeScript-007ACC?style=for-the-badge&logo=typescript&logoColor=white" alt="TypeScript" />
<img src="https://img.shields.io/badge/JavaScript-F7DF1E?style=for-the-badge&logo=javascript&logoColor=323330" alt="JavaScript" />
<img src="https://img.shields.io/badge/Iolo-000000?style=for-the-badge&logo=iolo&logoColor=white" alt="Iolo" />
<img src="https://img.shields.io/badge/Roboflow-FF6F00?style=for-the-badge&logo=roboflow&logoColor=white" alt="Roboflow" />
<img src="https://img.shields.io/badge/Figma-F24E1E?style=for-the-badge&logo=figma&logoColor=white" alt="Figma" />
<img src="https://img.shields.io/badge/GitHub-181717?style=for-the-badge&logo=github&logoColor=white" alt="GitHub" />
<img src="https://img.shields.io/badge/Slack-4A154B?style=for-the-badge&logo=slack&logoColor=white" alt="Slack" />
<img src="https://img.shields.io/badge/Discord-5865F2?style=for-the-badge&logo=discord&logoColor=white" alt="Discord" />
<img src="https://img.shields.io/badge/Visual%20Studio%20Code-0078d7?style=for-the-badge&logo=visual-studio-code&logoColor=white" alt="VSCode" />

→ [Voltar ao topo](#topo)

<span id="equipe">

# :busts_in_silhouette: Equipe

|    Função     | Nome                           |                                                                                                                                                      LinkedIn & GitHub                                                                                                                                                      |
| :-----------: | :----------------------------- | :-------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------: |
|   Product Owner    | Thiago Frederico da Silva Zani |         [![Linkedin Badge](https://img.shields.io/badge/Linkedin-blue?style=flat-square&logo=Linkedin&logoColor=white)](https://www.linkedin.com/in/thiago-zani-1b8503249/) [![GitHub Badge](https://img.shields.io/badge/GitHub-111217?style=flat-square&logo=github&logoColor=white)](https://github.com/zani19)          |             
| Scrum Master | Jean Lucas de Faria Silva      |         [![Linkedin Badge](https://img.shields.io/badge/Linkedin-blue?style=flat-square&logo=Linkedin&logoColor=white)](https://www.linkedin.com/in/jeanlfs/) [![GitHub Badge](https://img.shields.io/badge/GitHub-111217?style=flat-square&logo=github&logoColor=white)](https://github.com/jeejinf)          |             
|   Dev Team    | Gabriel Brosig Briscese        |   [![Linkedin Badge](https://img.shields.io/badge/Linkedin-blue?style=flat-square&logo=Linkedin&logoColor=white)](https://www.linkedin.com/in/gabriel-brosig-briscese-344a5587/) [![GitHub Badge](https://img.shields.io/badge/GitHub-111217?style=flat-square&logo=github&logoColor=white)](https://github.com/Briscese)   |
|   Dev Team    | Jonas Rafael Siqueira Ribeiro      |                 [![Linkedin Badge](https://img.shields.io/badge/Linkedin-blue?style=flat-square&logo=Linkedin&logoColor=white)](https://www.linkedin.com/in/jonasrsribeiro/) [![GitHub Badge](https://img.shields.io/badge/GitHub-111217?style=flat-square&logo=github&logoColor=white)](https://github.com/jonasrsribeiro)         |
|   Dev Team    | Jonatas Mathias Dalló     |         [![Linkedin Badge](https://img.shields.io/badge/Linkedin-blue?style=flat-square&logo=Linkedin&logoColor=white)](https://www.linkedin.com/in/jonatas-mathias-147638206) [![GitHub Badge](https://img.shields.io/badge/GitHub-111217?style=flat-square&logo=github&logoColor=white)](https://github.com/Jonatas-Dallo)          |
|   Dev Team    | Miguel Carvalho Soares     |         [![Linkedin Badge](https://img.shields.io/badge/Linkedin-blue?style=flat-square&logo=Linkedin&logoColor=white)](https://www.linkedin.com/in/miguel-carvalho-soares-722b161a3/) [![GitHub Badge](https://img.shields.io/badge/GitHub-111217?style=flat-square&logo=github&logoColor=white)](https://github.com/Miguel-C1)          |

→ [Voltar ao topo](#topo)

<span id="links">

# :link: Links úteis

- [Repositório Frontend](https://github.com/jeejdev/frontend-nocloud)

- [Repositórios Backend:]()
  - [Cadastro-Autenticação](https://github.com/jeejdev/controller-cadastro-autenticacao-nocloud)
  - [Identificação IA](https://github.com/jeejdev/controller-identificacao-ia-nocloud)

- [Repositório Banco de Dados](https://github.com/jeejdev/controller-firebase-nocloud)

- [Fatec "Profº Jessen Vidal" SJCampos](https://fatecsjc-prd.azurewebsites.net/)

- [Visiona Tecnologia Espacial](https://visionaespacial.com/empresa/)

   <br>

  → [Voltar ao topo](#topo)
