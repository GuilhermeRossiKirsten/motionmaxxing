# Bloom filter — storyboard (20 s, 1920x1080, 30 fps)

## PAGE
- **P** Bloom filter é explicado com diagramas de caixinhas e fórmulas; ninguém *vê* por que ele diz "com certeza não" e só "talvez sim".
- **A** Devs e estudantes num feed, possivelmente sem som. Precisa ler sem áudio.
- **G** Educação: sair entendendo a assimetria (falso positivo existe, falso negativo não).
- **E** De "mais uma estrutura de dados chata" para "ah, é só isso — e é genial".

Um fato verdadeiro: o filtro não guarda o elemento, só k bits ligados por k funções de hash; a consulta olha os mesmos k bits.

## Inventário (não há marca: identidade decidida de propósito)
| Olhar | Resposta |
|---|---|
| Forma | o array de bits — uma fita perfurada (paper tape) |
| Controle | inserir / consultar |
| Material | papel de fita perfurada sobre uma mesa de luz: bit 1 = furo por onde a luz passa |
| Verbo | perfurar (inserir), olhar através (consultar) |
| Momento de sucesso | um raio cai em papel sem furo → "com certeza não" |
| Voz | técnica, curta, honesta, em pt-br; sem jargão de marketing |
| Cor | âmbar = luz = bit ligado (único acento, um significado); creme = tinta; resto é papel e sombra |
| Tipo | Inter 450-550, sentence case |
| Nunca faria | flor desabrochando, glow de "IA", stat slide |

## Ideias
1. (descartada) Uma flor desabrochando — primeira associação do nome.
2. UI documentary: um campo "nome de usuário disponível?" consultando um filtro. Bom, mas é o filme de qualquer cache/DB.
3. **Escolhida — um plano único que muda:** uma fita perfurada sobre uma mesa de luz. Cada palavra dispara 3 raios (h1,h2,h3) que furam a fita e vão embora; a palavra some, os furos ficam. Consultas olham os mesmos furos. Só a estrutura em si filma isso: o "não guarda a palavra" é encenado, não legendado.

Por quê: o material (furo = 1, luz = verdade) torna a assimetria visível — um furo apagado é prova; três acesos podem ser coincidência.

## Mundo
- Chão: mesa escura quente (#15120E) com textura, luz-chave vindo de cima/esquerda.
- Luz: a mesa de luz âmbar por trás da fita; só os furos deixam passar. Luz = significado.
- Profundidade: fita (plano principal) com sombra na mesa; raios por cima; texto em espaço de tela.
- Textura: grão de papel, furos de tração (sprocket) na borda da fita, numeração impressa das células.
- Som: sem ElevenLabs nesta máquina → SFX sintetizados (ffmpeg): perfuração seca, tique de consulta, um tom baixo no "não", duas notas no "talvez", um acorde quente no fim.

**Momento-screenshot:** macro na célula 91: dois furos âmbar acesos à esquerda e à direita, o raio da consulta "lua?" parado sobre papel opaco.

## Beats (importância 1-3; ≤25% são 3)
| # | f | papel | compra | cópia | o que move | passagem |
|---|---|---|---|---|---|---|
| 1 | 0-80 | hook (2) | o espectador entende que a palavra não é guardada | "Um Bloom filter não guarda a palavra." | "gato" chega de 2x, 3 raios furam 3 células, "gato" sai para cima e some | os furos ficam acesos |
| 2 | 80-190 | turn (1) | inserir é só isso, e rápido | "Guarda só os furos que ela deixa." | "sol", "rio", "mar" em ritmo acelerando; furos se acumulam | a fita cheia de luz recebe a consulta |
| 3 | 190-330 | proof (3) | um furo apagado prova o "não" | "lua?" → "Um furo apagado: com certeza não." | raios tracejados; 2 caem em luz, 1 em papel; câmera mergulha na célula escura | corte em movimento para o plano aberto |
| 4 | 330-455 | proof (2) | três acesos podem ser coincidência | "pão?" → "Tudo aceso: talvez." | 3 raios caem em furos de gato, sol e rio; etiquetas a lápis mostram quem furou | câmera recua |
| 5 | 455-600 | cta (2) | é uma fita enorme, barata, e a regra é uma só | "Nunca erra um não. Às vezes, um sim." → "Bloom filter" | recuo para 0.2x: a fita vira uma linha de luzes; título chega de 2.4x e assenta | fim com respiração das luzes |

Cobrindo o texto: fita de papel com furos de luz, raios caindo, câmera mergulhando e recuando — há imagem em todo quadro.
Gates previstos: G1 fita cortada pela borda do quadro, texto ≥ 0.05 H; G3 título assenta ~f560, final ≤ 25%; G4 um herói (a fita).
