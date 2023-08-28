# Processo de Desenvolvimento

## Índice
1. [Refinamento](#1-refinamento)
    - 1.1. Análise detalhada dos requisitos
    - 1.2. Criando experiências intuitivas
2. [Design de Interface](#2-design-de-interface)
    - 2.1. Prototipagem de interfaces
    - 2.2. Escolha de estilos e elementos de design
3. [Desenvolvimento](#3-desenvolvimento)
    - 3.1. Configurando seu Ambiente de Desenvolvimento
    - 3.2. Configurando sua Branch de Desenvolvimento
    - 3.3. Escolhas de Tecnologias Front-end
    - 3.4. Implementação de Funcionalidades
4. [Testes](#4-testes)
    - 4.1. Testes Unitários
    - 4.2. Testes de integração
    - 4.3. Testes de usabilidade
5. [Otimização](#5-otimização)
    - 5.1 Análise de Desempenho
    - 5.2. Otimização de Código e Recursos



## 1. Refinamento

A fase de refinamento é fundamental para aprimorar e detalhar os requisitos iniciais, garantindo que o desenvolvimento do front-end atenda às expectativas do projeto.

### 1.1 Análise Detalhada dos Requisitos
- **Detalhamento dos Requisitos:**  
Refine os requisitos iniciais, tornando-os mais específicos e detalhados. Isso inclui a definição de funcionalidades específicas, comportamentos esperados e critérios de aceitação.
- **Identificação de Prioridades:**  
 Estabeleça prioridades para os requisitos, determinando quais funcionalidades são essenciais e quais são opcionais.


### 1.2 Definição de metas e objetivos

- **Defina Metas Claras:**  
Estabeleça metas de tempo realistas para o desenvolvimento, levando em consideração os prazos do projeto. Considere a complexidade das tarefas, recursos disponíveis e quaisquer eventos ou marcos importantes.

- **Identificação de Restrições de Prazo:**   
Avalie quaisquer restrições de prazo críticas, como lançamentos sazonais, datas de eventos (treinamentos, feriados) e impedimentos.

<br>
A fase de refinamento é crucial para evitar ambiguidades, retrabalho e garantir que o desenvolvimento front-end siga uma direção clara e alinhada com as necessidades do projeto. E é essencial para garantir que o projeto seja concluído dentro do prazo. Isso estabelece uma base sólida para o desenvolvimento subsequente.


## 2. Design de Interface

O design de interface é uma etapa crucial para criar uma experiência de usuário atraente e eficaz.

### 2.1 Prototipagem de Interfaces

- **Crie Protótipos:** Protótipos ou wireframes serão criados para representar visualmente as páginas e componentes de interface do usuário. Isso ajudará os desenvolvedores a visualizar o como deverá ser o layout, a estrutura de navegação e as interações. Como também manter consistência com as medidas usadas de largura, altura, espaçamento, etc. já definidas pelo UI designer.

- **Teste com Usuários:** Realize testes de usabilidade com protótipos para coletar feedback dos usuários e identificar possíveis melhorias.


### 2.2 Escolha de Estilos e Elementos de Design

- **Defina Estilos Visuais:** Escolha esquemas de cores, tipografia e elementos de design que representem a identidade visual do projeto.

- **Padronização de Elementos e Design System:** Estabeleça diretrizes para o uso consistente de botões, ícones, formulários e outros elementos de interface em todo o projeto.

   >**IMPORTANTE**  
    >*A Valecard já conta com um Design System criado com o objetivo de garantir um padrão e consistência entre seus produtos. **Todo design deverá ser baseado nele**.*<br>
>

O design de interface desempenha um papel fundamental na usabilidade e na estética do software, influenciando diretamente a experiência do usuário. A prototipagem ajuda a validar o design antes da implementação, economizando tempo e recursos. A escolha cuidadosa de estilos e elementos de design garante uma aparência coesa e profissional em todo o projeto.


## 3. Desenvolvimento

A fase de desenvolvimento é onde a implementação real da interface de usuário ocorre.

### 3.1 Configurando seu Ambiente de Desenvolvimento
- **Visual Studio Code (VSCode):**
Recomendamos o uso do Visual Studio Code como ambiente de desenvolvimento de front-end devido à sua popularidade, suporte extensivo à comunidade e recursos avançados para desenvolvimento web. Mas sinta-se livre para usar o editor/IDE de sua preferência.

- **Por que o VSCode?**
O VSCode oferece uma ampla gama de extensões, integração com Git, depuração integrada e uma interface amigável. É uma escolha sólida para aumentar a produtividade no desenvolvimento.

- **Extensões Recomendadas:**
A fim de facilitar seu desenvolvimento recomendamos as seguintes extensões para vc usar no seu VSCode:

    1. **Git Blame:** 
    Esta extensão permite visualizar as informações do Git Blame diretamente no VSCode, facilitando a rastreabilidade das alterações no código.
    2. **Auto Rename Tag:** 
    Simplifica a renomeação de tags HTML, garantindo que as tags de abertura e fechamento sejam atualizadas automaticamente.
    3. **Auto Close Tag:**
    Agiliza a escrita de código HTML, fechando automaticamente as tags HTML quando você insere a tag de abertura.

### 3.2 Configurando sua Branch de Desenvolvimento
- **Uso do Git Flow**: 
Adotamos o modelo GitFlow para gerenciar o versionamento do código. Isso envolve a criação de diferentes tipos de branches para organização e controle de versões.

- **Branch Base**: 
A criação de novas branches será baseada na "release-dev". Isso ajuda a manter a estabilidade da versão principal enquanto permite o desenvolvimento contínuo de novos recursos.
    >**DICA**  
    >*O que é GitFlow? Clique [aqui]() para ler o tutorial.*<br>
>


Essas configurações e práticas ajudarão a garantir um ambiente de desenvolvimento eficiente e organizado, além de promover uma colaboração mais eficaz em equipe.

### 3.3 Escolhas de Tecnologias Front-end
- **Angular:** 
Na Valecard é usado o framework Angular para desenvolvimento de aplicações front-end.

    >**IMPORTANTE**  
    >*Existe um repositório de um projeto boilerplate, no qual ja consta configurado todo seu design system padrão da empresa, configs de CI/CD, todos os módulos e bibliotecas externos essenciais para o desenvolvimento de uma aplicação. **Esse boilerplate deverá ser usado para  toda criação de projetos do zero.***<br>
>

- **Bibliotecas e módulos externos:** 
Com o objetivo de elevar o nível técnico de nossos desenvolvedores e deixar nosso produto o mais leve possível, a inclusão de novas bibliotecas e módulos externos (além daqueles previamente instalados no boilerplate) é extremamente proibida. É incentivado ao desenvolvedor criar sua funcionalidade do zero, pois assim teremos 100% do controle sobre essa funcionalidade. Caberá somente ao líder técnico a decisão se deverá ser incluso ou não um novo módulo ou biblioteca externa.

### 3.4. Implementação de Funcionalidades
- **Organização do Código:** Estruture o código de forma lógica e organizada, seguindo o padrão já existente no projeto, ou então, seguindo as melhores práticas de desenvolvimento. Como por exemplo a criação de componentes ou services reutilizáveis.

- **Desenvolvimento de Funcionalidades:** Implemente as funcionalidades conforme definido nos requisitos, seguindo os padrões de design e as diretrizes de usabilidade estabelecidas durante a fase de design.

A fase de desenvolvimento é onde a visão do projeto começa a se concretizar. A escolha das tecnologias certas, a estruturação adequada do código e a implementação das funcionalidades de acordo com os requisitos são cruciais para o sucesso do desenvolvimento front-end.


## 4. Testes
A fase de testes é essencial para garantir a qualidade e a confiabilidade do software front-end.

### 4.1 Testes Unitários
- **Karma+Jasmine ou Jest:** Em projetos Angular, os testes unitários são comumente realizados com o uso das engines de teste Karma e Jasmine, embora também seja possível optar por Jest como uma alternativa. Essas ferramentas permitem a criação de testes específicos para os componentes e serviços do Angular.

- **Arquivos .spec.ts:** Cada componente, serviço ou módulo deve ter um arquivo de teste associado com a extensão .spec.ts. Serão nesses arquivos onde será feita toda a escrita e especificação dos testes. Esses arquivos são reconhecidos automaticamente pelas ferramentas de teste.

- **Testes de Componentes:** Crie testes para verificar o comportamento e a funcionalidade de componentes individuais, como botões, formulários e outros elementos de interface.

- **Testes de Services:** Os services desempenham um papel fundamental em projetos Angular, muitas vezes encapsulando lógica de negócios ou chamadas a APIs. Portanto, é essencial realizar testes para verificar o comportamento e a funcionalidade dos serviços.

- **Testes de Mocks:** Para testar serviços que dependem de APIs externas ou recursos externos, é comum criar mocks (simulações) dos serviços ou recursos externos. Isso permite isolar o serviço e testar seu comportamento de forma controlada.

### 4.2 Testes de Integração
- **Integração de Componentes:** Realize testes de integração para verificar como os diferentes componentes interagem uns com os outros, garantindo que a interface funcione como um todo.

- **Testes de APIs:** Se o front-end se comunica com APIs, certifique-se de testar a integração com essas APIs para garantir a troca de dados adequada.

### 4.3 Testes de Usabilidade (e2e)

- **Testes de QA:** Integre a etapa de Qualidade de Software (QA) para realizar testes abrangentes que verifiquem a conformidade com os requisitos e padrões de qualidade estabelecidos. Realizando os eventuais ajustes que possam ocorrer.

- **Testes de Usuário:**
Realize testes de usabilidade com usuários reais para coletar feedback sobre a experiência de usuário, identificar problemas de usabilidade e melhorar a interface.

- **Testes de Acessibilidade:** Verifique a conformidade com as diretrizes de acessibilidade, como as WCAG, para garantir que o software seja acessível a todos os usuários.


A realização de testes rigorosos ajuda a identificar problemas de forma precoce e a assegurar que o produto ofereça uma experiência confiável, eficaz e agradável aos usuários.


## 5. Otimização
A otimização é uma etapa fundamental para garantir que a aplicação seja eficiente, rápida e responsiva.

### 5.1 Análise de Desempenho
- **Ferramentas de Análise:** Utilize ferramentas como o Google Lighthouse, PageSpeed Insights e WebPageTest para avaliar o desempenho do seu software em relação ao carregamento da página, tempo de resposta e outros indicadores-chave de desempenho.

- **Identificação de Pontos de Melhoria:** Analise os relatórios das ferramentas de análise para identificar áreas que precisam de melhorias. Isso pode incluir redução do tempo de carregamento, redução de requisições HTTP e melhoria na renderização.

### 5.2. Otimização de Código e Recursos
Minificação e Compactação: Minimize o tamanho do código JavaScript, CSS e HTML removendo espaços em branco, comentários e caracteres desnecessários. Além disso, compacte imagens e recursos para reduzir o tempo de carregamento.

- **Lazy Loading:** Implemente o carregamento tardio (lazy loading) de recursos, como imagens e scripts, para que eles sejam carregados apenas quando forem necessários, melhorando a velocidade de carregamento inicial.

- **Cache Eficiente:** Configure cabeçalhos de cache no servidor para permitir que o navegador armazene em cache recursos estáticos e os reutilize em visitas subsequentes.

- **Otimização de Imagens:** Utilize formatos de imagem otimizados, como WebP, e dimensione imagens conforme necessário para reduzir o tamanho do download.

- **Code Splitting:** Divida o código em módulos menores e carregue apenas o código necessário para cada página, reduzindo o tamanho inicial do carregamento.

- **Eliminação de Renderizações não Utilizadas:** Remova códigos e componentes não utilizados para reduzir a complexidade e o peso da aplicação.

A otimização é crucial para garantir que seu software front-end seja rápido e eficiente, proporcionando uma experiência de usuário suave e responsiva. A combinação de análise de desempenho, otimização de código e recursos contribui para um produto final de alta qualidade.



---
9. Requisitos Iniciais
   - 9.1. [Levantamento de requisitos do front-end](./desenvolvimento/requisitos/levantamento.md)
   - 9.2. [Definição de metas e objetivos](./desenvolvimento/requisitos/definicao-metas.md)
   
10. Design de Interface
    - 10.1. [Prototipagem de interfaces](./desenvolvimento/design/interface-prototipagem.md)
    - 10.2. [Escolha de estilos e elementos de design](./desenvolvimento/design/escolha-estilos.md)
    
11. Desenvolvimento
    - 11.1. [Escolha de tecnologias front-end](./desenvolvimento/desenvolvimento/escolha-tecnologias.md)
    - 11.2. [Estruturação do código](./desenvolvimento/desenvolvimento/estruturacao-codigo.md)
    - 11.3. [Implementação de funcionalidades](./desenvolvimento/desenvolvimento/implementacao-funcionalidades.md)
    
12. Testes
    - 12.1. [Testes de unidade](./desenvolvimento/testes/testes-unidade.md)
    - 12.2. [Testes de integração](./desenvolvimento/testes/testes-integracao.md)
    - 12.3. [Testes de usabilidade](./desenvolvimento/testes/testes-usabilidade.md)
    
13. Otimização
    - 13.1. [Análise de desempenho](./desenvolvimento/otimizacao/analise-desempenho.md)
    - 13.2. [Otimização de código e recursos](./desenvolvimento/otimizacao/otimizacao-codigo.md)
    
14. Acessibilidade e Testes Finais
    - 14.1. [Verificação de conformidade com padrões de acessibilidade](./desenvolvimento/acessibilidade/verificacao-conformidade.md)
    - 14.2. [Testes finais em diversos dispositivos e navegadores](./desenvolvimento/acessibilidade/testes-finais.md)

## Implantação
15. Preparação para Implantação
    - 15.1. [Configuração de servidores](./implantacao/preparacao/configuracao-servidores.md)
    - 15.2. [Preparação de ambientes](./implantacao/preparacao/preparacao-ambientes.md)
    
16. Implantação em Produção
    - 16.1. [Migração de código](./implantacao/producao/migracao-codigo.md)
    - 16.2. [Monitoramento pós-implantação](./implantacao/producao/monitoramento.md)

## Manutenção Contínua
17. Monitoramento de Desempenho
    - 17.1. [Acompanhamento da performance em produção](./manutencao/monitoramento/acompanhamento-performance.md)
    - 17.2. [Ajustes e otimizações contínuas](./manutencao/monitoramento/ajustes-otimizacoes.md)

18. Atualizações e Evoluções
    - 18.1. [Gerenciamento de mudanças](./manutencao/evolucoes/gerenciamento-mudancas.md)
    - 18.2. [Adaptação a novas necessidades do usuário](./manutencao/evolucoes/adaptacao-necessidades.md)



---

[Página anterior](../README.md)