# 🍄 Resposta da Ponderada 🍄

## 1️⃣ Pesquisa Referenciado: 
[**Methodology for the Development and Deployment of a Hospital Management
Information System using Free Open Source Software**](https://d1wqtxts1xzle7.cloudfront.net/76297394/ICOSST__3_1-libre.pdf?1639506953=&response-content-disposition=inline%3B+filename%3DMethodology_for_the_Development_and_Depl.pdf&Expires=1725556723&Signature=BqdycaZ7wyWHSGUp0BTm21Dkx4pyTCaukDdtWZS~SaA~G0PNXLKCl2kAeq2GkD5FGfVWA-CiOKLwhZrmewOfNqULh3HrRAtm3y2dxgAxObz69okCJHJT4QkWaujP2iKJVkU1~nKfJ8oPfTinkF8qNXFT1hHCeSa65KX7LEyG~X1Sg68Pj6AAvW~79Qdy2z~FqxYUmLn2H2HM4p0TzPFWzBcTDF5y7nlZE-JGlO-uBfXu7WhM5mP0L5ZOOEFlQSS7mzjpe9dwTPgqmX-hxF3GQBdKcHN-khBd2TXQWqnSTmNtAR8TKDdjcEwma8p01HI37SaPQ1EASMN905zVZhvRJw__&Key-Pair-Id=APKAJLOHF5GGSLRBV4ZA)

Este plano de cutover foi criado para o projeto **Implementação do Sistema de Gestão Hospitalar**, que teve como objetivo a implantação de um sistema de gerenciamento hospitalar utilizando software livre e de código aberto. Este projeto visava modernizar e otimizar a gestão hospitalar, melhorando o operacional e a qualidade dos serviços prestados. A transição abordada envolve a substituição de processos manuais e sistemas legados por uma solução centralizada, com o intuito de aperfeiçoar a precisão dos registros médicos, facilitar a comunicação entre as equipes de saúde e elevar a qualidade dos serviços prestados aos pacientes. Interessante observar como tudo isso foi feito mantendo o hospital funcionando.

O plano de cutover, abordado na seção 7 do paper, foca em uma transição suave, minimizando riscos associados à interrupção do serviço hospitalar, ao mesmo tempo em que assegura que todos os dados críticos sejam migrados e que o novo sistema esteja completamente funcional para uso imediato e seguro.

## Aspectos principais do projeto

Dentro do paper, analisei os seguintes principais aspectos envolvendo essa alteração de gestão com um sistema de gestão hospitalar livre:

- Existia uma redução de interrupções. Tinham que garantir que o impacto nas operações diárias seria o mínimo, com a migração ocorrendo fora dos horários de pico ou em fases progressivas, para que as atividades hospitalares continuassem de forma ininterrupta.
- Foi dado suporte contínuo na transição. Durante e após o cutover, uma equipe de TI dedicada estava disponível para resolver rapidamente quaisquer problemas técnicos, algo semelhante ao que a G2 está fazendo conosco neste projeto da turma de Sistemas de Informação.
- Notável a preocupação com o treinamento dos envolvidos. Todo o pessoal envolvido nas operações hospitalares foi previamente treinado no uso do novo sistema, reduzindo erros operacionais durante a transição. Isso é algo crucial, pensando que as pessoas já estavam acostumadas com outro padrão de funcionamento do hospital.

## 2️⃣ Principais Elementos do Plano de Cutover:

Os principais elementos identificados no plano de cutover são:

- **Preparação de Sistemas:** Detalha como os sistemas serão preparados antes do cutover.
- **Treinamento de Usuários:** Como já analisado, foi realizado o treinamento para garantir que os usuários estivessem prontos.
- **Plano de Contingência:** Para resolver os problemas que podem aparecer com os testes do sistema, é necessário ter um plano que dê uma direção sobre como resolvê-los, pelo menos para aqueles que estão dentro da capacidade de previsão.
- **Execução do Cutover:** Definiu-se o cronograma exato de atividades durante a transição. Senti falta de um melhor detalhamento e documentação disso no paper.
- **Validação Pós-Cutover:** Após a aplicação, realizaram a verificação do sucesso da transição na execução do cutover.

Agora, abordando cada um dos planos de forma mais detalhada sobre o que se espera deles e como foi tratado no paper analisado:

### Preparação de Sistemas:
A preparação dos sistemas garante uma transição sem falhas. O backup completo dos dados é necessário para possibilitar a restauração em caso de erro. No artigo, a migração utilizou três arquivos CSV para transferir dados, com a migração de dados dinâmicos adiada até o final da execução paralela, enfatizando a importância de planejar migrações flexíveis para sistemas que lidam com dados em constante mudança, como prontuários médicos e informações financeiras.

### Treinamento de Usuários:
O paper menciona que o plano inclui sessões de treinamento e simulações, garantindo que todos os usuários estejam preparados. O artigo foca na migração de dados e menciona uma pequena equipe interna que, provavelmente, teve que aprender rapidamente o novo sistema, sem um processo formal de treinamento.

### Planos de Contingência:
Acredito que um plano de contingência inclui procedimentos de reversão e suporte 24 horas. Todavia, o artigo aborda a execução paralela como forma de mitigar riscos, sem focar tanto em contingências imediatas.

### Execução do Cutover:
A execução requer um cronograma bem definido e o congelamento de atualizações no sistema anterior para proteger a integridade dos dados. No artigo, o corte foi planejado com base no congelamento do banco de dados anterior. Contudo, observei pontos de melhoria no detalhamento desse processo no artigo.

### Validação Pós-Cutover:
No artigo, a validação dos dados dinâmicos foi priorizada após a migração. Penso que o plano deveria expandir essa etapa, incluindo a validação pelos usuários e testes das funções críticas, assegurando uma transição mais completa.

## 3️⃣ Pontos Positivos e Negativos:

### Pontos Positivos 🌟
- **Preparação Estruturada:** A separação entre dados dinâmicos e estáticos, além de uma execução faseada com um parallel run, reduziu os riscos de interrupção operacional.
- **Paralelo com Ambiente de Testes:** O uso de uma base de dados de testes durante o parallel run evitou impactos diretos nas operações durante a fase de migração.
- **Equipe Dedicada e Flexível:** Mesmo com uma equipe pequena, a flexibilidade permitiu resolver problemas rapidamente. Achei impressionante, já que o ambiente hospitalar é crítico.

### Pontos Negativos ⚠️
- **Falta de Documentação Formal:** A ausência de uma documentação mais detalhada dos requisitos do usuário e de um plano formal de QA criou vulnerabilidades. Com tempo curto e da forma como foi organizado, estavam sujeitos a retrabalho e riscos de defeitos não descobertos antes da produção.
- **Dependência de Desenvolvedores:** A execução dos testes pelos próprios desenvolvedores pode ter comprometido a qualidade da validação, já que a perspectiva de um testador externo independente não foi considerada.

## 4️⃣ Recomendações de Melhoria:

Para fortalecer o processo de cutover e evitar os problemas enfrentados, proponho as seguintes recomendações:

- **Matriz RACI:** Definir claramente quem são os responsáveis (Responsável, Aprovador, Consultado e Informado) para cada etapa do processo de cutover.
- **Documentação de Versionamento:** Manter um controle rigoroso das atualizações no documento do plano, com registros de quem atualizou e quando.
- **Melhoria na Documentação de Requisitos:** Criar uma lista de requisitos numerada e validada pelos usuários para evitar retrabalhos e garantir que as funcionalidades menos frequentes não sejam esquecidas.
- **Passagem de Conhecimento:** Garantir que a equipe que vai assumir a sustentação do sistema receba todo o conhecimento necessário através de treinamento e documentação, que, aparentemente, parece incompleta sem acesso a outros documentos.



---

✨ *Essa foi a minha análise hihiii! Espero que tenha sido dentro-acima do esperado.* ✨

**Obs**: para documentar, utilizei o Chat GPT para obter um templete de registro sobre a atividade. 

--- 

![duo-querido](https://i.pinimg.com/736x/d0/9d/6a/d09d6a92d3a494dfffc51d946d376e4b.jpg)


