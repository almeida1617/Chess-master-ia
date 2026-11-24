# Guia do Chess Master AI

## O que funciona nesta versão
- Tabuleiro 8×8 com regras legais de xadrez via chess.js.
- Histórico de lances clicável, desfazer/refazer, inverter tabuleiro, reiniciar.
- Importação e exportação de PGN e carregamento de FEN.
- Biblioteca local de PGNs: importar arquivos, abrir partidas no tabuleiro e remover itens.
- Enciclopédia inicial de regras, tática, estratégia e finais.
- Catálogo introdutório de 25 aberturas e gambitos.
- Treinamento com 12 perguntas e explicações.
- Repertório pessoal e anotações guardados no armazenamento local do navegador.
- Links para coleções PGN de dez grandes mestres.
- Integração de Stockfish 19 Lite single-threaded via Web Worker e WebAssembly, carregada sob demanda.

## Como estudar partidas dos mestres
1. Abra a seção Grandes mestres.
2. Entre na página PGN Mentor e procure o jogador.
3. Baixe o arquivo PGN desejado.
4. No Chess Master AI, use Importar partidas.
5. Abra a partida e clique em qualquer lance para navegar pelo histórico.
6. Se quiser, carregue Stockfish e analise a posição atual.

A coleção externa é mantida pelo PGN Mentor e pode mudar. O projeto não copia nem promete conter todas as partidas existentes. A base é uma porta de entrada para importar os jogos que você quiser estudar.

## Limitações conhecidas
- Stockfish é um motor de avaliação, não um tutor conversacional. O uso do motor depende de internet, suporte a WebAssembly e disponibilidade do CDN. O funcionamento precisa ser confirmado no navegador e aparelho de cada usuário.
- A avaliação e a linha principal são ferramentas de apoio; não substituem comentários humanos nem provam a intenção psicológica de um jogador.
- As aulas são resumos autorais. Os PDFs de Orfeu D'Agostini, Ludek Pachman e Bobby Fischer são referências para estudo; esta versão não contém uma transcrição ou revisão completa de cada capítulo.
- A lista de aberturas é introdutória, não um catálogo exaustivo de todas as variantes, gambitos, armadilhas ou refutações.
- O projeto é uma aplicação web estática; não tem contas, sincronização entre aparelhos, multiplayer ou tutor de IA em nuvem.

## Privacidade
Partidas importadas, repertório e anotações ficam no armazenamento local do navegador. Limpar os dados do site pode apagar essas informações. Não importe arquivos pessoais ou dados que não queira manter no aparelho.

## Créditos e licenças
- chess.js: biblioteca de regras de xadrez, distribuída sob licença BSD-2-Clause.
- Stockfish.js 19 Lite: motor de código aberto sob GNU GPL v3. A versão carregada é single-threaded e usa WebAssembly.
- PGN Mentor: fonte externa de coleções PGN disponibilizadas gratuitamente para estudo; consulte a página original para detalhes e condições.

Fontes:
- https://github.com/jhlywa/chess.js
- https://github.com/nmrugg/stockfish.js
- https://www.pgnmentor.com/files.html
