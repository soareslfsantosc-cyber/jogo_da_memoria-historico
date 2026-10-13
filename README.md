# Jogo da Memória Histórica — XByte Games Studio

Jogo da memória para navegador com tema de personagens históricos. Encontre os pares de cartas, acompanhe suas tentativas e conheça um pouco sobre cada personalidade.

## Personagens

O tabuleiro contém pares de imagens de oito personagens:

- Albert Einstein
- Cleópatra VII
- Joana d'Arc
- Malala Yousafzai
- Martin Luther King Jr.
- Marie Curie
- Nelson Mandela
- Napoleão Bonaparte

## Recursos

- Tabuleiro embaralhado com 16 cartas (8 pares).
- Contador de tentativas e registro da melhor pontuação.
- Biografia exibida ao encontrar um par.
- Ranking local com até oito melhores resultados, ordenados por tempo e tentativas.
- Animações, efeitos visuais e arquibancada ilustrada em canvas.
- Layout responsivo para desktop e dispositivos móveis.
- Botões para iniciar um novo jogo e consultar o ranking.

## Como executar

Não há dependências de build nem backend. Abra `index.html` em um navegador moderno. Para servir os arquivos localmente, use:

```bash
python3 -m http.server 8000
```

Em seguida, abra <http://localhost:8000>.

As imagens ficam na pasta `images/`. O ranking é guardado no `localStorage` do navegador em uso; portanto, os resultados não são compartilhados entre navegadores ou dispositivos. A página carrega o reset CSS e a fonte decorativa por URLs externas, então esses recursos visuais dependem de conexão com a internet; a fonte do sistema funciona como alternativa.

## Estrutura do projeto

```text
.
├── index.html
├── script.js
├── style.css
├── README.md
└── images/
    ├── cleopatra.jpg
    ├── curie.jpg
    ├── einstein.jpg
    ├── joana.jpg
    ├── malala.jpg
    ├── mandela.jpg
    ├── mlk.jpg
    └── napoleao.jpg
```

## Verificação

Para verificar a sintaxe do JavaScript com Node.js:

```bash
node --check script.js
```
