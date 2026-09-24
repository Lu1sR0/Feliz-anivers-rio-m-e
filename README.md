<div align="center">

# Feliz Aniversário, Mãe

Uma mensagem de aniversário animada, feita como presente para a minha mãe.

[![Ver site](https://img.shields.io/badge/VER_SITE-0D0D0D?style=for-the-badge&logo=vercel&logoColor=FF003C)](https://felizaniversariomae.vercel.app)

![HTML5](https://img.shields.io/badge/HTML5-0D0D0D?style=for-the-badge&logo=html5&logoColor=FF003C)
![CSS3](https://img.shields.io/badge/CSS3-0D0D0D?style=for-the-badge&logo=css&logoColor=FF003C)
![JavaScript](https://img.shields.io/badge/JavaScript-0D0D0D?style=for-the-badge&logo=javascript&logoColor=FF003C)
![GSAP](https://img.shields.io/badge/GSAP-0D0D0D?style=for-the-badge&logo=greensock&logoColor=FF003C)

</div>

## Sobre

Página de uma tela só que conta uma pequena história animada até chegar ao "Feliz aniversário". Em vez de um cartão estático, a mensagem aparece em etapas: saudação, uma conversa que "quase" foi enviada, frases que entram e saem de cena, balões, a foto da aniversariante com chapéu de festa e, por fim, a dedicatória.

Todo o conteúdo em texto fica em um arquivo JSON, então a mesma base pode ser reaproveitada para outras pessoas sem mexer no HTML.

## Funcionalidades

- **Linha do tempo animada** com GSAP (`TimelineMax`), com dezenas de etapas encadeadas.
- **Mensagem digitada**: o texto da caixa de conversa aparece letra por letra e o botão "enviar" muda de cor.
- **Frases em sequência** com entradas e saídas em perspectiva (rotação e inclinação).
- **Balões subindo** pela tela, foto com chapéu de festa e o título "Feliz aniversário" animado letra a letra.
- **Efeito de confete** com círculos que se expandem em ondas.
- **Replay**: um clique no texto final reinicia toda a animação.
- **Conteúdo configurável**: saudação, nome, frases, dedicatória e caminho da foto ficam em `customize.json`.

## Tecnologias

- HTML5, CSS3 e JavaScript puro
- [GSAP](https://gsap.com/) 1.20 (TweenMax, via CDN)
- [Google Fonts](https://fonts.google.com/): Work Sans
- [Vite](https://vitejs.dev/) e [Browser Sync](https://browsersync.io/) como servidores de desenvolvimento

## Estrutura

```
├── index.html        # Estrutura das cenas
├── customize.json    # Textos e foto exibidos na animação
├── script/main.js    # Lê o JSON, preenche a página e monta a timeline
├── style/style.css   # Layout e estados iniciais das cenas
└── img/              # Balões, chapéu, favicon e foto
```

## Como rodar localmente

O script carrega o `customize.json` com `fetch`, então a página precisa ser servida por HTTP (abrir o `index.html` direto do disco não funciona).

```bash
git clone https://github.com/Lu1sR0/Feliz-anivers-rio-m-e.git
cd Feliz-anivers-rio-m-e
npm install
npm run dev
```

Outra opção é abrir a pasta no VS Code e usar a extensão **Live Server**.

### Personalizando

1. Edite os textos em `customize.json`.
2. Substitua a foto em `img/` e atualize o campo `imagePath`.

## Créditos

Baseado no projeto open source [happy-birthday](https://github.com/faahim/happy-birthday), de Afiur Rahman Fahim, distribuído sob a licença MIT (veja [LICENSE](./LICENSE)). Textos traduzidos e personalizados para esta homenagem.

---

<div align="center">
Desenvolvido por <a href="https://github.com/Lu1sR0">Luis Roberto</a> · <a href="https://outframe.dev">Outframe</a>
</div>
