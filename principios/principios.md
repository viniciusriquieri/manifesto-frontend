# Princípios

Nesta seção, apresentamos os princípios fundamentais que direcionam o desenvolvimento do nossa aplicação front-end. Ao segui-los, garantimos que nossos projetos sejam coesos, de alta qualidade e alinhados com as expectativas dos usuários.


## Índice
1. [Foco no Usuário](#1-foco-no-usuário)
   - 1.1. Entendendo as necessidades do usuário
   - 1.2. Criando experiências intuitivas
2. [Design Responsivo](#2-design-responsivo)
   - 2.1. Adaptação a diferentes dispositivos
   - 2.2. Garantindo uma experiência consistente
3. [Performance Otimizada](#3-performance-otimizada)
   - 3.1. Estratégias de otimização de desempenho
   - 3.2. Carregamento rápido de páginas
4. [Acessibilidade](#4-acessibilidade)
   - 4.1. Criando para todos os públicos
   - 4.2. Cumprindo os padrões de acessibilidade
5. [Manutenibilidade](#5-manutenibilidade)
   - 5.1. Organização do código
   - 5.2. Documentação e comentários


## 1. Foco no Usuário
O princípio fundamental do desenvolvimento front-end é manter um foco constante no usuário final. Isso significa entender profundamente as necessidades, expectativas e comportamentos dos usuários para criar experiências intuitivas e eficazes.


### 1.1. Entendendo as necessidades do usuário
Antes de iniciar qualquer projeto, é essencial conduzir analisar e entender as necessidades do usuário. Isso envolve:

- **Pesquisar no mercado soluções similares para identificar tendências e demandas, e usá-las como inspiração no seu desenvolvimento.**
- **Coletar feedback de usuários.**
- **Mapear jornadas do usuário para compreender como eles interagem com o sistema.**

Compreender as necessidades do usuário é o primeiro passo para criar uma interface que atenda às expectativas e resolva os problemas dos usuários.


### 1.2. Criando experiências intuitivas
Uma vez que as necessidades do usuário estejam bem definidas, o próximo passo é projetar uma interface que seja intuitiva de usar. Ou seja:

- **Desenvolver fluxos de usuário lógicos e intuitivos.**
- **Priorizar a consistência de design em toda a aplicação.**
- **Utilizar padrões de design reconhecíveis para elementos comuns, como menus e botões.**
- **Minimizar a sobrecarga de informações na interface.**

Uma experiência intuitiva reduz a curva de aprendizado para os usuários, tornando a interação com o software mais agradável e eficiente.


## 2. Design Responsivo
O princípio de design responsivo consiste em criar interfaces que se adaptem a uma variedade de dispositivos e tamanhos de tela, proporcionando uma experiência consistente e eficaz em todas as situações.

### 2.1. Adaptação a diferentes dispositivos
O design responsivo envolve a criação de interfaces que se ajustem automaticamente a diferentes tamanhos de tela e dispositivos. Isso é alcançado por meio de técnicas como:

- **Media queries para adaptar estilos e layouts com base no tamanho da tela.**

    > **DICA**  
    >*Existe um padrão "universal" referente a largura de tela:*
    >- ***320px à 480px***: *smartphones.*
    >- ***481px à 1080px***: *tablets, algumas telas pequenas.*
    >- ***1080px à 1450px***: *laptops, telas pequenas*
    >- ***1025px à 1200px***: *desktops, telas grandes*
    >- ***1201px e acima***:  *telas muito grandes, TVs * 
    
<br>

- **Imagens responsivas que se ajustam ao espaço disponível.**
- **Usar CSS flexível e layouts fluidos.**
- **Priorização de conteúdo essencial em telas menores.**

Adaptar-se a diferentes dispositivos garante que os usuários tenham uma experiência de alta qualidade, independentemente de estarem em um desktop, tablet ou smartphone.

### 2.2. Garantindo uma experiência consistente
A consistência é fundamental no design responsivo. Isso significa que, independentemente do dispositivo ou tamanho de tela, os elementos de interface devem se comportar de maneira previsível. Para garantir uma experiência consistente:

- **Mantenha a mesma estrutura de navegação em todas as versões do site.**
- **Certifique que os botões e elementos interativos sejam fáceis de tocar ou clicar em telas sensíveis ao toque.**
- **Teste tanto em emuladores quanto em dispositivos reais para verificar a consistência.**

Uma experiência consistente transmite profissionalismo e aumenta a confiança dos usuários em seu software.

Lembrando que o design responsivo não é apenas uma técnica, mas um princípio fundamental que garante que seu software seja acessível e funcional em qualquer dispositivo que os usuários possam utilizar.

## 3. Performance Otimizada
A otimização de desempenho no desenvolvimento front-end visa garantir que as interfaces de usuário carreguem rapidamente e funcionem de maneira eficiente em uma variedade de cenários.

### 3.1. Estratégias de otimização de desempenho
Para otimizar o desempenho, é essencial adotar estratégias que minimizem o tempo de carregamento da página e melhorem a responsividade da interface. Isso inclui:

- **Compactação e Minificação de Recursos**: Reduza o tamanho de arquivos CSS, JavaScript e imagens, eliminando espaços em branco e removendo código redundante.

    >**DICA**  
    >No Angular o processo de minificação é feito durante o build do projeto. Com o comando:<br>
    >`ng build --prod`
>

- **Lazy Loading**: Implemente o conceito de "lazy loading" nos módulos e imagens da aplicação. Isso significa que os módulos nao utilizados inicialmente não serão carregados até que o usuário os acesse, acelerando o tempo de carregamento inicial. E no caso das imagens, elas só serão carregadas aquelas que estiverem na janela de visualização.

   >**EXEMPLO**  
    >`<img loading="lazy" src="imagem.jpg" alt="Descrição da imagem">` 
>

- **Carregamento Assíncrono**: Carregue recursos de forma assíncrona sempre que possível, permitindo que a página seja exibida enquanto outros recursos são baixados em segundo plano.

### 3.2. Carregamento rápido de páginas
A velocidade de carregamento das páginas desempenha um papel crítico na satisfação do usuário e no SEO. Para garantir um carregamento rápido deve-se:

- **Otimize Imagens:** Comprima e dimensione imagens de forma adequada, escolhendo o formato correto (por exemplo, WebP) e usando formatos de imagem modernos.
- **Redução e Assincronismo de Requisições HTTP**: Minimize o número de solicitações HTTP necessárias, e se possível implemente requisições assíncronas
- **Priorize Conteúdo Visível**: Carregue inicialmente o conteúdo visível ao usuário e carregue recursos secundários posteriormente, conforme necessário.
- **Teste em Diferentes Velocidades de Conexão**: Verifique como sua interface se comporta em conexões lentas, garantindo que os usuários com conexões mais lentas também tenham uma experiência agradável.

## 4. Acessibilidade
A acessibilidade é um princípio crítico no desenvolvimento front-end, garantindo que todas as pessoas, incluindo aquelas com deficiências, possam usar e interagir com as interfaces de usuário de maneira eficaz.

### 4.1. Criando para todos os públicos
Desenvolver para acessibilidade significa projetar com empatia, reconhecendo as diversas necessidades dos usuários. Para criar interfaces acessíveis:

- **Utilize HTML Semântico:** Use tags HTML apropriadas para garantir uma estrutura de página bem definida. Por exemplo, use `<button>` para botões,`<section>` para seções, `<nav>` para menus de navegação, entre outras.
- **Forneça Texto Alternativo:** Sempre inclua texto alternativo para imagens, tornando o conteúdo visual acessível a pessoas com deficiência visual.
- **Teste com Tecnologias Assistivas:** Verifique como sua interface se comporta com leitores de tela, teclados e outras tecnologias assistivas.

### 4.2. Cumprindo os padrões de acessibilidade
Cumprir padrões de acessibilidade é essencial para garantir que seu software seja verdadeiramente acessível. Isso inclui:

- **Conformidade WCAG:** Siga as diretrizes do WCAG (Web Content Accessibility Guidelines) para atender aos padrões de acessibilidade.
- **Testes de Acessibilidade:** Realize testes regulares de acessibilidade usando ferramentas automatizadas e verificação manual para identificar e corrigir problemas de acessibilidade.
- **Atualizações Contínuas:** Esteja ciente de que as necessidades dos usuários podem evoluir, e mantenha-se atualizado com as últimas práticas de acessibilidade.

Garantir a acessibilidade amplia o alcance do seu software, tornando-o acessível a um público mais amplo, ao mesmo tempo que melhora a experiência para todos os usuários. É um compromisso com a inclusão e a equidade.

## 5. Manutenibilidade
A manutenibilidade no desenvolvimento front-end refere-se à capacidade de gerenciar, atualizar e aprimorar facilmente o código e as interfaces de usuário ao longo do tempo.

### 5.1. Organização do código
Uma organização de código eficaz é fundamental para a manutenibilidade. Isso inclui:

- **Estruturação Lógica:** Organize o código de forma lógica, agrupando funcionalidades relacionadas e separando responsabilidades claras.
- **Nomenclatura Intuitiva:** Use nomes de variáveis, classes e funções que sejam descritivos e autoexplicativos.
- **Verificações de Lint:** Lint é uma ferramenta que verifica se há erros no código, e incentiva bons padrões de codificação. Padrões que geralmente sao definidos no começo do projeto.
- **Comentários Descritivos:** Inclua comentários descritivos em seu código para explicar a lógica por trás das decisões e funcionalidades..

 Manter um código bem organizado facilita a localização de problemas, a realização de atualizações e a colaboração com outros membros da equipe.

 ### 5.2. Siga o padrão já existente
 Ao adicionar novo código ou funcionalidades, é importante seguir o padrão de codificação já existente. Isso garante consistência e facilita a manutenção a longo prazo. Siga o padrão existente em relação a:

- **Idioma de Variáveis, Métodos e Funções:**   
Mantenha a consistência no idioma das variáveis, métodos e funções. Se o código existente utiliza inglês para nomear variáveis, métodos e funções, mantenha em ingles a nova codificação. Se o projeto utiliza formatos como `camelCase`, siga esse padrão. Se utiliza `snake_case`, mantenha a mesma convenção.

   >**DICA**  
   >*Existem os seguintes case styles:*
   >   - *`camelCase`*
   >   - *`PascalCase`*
   >   - *`snake_case`*
   >   - *`kebab-case `*
>

- **Nomenclatura de variáveis e métodos de acordo com o seu propósito:**  
Ao nomear variaveis e metodos, nomeie-o de forma que seu propósito seja claro. Por exemplo, se você estiver chamando um serviço de "Autenticação", o método pode ser chamado de "autenticarUsuario".

   >**DICA**   
   >*Use verbos para nomear os métodos. Por exemplo:* <br>
   >   - *`calcularTotal()`*
   >   - *`listarProdutos()`*
   >   - *`togglePrices()`*
   >   - *`createForm()`*
>

Seguir o padrão já existente facilita a compreensão do código e a colaboração entre membros da equipe, tornando a manutenção mais eficiente e reduzindo erros causados por divergências de estilo.

---

[Página anterior](../README.md)