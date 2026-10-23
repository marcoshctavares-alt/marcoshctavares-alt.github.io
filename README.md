# Portfólio — Marcos Tavares

<img width="1332" height="611" alt="screenport" src="https://github.com/user-attachments/assets/c6ae3a8b-acbe-4585-98c5-3d34e90b8450" />


Site de portfólio pessoal de **Marcos Tavares**, desenvolvedor de software generalista, com tema de jardim botânico, modo claro e escuro e layout responsivo.

 **Site no ar:** https://marcoshctavares-alt.github.io

##  Recursos

- Página única (*single page*) com as seções **Início**, **Quem Sou**, **Projetos** e **Contato**
- **Modo claro e escuro**: detecta a preferência do sistema (`prefers-color-scheme`) e tem botão sol/lua, com a escolha salva em `localStorage`
- Cabeçalho fixo com **rolagem suave**, destaque automático da seção visível (*scroll spy*) e **menu lateral** no celular
- Animações em CSS (folhas, vagalumes, aparecer ao rolar) que respeitam `prefers-reduced-motion`
- Formulário de contato com validação, que envia a mensagem para o e-mail via [FormSubmit](https://formsubmit.co) (com plano B por `mailto:`)
- Acessibilidade: navegação por teclado, `aria-label`, link "pular para o conteúdo" e contraste adequado nos dois temas
- Sem frameworks e sem etapa de build: **apenas HTML, CSS e JavaScript** em um único arquivo

##  Como rodar localmente

Não precisa instalar nada. Baixe o repositório e abra o `index.html` no navegador


##  Publicar no GitHub Pages

1. Suba o `index.html` para a raiz do repositório (público).
2. Vá em **Settings → Pages**.
3. Em **Build and deployment**, escolha **Deploy from a branch**, branch `main` e pasta `/ (root)`.
4. Aguarde alguns minutos: o endereço do site aparece no topo da mesma página.

##  Como personalizar

Tudo está no `index.html`, com comentários nas partes principais:

| O que mudar | Onde |
|---|---|
| Cores dos temas | Variáveis CSS no começo do `<style>` (`:root` e `[data-theme="dark"]`) |
| Nome, textos e bio | Seções `#inicio` e `#quem-sou` no HTML |
| Foto | Tag `<img class="avatar">` (a imagem está embutida em base64; troque o `src` por um arquivo, se preferir) |
| Habilidades | Lista `<ul class="skills">` |
| Projetos | Array `projects` no `<script>` (título, descrição, link e imagem) |
| Links de contato | Bloco `.socials` (GitHub, WhatsApp e e-mail) |
| E-mail que recebe o formulário | Constante `CONTACT_EMAIL` no `<script>` |

###  Ativando o formulário de contato

O formulário usa o FormSubmit, que não precisa de servidor. No **primeiro envio**, o serviço manda um e-mail de ativação para o endereço configurado em `CONTACT_EMAIL`. Abra esse e-mail e clique no link de confirmação, uma única vez. Depois disso as mensagens passam a chegar normalmente.

##  Tecnologias

HTML5 · CSS3 (custom properties, grid, flexbox) · JavaScript (ES6+) · Google Fonts (Fraunces e Nunito Sans)

##  Licença

O **código** deste repositório está sob a licença [MIT](LICENSE).

A licença **não cobre**: a foto pessoal, os textos de apresentação e as imagens dos sites de terceiros exibidos na seção de projetos (Jeene, Boanerges & Cia, Gengibre da Natureza e ABAV). Esses conteúdos pertencem aos seus respectivos autores e titulares e **não podem ser reutilizados** sem autorização.

##  Contato

- GitHub: https://github.com/marcoshctavares-alt
- E-mail: marcos.hc.tavares@gmail.com
