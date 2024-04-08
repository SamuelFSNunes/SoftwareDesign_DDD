# SoftwareDesign_DDD
![image](https://github.com/SamuelFSNunes/SoftwareDesign_DDD/assets/123522471/58d44945-c111-491d-a629-a8b626ef6c73)

### O que é?
Antigamente no desenvolvimento de softwares muitos projetos eram **orientados a tecnologia**, e comunicação entre especialista de negócios e os desenvolvedores, o que resultava em muitos erros ou mal-entendidos criando muitos erros ou sistema não escaláveis.Para solucionar essa dor nasceu o modelo **DDD (Domain Driven Domain)**. Ou seja, o conceito surgiu para **alinhar o software às complexas regras de negócios**.

Sendo assim, DDD é uma abordagem de desenvolvimento de software que coloca o foco primordial no entendimento profundo do domínio de negócios. Ao invés de começar pelo código ou pela tecnologia, prioriza-se a compreensão das regras, processos e conceitos da empresa que a aplicação está destinada a atender.


### Quem o criou?
O conceito começou a ser desenvolvido na década de 1960 e o surgimento das linguagens orientadas ao objeto faz parte dessa evolução. No entanto, o principal marco da abordagem é a publicação do livro Domain-Driven Design: Tackling Complexity in the Heart of Software de Eric Evans, em 2003, que formalizou a abordagem de forma coesa e sistemática. 

### Como o DDD trabalha?
Esse modelo de domínio é expresso por meio de uma linguagem ubíqua, ou seja, uma linguagem comum compreendida tanto por especialistas do domínio quanto por desenvolvedores. O DDD também aborda a arquitetura do software, enfatizando a divisão em camadas que refletem a complexidade do domínio e a separação de responsabilidades. 

## Building Blocks
![image](https://github.com/SamuelFSNunes/SoftwareDesign_DDD/assets/123522471/f6b17034-99d8-4f0a-a2f6-fa0bff292ff6)

Conjunto de conceitos e padrões que auxiliam na modelagem orientado pelo domínio

- ### Entidades
As entidades são objetos que contêm identidade própria e podem mudar ao longo do tempo, mas são distintos pela sua identidade, não apenas pelos seus atributos. **Elas representam elementos centrais e significativos do domínio.** Exemplos de entidades incluem cliente, um pedido ou uma conta bancária. 

- ### Objetos de valor
Diferente das entidades, os objetos de valor são elementos imutáveis que não apresentam identidade própria, mas são definidos pelos seus atributos. **Eles representam conceitos que são importantes no domínio, mas não têm uma existência distinta**, como datas, moedas ou coordenadas geográficas. 

- ### Agregados 
Os agregados são **conjuntos de entidades e objetos de valor que são tratados como uma única unidade coesa**. Cada agregado tem uma raiz, que é a única entrada para acessar ou manipular o agregado como um todo, o que ajuda a manter a consistência e a integridade do domínio. 

- ### Repositórios 
Os repositórios são responsáveis pela persistência e recuperação de entidades. **Eles oferecem uma abstração que permite ao código de domínio trabalhar com objetos do domínio**, sem se preocupar com os detalhes de armazenamento e recuperação. Utilizado principalmente para administrar regras de negócio.

- ### Serviços de domínio 
Os serviços de domínio encapsulam lógica de negócios que não se encaixa facilmente nas entidades ou agregados. **Eles são responsáveis por operações que envolvem múltiplos elementos do domínio** ou que não são diretamente associados a um único objeto. 

- ### Eventos de domínio 
Os eventos de domínio representam acontecimentos importantes que ocorrem no domínio e que podem ter impacto em diferentes partes do sistema.** Eles permitem uma comunicação assíncrona entre diferentes componentes do sistema.**

- ### Bounded context 
A divisão do sistema em contextos delimitados (bounded context) mantém a clareza e a separação de responsabilidades. **Ela reconhece que determinados termos e regras de negócios podem ter significados diferentes em partes distintas de um sistema.** Cada contexto delimitado conta com seu próprio modelo de domínio e linguagem ubíqua, evitando conflitos e ambiguidades. 

# Quando usar Domain-Driven Design? 
![image](https://github.com/SamuelFSNunes/SoftwareDesign_DDD/assets/123522471/774ee1ee-0aaf-40b2-ba83-2d9e7fe21139)

Essa é uma abordagem poderosa, mas não é uma solução universal para todos os projetos de software. A decisão de usar ou não o DDD depende de vários fatores, incluindo a complexidade do domínio, a equipe, os requisitos do projeto e o contexto em que o projeto está inserido. 

A estratégia é mais benéfica em projetos complexos, em que as regras de negócios são intrincadas e suscetíveis a mudanças. Em projetos mais simples, seu overhead pode superar os benefícios. Contudo, mesmo em contextos menos complexos, os princípios do DDD, como a criação de uma linguagem ubíqua, podem ser úteis para melhorar a comunicação. 

O DDD brilha em projetos de sistemas financeiros, saúde, logística, projetos de e-commerce e aplicações de Customer Relationship Management (CRM) e Enterprise Resource Planning (ERP), nas quais os requisitos de negócios são substanciais e estão sujeitos a mudanças frequentes. Além disso, a abordagem também é útil na integração de sistemas legados e no desenvolvimento de plataformas e frameworks. 
