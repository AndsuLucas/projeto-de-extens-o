
> A descrição técnica e plano de ação não se difere tanto de projeto para projeto. 


> O que mais muda de projeto para projeto: nome, descrição funcional e objetivo.

## Proposta 1

### Nome do projeto

- **"ScreenCare"**

### Descrição geral e objetivo de projeto

- Cadastro de clientes: Registro e gerenciamento das informações dos clientes para fácil acesso.
- Registro de ordens de serviço: Criação e acompanhamento de ordens de serviço de maneira eficiente.
- Edição e atualização de ordens: Permite modificar detalhes das ordens conforme necessário.
- Acesso rápido a contatos: Organização e acesso imediato a informações de contato dos clientes.
- Gerenciamento de notificações: O sistema notificará os clientes sobre o andamento de seus serviços em tempo real.
- Relatórios e análise de desempenho: Visão geral das ordens finalizadas, pendentes e métricas de eficiência.
### Descrição funcional do projeto

O intuito é facilitar que profissionais da área realizem tarefas de gerenciamento de ordens de serviço de maneira automatizadas. Tarefas essas que muitas vezes são manuais e tomam um tempo acima do desnecessário. Através do sistema o profissional poderá realizar cadastro de clientes, registro de ordem de serviços, edições, rápido acesso a fontes de contato e também um gerenciamento de notificações que informará ao cliente o andamento atual de determinado serviço. Além de outras features.

### Modelo de Negócio:
🔹 **SaaS Freemium:** Plataforma básica gratuita, com versão premium para personalização avançada (como integração com WhatsApp, relatórios mais detalhados e maior volume de notificações).  
🔹 **Suporte e Consultoria:** Empresas podem pagar para implementação personalizada e suporte técnico.  
🔹 **Treinamentos:** Venda de cursos e certificações para empresas que utilizam a plataforma.  
🔹 **Parcerias com Provedores de Hospedagem:** Empresas que oferecem servidores podem patrocinar o projeto para ganhar visibilidade.

### Descrição técnica

O uso de bibliotecas proprietárias será evitado. Serão utilizadas de maneira reduzida apenas bibliotecas open source que tem seu código aberto. Não será utilizado nenhum framework, apenas bibliotecas que serão adicionadas sob demanda conforme a necessidade do projeto. O intuito dessa decisão, é favorecer a reutilização das bibliotecas e componentes do sistema para a comunidade de desenvolvimento opensource. Isto será feito de forma não restritiva, visando a liberdade de futuros atuantes integrarem com os frameworks ou tecnologias proprietárias de sua preferência.
Será desenvolvido em plataforma web inicialmente. Com suporte para desktop e mobile, a princípio apenas através de acesso via url. 

Será utilizada uma base de dados relacional, como por exemplo **Mysql** para armazenamento das informações necessárias. Também, para agilizar determinados tipos de busca e acesso, será utilizado um banco de dados em memória não relacional, tal como o **Redis**.

Para desenvolvimento backend, irá ser utilizado o **PHP** por ser uma linguagem amplamente utilizada no backend da web, ter seu custo de infraestrutura relativamente menor se comparado com outras linguagens. Além de favorecer um ecossistema rico de servidores "plug and play" para esta linguagem.

Como tecnologia front-end, será utilizado html, css  e javascript.

Será necessário a integração com diferentes tipos de tecnologias de notificação. Inicialmente tem-se a ideia de criar apenas notficações por e-mail, como por exemplo, caso o produto já esteja pronto ou caso algum tipo de contratempo aconteça. Para isso, inicialmente iremos utilizar o **MailTrap** para o desenvolvimento, e será necessário o estudo de servidores de e-mail disponíveis no mercado para a implantação do projeto.

Será utilizado caso necessário um serviço de mensageria ou stream, tal como o **RabbitMQ** ou **Kafka**.

O projeto será armazenado no github e terá uma pipeline de CI/CD.

