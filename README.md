# Portfolio - Everson Henrique

> Site de portfólio pessoal criado em HTML e CSS que apresenta uma breve apresentação, seção "Sobre mim", projetos e formulário de contato.

## Visão geral

Este repositório contém um site estático (HTML + CSS) que funciona como portfólio pessoal. O conteúdo principal está em `index.html` e os estilos e ativos (imagens, ícones) estão na pasta `src`.

Principais seções do site:
- Início — introdução e tecnologias
- Sobre mim — texto descritivo, interesses, formações e link para o GitHub
- Projetos — cards para apresentar projetos
- Contatos — formulário simples (front-end apenas)

## Como visualizar localmente

Opções rápidas para abrir o site no seu computador:

1) Abrir diretamente no navegador

   - Abra o arquivo `index.html` no seu navegador (clique duas vezes ou use "Abrir com" no Windows).

2) Servir via servidor HTTP simples (recomendado para evitar problemas de CORS com fetch ou módulos)

   - Se você tiver Python instalado (recomendado):

     - Python 3.x:
       - No PowerShell, execute:
         ```powershell
         python -m http.server 8000
         ```
       - Abra `http://localhost:8000` no navegador.

   - Alternativa com Node.js (se tiver instalado):

       - Instale o pacote `http-server` globalmente (uma vez):
         ```powershell
         npm install -g http-server
         ```
       - Então rode:
         ```powershell
         http-server -p 8000
         ```

## Estrutura do projeto

```
index.html
src/
  assets/         # imagens, logos e ícones usados pelo site
  styles/         # arquivos CSS (global.css, e seções específicas)
```

- `index.html` — página principal do portfólio.
- `src/styles/global.css` — estilos globais; também existem arquivos de CSS por seção em `src/styles`.
- `src/assets/` — imagens como `logo-olhos.png`, `tecnologias.png`, fotos de perfil e ícones.

## O que editar para personalizar

- Para trocar o nome, ocupação e textos principais: edite `index.html` nos elementos dentro da seção `#inicio-sec` e `#sobre-mim-sec`.
- Para atualizar projetos: edite a seção `#projetos-sec` e substitua os cards por projetos reais (imagem, título, descrição e links).
- Para alterar estilos: modifique os arquivos em `src/styles/`.
- Para trocar imagens e ícones: substitua ou adicione arquivos em `src/assets/` e atualize os caminhos em `index.html`.

## Observações importantes

- O formulário em `#contatos-sec` é apenas visual — ele não envia mensagens sem um backend ou uma integração com um serviço de formulário (por exemplo, Formspree, Netlify Forms ou um endpoint próprio).
- O site é estático; para deploy simples, use GitHub Pages, Netlify ou Vercel.

## Sugestões de melhorias

- Adicionar um backend leve para processar o formulário de contato (Node.js/Express, serverless function).
- Melhorar a responsividade e acessibilidade (contraste, labels, validação de formulário).
- Configurar SEO básico (meta tags, Open Graph) e arquivo `robots.txt`.
- Incluir um `LICENSE` se quiser deixar explícito como outras pessoas podem reutilizar seu trabalho.

## Contribuições

Se quiser contribuir com melhorias, abra uma issue descrevendo a sugestão ou envie um pull request com mudanças.

## Contato

Perfil do autor (GitHub): https://github.com/pablo-lorenzo09

---

Se quiser, posso:
- adicionar um `LICENSE` (sugiro MIT),
- transformar o formulário em funcional com um exemplo de endpoint em Node.js,
- ou criar um deploy para o GitHub Pages e te guiar nos passos.
