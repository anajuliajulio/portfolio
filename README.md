# Portfólio Pessoal — Arquitetura & Desenvolvimento de Sistemas

**Aluna:** Ana Júlia

---

## Descrição do Portfólio

Este projeto é um portfólio pessoal desenvolvido para apresentar minha trajetória profissional e acadêmica, conectando minha formação em **Arquitetura e Urbanismo** aos meus estudos atuais no curso técnico em **Desenvolvimento de Sistemas**. A página reúne minhas principais informações, habilidades técnicas em evolução, vitrine de projetos e canais de contato.

---

## Link do Site Publicado

 **Acesse o portfólio online:** [https://anajuliajulio.github.io/nome-do-repositorio/](https://anajuliajulio.github.io)  
*(Substitua `nome-do-repositorio` pelo nome exato do seu repositório no GitHub após ativar o GitHub Pages)*

---

## Tecnologias Utilizadas

* **HTML5:** Estruturação semântica das seções da página (`nav`, `header`, `section`, `footer`).
* **CSS3:** Estilização personalizada, controle de variáveis de cores, layout e ajustes visuais.
* **Bootstrap 5 & Bootstrap Icons:** Sistema de grid responsivo, componentes de navegação, cards e ícones.
* **JavaScript:** Manipulação do DOM para interatividade, alternância de tema e animação de componentes.
* **Google Fonts:** Tipografia combinando as fontes *Fraunces* (títulos) e *Inter* (textos).

---

## Explicação do Funcionamento do Projeto

O portfólio funciona como uma *Single Page Application* (página única) totalmente responsiva, adaptando-se a computadores, tablets e celulares:

1. **Navegação Fixa com ScrollSpy:** O menu superior acompanha a rolagem da tela e destaca automaticamente a seção em que o usuário está.
2. **Apresentação (Hero):** Exibe o resumo profissional, botões de ação rápida e a foto de perfil.
3. **Seção de Habilidades:** Apresenta barras de progresso dinâmicas indicando o nível atual de domínio em cada tecnologia estudada.
4. **Vitrine de Projetos:** Exibe cards organizados com descrição, tecnologias aplicadas e links diretos para os repositórios no GitHub.
5. **Alternância de Tema (Claro/Escuro):** Um botão no menu permite alternar o esquema de cores da página em tempo real, alterando o atributo `data-bs-theme` do HTML via JavaScript.

---

## Descrição do Recurso Novo Adicionado

Além das adaptações visuais, identidade própria e integração da foto de retrato personalizada, foram adicionados os seguintes recursos de evolução sobre o modelo base:

* **Seção Estruturada de Vitrine de Projetos (`#projetos`):** Inclusão de uma nova seção dedicada à exibição de projetos em formato de *cards* interativos com tags de tecnologias, links externos e card de "Em breve".
* **Enquadramento Circular Responsivo com Proporção Fixa:** Implementação de um contêiner estilizado para a foto de retrato (`foto-ana.jpg`), garantindo corte circular perfeito sem distorções independentemente do tamanho da tela.

---

## Explicação de Como Esse Recurso Foi Implementado

1. **Vitrine de Projetos:**
   * No **HTML5**, foi criada uma nova `<section id="projetos">` integrada ao `ScrollSpy` da barra de navegação (`#menu`).
   * Utilizou-se o sistema de grid do **Bootstrap 5** (`row g-4` e `col-md-6 col-lg-4`) aliado ao componente `card h-100` e classes *Flexbox* (`d-flex flex-column`, `flex-grow-1`) para manter todos os cards alinhados com a mesma altura, independentemente do tamanho do texto.
   * Foram adicionadas *badges* (`bg-secondary-subtle`) para identificar as stacks de cada projeto e links com `target="_blank" rel="noopener"` para segurança na abertura de abas externas.

2. **Enquadramento da Foto de Retrato:**
   * Na seção `#perfil`, a imagem (`foto-ana.jpg`) foi envolvida em uma `div.foto-wrapper` com proporção travada (`aspect-ratio: 1`) e bordas totalmente arredondadas (`border-radius: 50%`, `overflow: hidden`).
   * Na tag `<img>`, aplicou-se `object-fit: cover` com largura e altura em `100%`, além de borda e sombra do Bootstrap (`shadow-lg border border-4`), garantindo que a foto preencha o círculo sem esticar ou achatar a imagem.

---

## Estrutura dos Arquivos

```text
├── index.html          # Estrutura principal da página
├── foto-ana.jpg        # Foto de retrato exibida no perfil
├── README.md           # Documentação do projeto
├── css/
│   └── style.css       # Estilos personalizados e variáveis de tema
└── js/
    └── script.js       # Lógica do modo escuro e animações
```