A infraestrutura e local de deploy terá que ser estudada. Procurando opções gratuitas no mercado para projetos opensource sem fins lucrativos.

Para o desenvolvimento, será utilizada uma estrutura docker com docker-compose. Com o intuito de diminuir o atrito do desenvolvimento em diferentes sistemas e computadores. Visto que a premissa é disponibilizar o projeto para contribuições.
## Plano de ação inicial
- Provisionar o(s) repositórios para o código fonte do projeto. Bem como suas documentações técnicas;
- Criar um repositório ou algum local de armazenamento para os artefatos e documentações do projeto a nível de negócios;
- Mapear principais funcionalidades do sistema e criar atividades para cada uma delas;
- Definir design system do projeto;
- Definir setup inicial para o desenvolvimento;
- Definir "esteira" de **CI/CD**
- Iniciar o desenvolvimento das principais atividades, para ter um MVP mais rápido possível;
- Iniciar a pesquisa de um servidor gratuito ou com custo reduzido para projetos sem fins lucrativos;
- Com o MVP pronto e a plataforma de deploy estabelecida, realizar a implantação em produção para que seja possível a utilização do projeto;
- Revisar o andamento das features, verificar possíveis pontos de melhoria e seguir com as funcionalidades "secundárias".
### Observação

> O produto final será gratuito. Totalmente disponibilizado na web junto com seu código fonte.
> Inicialmente será privado, mas após a implantação, será disponibilizado gratuitamente em sua versão básica.

### Privacidade
 - **Totalmente privado** até a implantação do projeto/disponibilização do código fonte. Não autorizo, nem com a minha presença, a divulgação 
### Equipe proposta

- Anderson Lucas Silva de oliveira.
## Proposta 2

### Nome do projeto

**EduSync: AI-Powered Study Planner**

### Descrição geral e objetivo do projeto

EduSync é uma plataforma inteligente para planejamento de estudos, permitindo que estudantes otimizem seu tempo e organizem suas rotinas de aprendizado de forma eficaz. O objetivo principal é oferecer um sistema que analisa a disponibilidade e metas do usuário para gerar um cronograma de estudos personalizado, ajudando a manter a produtividade e o foco.

### Descrição funcional do projeto

- **Criação de planejamento personalizado:** O usuário insere suas matérias, prazos e disponibilidade, e o sistema gera um cronograma otimizado.
    
- **Sistema de lembretes e notificações:** Alertas para manter o estudante no ritmo e evitar procrastinação.

- **Relatórios de progresso:** Gráficos e estatísticas para acompanhar a evolução do aprendizado.
    
- **Integração com flashcards e materiais de estudo:** Possibilidade de adicionar recursos interativos para reforçar o aprendizado.
    
- **Comunidade de estudos:** Opção para formar grupos de estudo e compartilhar metas e progresso.

### Modelo de Negócio

🔹 **Assinatura Premium (Freemium):** O core do sistema é gratuito, mas recursos avançados (ex: inteligência artificial para otimização de cronogramas, integração com Google Calendar, relatórios avançados) são pagos.  
🔹 **Publicidade:** Parceria com edtechs e empresas de cursos para exibição de anúncios relevantes.  
🔹 **Parcerias com Instituições de Ensino:** Universidades e escolas podem pagar para customizar e integrar a plataforma para seus alunos.  
🔹 **Doações e Crowdfunding:** Incentivo à contribuição de usuários via **OpenCollective, GitHub Sponsors, Patreon**.

### Descrição técnica 

O uso de bibliotecas proprietárias será evitado. Serão utilizadas de maneira reduzida apenas bibliotecas open source que tem seu código aberto. Não será utilizado nenhum framework, apenas bibliotecas que serão adicionadas sob demanda conforme a necessidade do projeto. O intuito dessa decisão, é favorecer a reutilização das bibliotecas e componentes do sistema para a comunidade de desenvolvimento opensource. Isto será feito de forma não restritiva, visando a liberdade de futuros atuantes integrarem com os frameworks ou tecnologias proprietárias de sua preferência.
Será desenvolvido em plataforma web inicialmente. Com suporte para desktop e mobile, a princípio apenas através de acesso via url. 

