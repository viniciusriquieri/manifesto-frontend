# Processo de Implantação

A fase de implantação envolve a integração e o lançamento do código em um ambiente de produção. 

## Índice
1. [Envio e Preparação de Código](#1-foco-no-usuário)
   - 1.1. Entendendo as necessidades do usuário
   - 1.2. Criando experiências intuitivas
2. [Code Review](#2-design-responsivo)
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




## 1. Envio e Preparação de Código

- **Commit Messages Descritivos:** Antes de enviar qualquer código, certifique-se de que os commit messages sejam descritivos e concisos. Eles devem explicar claramente o que foi alterado ou adicionado.

    >**IMPORTANTE**  
    >*Será usado o seguinte formato de commit:  
    `<tipo>[história]: <descrição>`*  
    >
    >Exemplos:  
    >`feat(OWN-9494): desenvolvimento da tela de pagamento via pix`
    >
    >Clique [aqui]() para mais detalhes sobre commit message.
>

- **Criação de Pull Request/Merge Request:** Após concluir as implementações ou correções, crie um pull request/merge request da sua branch com a "release-dev". Com o MR/PR criado, sinalize o líder técnico para que ele possa revisar seu código.

## 2. Code Review
Com o objetivo de manter um código padronizado de qualidade e fácil manutenção, o desenvolvedor não terá mais liberdade para subir o que bem entender para os ambientes. Haverá uma etapa antes de seu código ser mergeado.

- **Revisao do Código**: 
O líder técnico será responsável por revisar o código e aprová-lo ou não, caso nao atenda aos padrões mencionados acima.

- **Feedback e Ajustes:** Se necessário, ajustes ou melhorias podem ser solicitados durante a revisão. Certifique-se de responder prontamente às observações do líder técnico.

## 3. Disponibilização em outros Ambientes
Após a revisão e preparação, o código será disponibilizado na "release-dev" e também nos ambientes "release-qa" (Quality Assurance) e "release-hml" (Homologação). Isso permitirá testes adicionais para garantir que as alterações funcionem corretamente em diferentes cenários.



## 4. Agrupamento e preparação para Implantação
- **Agrupamento das funcionalidades:** O líder técnico pode consolidar várias funcionalidades em um único pacote de alterações, se apropriado, para simplificar o processo de implantação.

- **Preparação para Produção:** Com as funcionalidades consolidadas e aprovadas, elas serão disponibilizadas na branch "release-prd", para serem preparadas para implantação em produção (master).

- **Implantação em Produção:** Com a release-prd preparada, seguirá o processo de implantação padrão da Valecard.



Esse processo de implantação visa garantir que o código seja cuidadosamente revisado e que a implantação em produção seja realizada de forma organizada e segura. Certifique-se de seguir as etapas e colaborar com o líder técnico para manter a qualidade do software.

---

[Página anterior](../README.md)