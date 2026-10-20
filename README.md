# 🎵 Projeto Música

Site educativo sobre música, desenvolvido como Projeto Integrador do curso de **Informática para Internet** (Info Noturno) da **ETEC de Nova Odessa** (Centro Paula Souza), para o evento **ETEC de Portas Abertas**.

O site apresenta o que é música, seus grandes grupos e estilos, e sua importância para as emoções, a mente, a conexão entre pessoas e a identidade cultural. É feito com páginas estáticas em HTML e CSS.

🔗 **Site no ar:** https://victorgx7.github.io/Projeto-m-sica/index.html

🔗 **Protótipo de Alta fidelidade:** https://www.figma.com/design/OPh7Z2orXz0FEgmYvUokMT/Projeto---M%C3%BAsica?node-id=0-1&t=WVPcLherEKcODLbF-1

---

## 📑 Sumário

- [Páginas do site](#-páginas-do-site)
- [Tecnologias](#-tecnologias)
- [Estrutura do projeto](#-estrutura-do-projeto)
- [Padrões do código](#-padrões-do-código)
- [Equipe](#-equipe)

---

## 📄 Páginas do site

| Arquivo | Página | Descrição |
|---|---|---|
| `index.html` | Home | Apresentação do projeto: seção principal com a frase "A música faz parte de quem somos", boas-vindas, três blocos de conteúdo (Estilos musicais, História da música e Impacto cultural) e botões para explorar os estilos e conhecer o projeto. |
| `sobre.html` | Sobre | Explica o que é música ("a arte de combinar sons e silêncios") e como ela acompanha a humanidade, com imagens ilustrativas em duas seções alternadas. |
| `tiposmusicas.html` | Tipos musicais | Apresenta os três grandes grupos (música erudita, popular e folclórica), um quadro comparativo com a definição e os estilos de cada grupo, e um vídeo do YouTube sobre gêneros musicais. |
| `importancia.html` | Importância | Quatro blocos sobre o valor da música (Emoções e sentimentos, Mente e criatividade, Conexão entre pessoas, História e identidade) e um link para um vídeo em destaque no YouTube. |
| `Creditos.html` | Créditos | Créditos do projeto: turma e curso, desenvolvedores e professores orientadores. |
| `desenvolvedores.html` | Sobre os desenvolvedores | Apresenta cada integrante da equipe e sua responsabilidade no projeto. |
| `SobreEtec.html` | Sobre a ETEC | Informações sobre o Centro Paula Souza e a ETEC de Nova Odessa, com links para as redes sociais. |
| `subdivisoes.html` | Subdivisões da música | Contém o quadro comparativo dos grandes grupos e o vídeo de gêneros musicais, mesmo conteúdo da parte final de `tiposmusicas.html`. Nenhuma página do site linka para ela. |

### Navegação

Todas as páginas compartilham a mesma estrutura:

- **Navbar** no topo, com o logo "MÚSICA" e os links Home, Sobre, Tipos musicais e Importância. A página atual recebe a classe `active`. À direita ficam links externos para o Instagram da ETEC de Nova Odessa e para o site do Centro Paula Souza.
- **Rodapé** com o logo, os mesmos links principais, links para Créditos e Sobre os desenvolvedores, ícones de redes sociais (que levam a `SobreEtec.html`) e o aviso de direitos autorais de 2026.

---

## 🛠 Tecnologias

- **HTML5**, com `lang="pt-br"`, meta `description` em cada página e atributos de acessibilidade (`aria-label`, `aria-labelledby`, `alt` nas imagens).
- 
- **CSS3**, com um arquivo global e arquivos específicos por página.
- 
- **YouTube (iframe)**, para o vídeo educativo de gêneros musicais.
- 
- **GitHub Pages**, para a hospedagem do site.
- 
- **Figma**, Para prototipagem do site.

---

## 📁 Estrutura do projeto

```
Musica-EtecPortasAbertas/
├── .vscode/                  # Configurações do editor
├── assets/                   # Imagens e ícones
│   ├── icon/                 # Ícones (notas-musicais, coracao, cerebro, pessoas)
│   ├── pessoas/              # Fotos da equipe e dos professores
│   ├── headphones-hero.jpg
│   ├── Frequencia.jpeg
│   ├── Harmonia.jpeg
│   ├── Pessoas.jpeg
│   ├── NotaMusicais.jpeg
│   ├── musica-erudita.jpg
│   ├── musica-popular.jpg
│   ├── musica-folclorica.jpg
│   ├── etec-nova-odessa.jpg
│   ├── logoInfo.jpeg
│   ├── TurmaInfo.jpeg
│   ├── instagram.png
│   ├── logo_cps_versao_br.png
│   └── logo_cps_versao_cor.png
├── css/
│   ├── style.css             # Estilos globais (navbar, rodapé)
│   ├── home.css              # Estilos da Home
│   ├── sobre.css             # Estilos da página Sobre
│   └── tiposmusicas.css      # Estilos de Tipos musicais / Subdivisões
├── index.html
├── sobre.html
├── tiposmusicas.html
├── importancia.html
├── Creditos.html
├── desenvolvedores.html
├── SobreEtec.html
└── subdivisoes.html
```

> A pasta `css/` pode conter outros arquivos, usados por páginas como Importância e Créditos. Os listados acima são os que aparecem no código de `index.html`, `sobre.html` e `subdivisoes.html`.

## 🧩 Padrões do código

- **CSS por página:** cada página carrega `css/style.css` (comum a todas) e o CSS próprio dela. Ex.: `index.html` carrega `home.css`, e `sobre.html` carrega `sobre.css`.
- **Classes com prefixo por página:** `home-*` na Home, `sobre-*` em Sobre e `tipos-*` em Tipos/Subdivisões. Isso evita conflito de estilos entre páginas.
- **Acessibilidade:** imagens decorativas usam `alt=""` e `aria-hidden="true"`, e imagens com significado têm texto alternativo descritivo.
- **Carregamento de imagens:** o atributo `loading` é usado (`eager` para a imagem principal, `lazy` para as demais).
- **Links externos:** abrem em nova aba com `rel="noopener noreferrer"`.

---

## 👥 Equipe

| Nome | Função |
|---|---|
| Victor G. De Sousa | Desenvolvedor / Líder do Projeto: liderança técnica, coordenação da equipe e desenvolvimento das funcionalidades |
| Luana de S. Retamero | Desenvolvedora / Designer: concepção visual, experiência do usuário e interfaces |
| Otávio B. Guedes | Desenvolvedor / Designer: estrutura das páginas e apoio na identidade visual |

**Professores orientadores:** Samuel Santos e Camila Spadaro.

**Curso:** Informática para Internet (Info Noturno), ETEC de Nova Odessa, turma 2026-2028.
