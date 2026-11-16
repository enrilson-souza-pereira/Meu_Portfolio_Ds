# Meu_Portf-lio_Ds

# Portfólio Pessoal - Enrilson Souza Pereira

**Aluno:** Enrilson Souza Pereira  
**Localidade:** São Paulo - SP  

## Descrição do Portfólio
Este projeto consiste no desenvolvimento e na evolução de um portfólio web pessoal e responsivo, criado para a atividade prática da disciplina de Desenvolvimento de Sistemas. A página apresenta minha formação dupla na Etec (**Técnico em Desenvolvimento de Sistemas** e **Técnico em Mecatrônica**), competências técnicas, fluência em idiomas (Inglês e Espanhol fluentes, Alemão em curso), projetos desenvolvidos e canais de contato profissional.

## Tecnologias Utilizadas
* **HTML5:** Estruturação semântica do conteúdo.
* **CSS3:** Estilização customizada, gradientes, transições e animações de interface.
* **Bootstrap 5 & Bootstrap Icons:** Sistema de grid responsivo, componentes de navegação (`navbar`), cards, barras de progresso e botões.
* **JavaScript (ES6):** Manipulação do DOM para filtragem dinâmica de projetos por categoria.
* **Git & GitHub Pages:** Versionamento de código e hospedagem estática gratuita.

## Link do Site Publicado
Acesse o portfólio online através do link:  
🔗 [https://enrilson-souza-pereira.github.io/portfolio/](https://enrilson-souza-pereira.github.io/portfolio/)  
*(Nota: Caso o nome do seu repositório no GitHub seja diferente de `portfolio`, substitua esse trecho na URL acima pelo nome exato do repositório).*

## Funcionamento do Projeto
O site adota uma estrutura moderna em *One-Page* com navegação fluida:
1. **Menu de Navegação Fixo:** Utiliza o componente `navbar` do Bootstrap com rolagem suave (*ScrollSpy*), colapsando em menu hambúrguer para dispositivos móveis.
2. **Seção de Perfil:** Exibe a foto integrada diretamente do perfil oficial do GitHub (`enrilson-souza-pereira`), título profissional e resumo da integração entre software e automação.
3. **Seção de Habilidades & Formação:** Cards responsivos apresentando indicadores visuais de proficiência técnica, as formações técnicas em Desenvolvimento de Sistemas e Mecatrônica pela Etec, além do domínio de idiomas (Inglês, Espanhol e Alemão).
4. **Seção de Projetos:** Grade de cards com descrições, tags de tecnologias e links diretos para os repositórios no GitHub.
5. **Seção de Contato:** Atalhos para o perfil profissional e formulário interativo para envio de mensagens.

## Recursos Novos Adicionados
Para ir além da estrutura básica vista em aula, foram implementados três recursos extras:
1. **Nova Seção de Habilidades e Formação:** Área dedicada às competências técnicas (com barras de progresso do Bootstrap), formação dupla na Etec e idiomas.
2. **Animações e Micro-interações CSS:** Efeito de elevação (`translateY`) com sombra nos cards de projetos ao passar o cursor (`:hover`), zoom suave na foto de perfil e sublinhado animado nos links do menu.
3. **Filtro Interativo de Projetos por Categoria:** Botões dinâmicos que permitem filtrar os projetos exibidos na tela (*Todos*, *Desenvolvimento Web* e *Python & Lógica*) sem recarregar a página.

## Como os Recursos Foram Implementados
* **Animações CSS (`style.css`):** Utilizou-se a propriedade `transition: transform 0.3s ease, box-shadow 0.3s ease` na classe `.project-card`. No estado `:hover`, aplicou-se `transform: translateY(-8px)` para criar profundidade visual. Nos links da barra de navegação, empregou-se o pseudo-elemento `::after` com largura animada de `0%` a `100%`.
* **Filtro Dinâmico (`index.html`):** Cada card de projeto recebeu um atributo personalizado `data-categoria` (ex: `data-categoria="web"` ou `data-categoria="python"`). Um script em JavaScript captura os cliques nos botões de filtro (`.filter-btn`), lê o atributo `data-filter` selecionado e alterna a propriedade CSS `display` (`block` ou `none`) dos cards correspondentes em tempo real.