Será utilizada uma base de dados relacional, como por exemplo **Mysql** para armazenamento das informações necessárias. Também, para agilizar determinados tipos de busca e acesso, será utilizado um banco de dados em memória não relacional, tal como o **Redis**.

Para desenvolvimento backend, irá ser utilizado o **PHP** por ser uma linguagem amplamente utilizada no backend da web, ter seu custo de infraestrutura relativamente menor se comparado com outras linguagens. Além de favorecer um ecossistema rico de servidores "plug and play" para esta linguagem.

Como tecnologia front-end, será utilizado html, css  e javascript.

Será necessário a integração com diferentes tipos de tecnologias de notificação. Mas para esse domínio especifico, é essencial o uso de notificações mobile com a utilização de algum mecanismo de agendamento.

Será utilizado, caso necessário um, serviço de mensageria ou stream, tal como o **RabbitMQ** ou **Kafka**.

O projeto será armazenado no github e terá uma pipeline de CI/CD.

A infraestrutura e local de deploy terá que ser estudada. Procurando opções gratuitas no mercado para projetos opensource sem fins lucrativos.

Para o desenvolvimento, será utilizada uma estrutura docker com docker-compose. Com o intuito de diminuir o atrito do desenvolvimento em diferentes sistemas e computadores. Visto que a premissa é disponibilizar o projeto para contribuições.
## Plano de ação inicial
- Provisionar o(s) repositórios para o código fonte do projeto. Bem como suas documentações técnicas;
- Criar um repositório ou algum local de armazenamento para os artefatos e documentações do projeto a nível de negócios;
- Mapear principais funcionalidades do sistema e criar atividades para cada uma delas;
- Definir design system do projeto;
- Definir setup inicial para o desenvolvimento;
- Definir "esteira" de **CI/CD**
- Iniciar o desenvolvimento das principais atividades, para ter um MVP mais rápido possível;
- Iniciar a pesquisa de um servidor gratuito ou com custo reduzido para projetos sem fins lucrativos;
- Com o MVP pronto e a plataforma de deploy estabelecida, realizar a implantação em produção para que seja possível a utilização do projeto;
- Revisar o andamento das features, verificar possíveis pontos de melhoria e seguir com as funcionalidades "secundárias".

### Observação

> O produto final será gratuito. Totalmente disponibilizado na web junto com seu código fonte.
> Inicialmente será privado, mas após a implantação, será disponibilizado gratuitamente.

### Privacidade
 - **Totalmente privado** até a implantação do projeto/disponibilização do código fonte. Não autorizo, nem com a minha presença, a divulgação 
### Equipe proposta

- Anderson Lucas Silva de oliveira.
 


## Proposta 3

### Nome do projeto

**FinWise**

### Descrição geral e objetivo do projeto

FinWise é uma plataforma de gerenciamento financeiro pessoal que ajuda os usuários a monitorar suas despesas, criar orçamentos e atingir metas financeiras. O objetivo é tornar o planejamento financeiro mais acessível e eficiente por meio de inteligência artificial, fornecendo insights personalizados e automatizando processos para uma melhor organização das finanças pessoais.

### Descrição funcional do projeto

- **Rastreamento automático de despesas:** O usuário pode inserir manualmente ou conectar contas bancárias (onde permitido) para registrar gastos automaticamente.
    
- **Sugestões de economia:** O sistema analisa padrões de gastos e sugere formas de economizar dinheiro.
    
- **Definição e acompanhamento de metas financeiras:** Usuários podem criar metas como "economizar para uma viagem" e acompanhar o progresso.
    
- **Relatórios e insights financeiros:** Gráficos interativos e análises detalhadas sobre os hábitos financeiros do usuário.
    
- **Geração de relatórios para impostos:** Facilidade para freelancers e autônomos gerarem relatórios financeiros.
    
- **Modo de orçamento planejado:** Permite definir um orçamento mensal e monitorar se os gastos estão dentro do planejado.
    

---
### Descrição técnica 

O uso de bibliotecas proprietárias será evitado. Serão utilizadas de maneira reduzida apenas bibliotecas open source que tem seu código aberto. Não será utilizado nenhum framework, apenas bibliotecas que serão adicionadas sob demanda conforme a necessidade do projeto. O intuito dessa decisão, é favorecer a reutilização das bibliotecas e componentes do sistema para a comunidade de desenvolvimento opensource. Isto será feito de forma não restritiva, visando a liberdade de futuros atuantes integrarem com os frameworks ou tecnologias proprietárias de sua preferência.
Será desenvolvido em plataforma web inicialmente. Com suporte para desktop e mobile, a princípio apenas através de acesso via url. 

Será utilizada uma base de dados relacional, como por exemplo **Mysql** para armazenamento das informações necessárias. Também, para agilizar determinados tipos de busca e acesso, será utilizado um banco de dados em memória não relacional, tal como o **Redis**.

Para desenvolvimento backend, irá ser utilizado o **PHP** por ser uma linguagem amplamente utilizada no backend da web, ter seu custo de infraestrutura relativamente menor se comparado com outras linguagens. Além de favorecer um ecossistema rico de servidores "plug and play" para esta linguagem.

Como tecnologia front-end, será utilizado html, css  e javascript.

Será utilizado caso necessário um serviço de mensageria ou stream, tal como o **RabbitMQ** ou **Kafka**.

O projeto será armazenado no github e terá uma pipeline de CI/CD.

A infraestrutura e local de deploy terá que ser estudada. Procurando opções gratuitas no mercado para projetos opensource sem fins lucrativos.

Para o desenvolvimento, será utilizada uma estrutura docker com docker-compose. Com o intuito de diminuir o atrito do desenvolvimento em diferentes sistemas e computadores. Visto que a premissa é disponibilizar o projeto para contribuições.

### Modelo de Negócio

🔹 **Licenciamento Dual:** O código é aberto, mas empresas podem pagar por uma versão corporativa com suporte.  
🔹 **API Monetizada:** Empresas de fintechs podem pagar pelo acesso à API do FinWise para integração com seus serviços.  
🔹 **Assinatura Premium (Freemium):** Funções básicas são gratuitas, enquanto funcionalidades avançadas (ex: sincronização bancária automática, relatórios de impostos) são pagas.  
🔹 **Treinamento e Certificações:** Cursos sobre planejamento financeiro e uso avançado da plataforma.
## Plano de ação inicial
- Provisionar o(s) repositórios para o código fonte do projeto. Bem como suas documentações técnicas;
- Criar um repositório ou algum local de armazenamento para os artefatos e documentações do projeto a nível de negócios;
- Mapear principais funcionalidades do sistema e criar atividades para cada uma delas;
- Definir design system do projeto;
- Definir setup inicial para o desenvolvimento;
- Definir "esteira" de **CI/CD**
- Iniciar o desenvolvimento das principais atividades, para ter um MVP mais rápido possível;
- Iniciar a pesquisa de um servidor gratuito ou com custo reduzido para projetos sem fins lucrativos;
- Com o MVP pronto e a plataforma de deploy estabelecida, realizar a implantação em produção para que seja possível a utilização do projeto;
- Revisar o andamento das features, verificar possíveis pontos de melhoria e seguir com as funcionalidades "secundárias".
### Observação

> O produto final será gratuito. Totalmente disponibilizado na web junto com seu código fonte.
> Inicialmente será privado, mas após a implantação, será disponibilizado gratuitamente.

### Privacidade
 - **Totalmente privado** até a implantação do projeto/disponibilização do código fonte. Não autorizo, nem com a minha presença, a divulgação 
### Equipe proposta

- Anderson Lucas Silva de oliveira.