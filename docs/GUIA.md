# Guia do Chess Master AI

## O que funciona nesta versão
- Tabuleiro 8×8 com regras legais de xadrez via chess.js.
- Histórico de lances clicável, desfazer/refazer, inverter tabuleiro, reiniciar.
- Importação e exportação de PGN e carregamento de FEN.
- Biblioteca PGN local: importar arquivos com uma ou várias partidas, pesquisar, paginar, abrir partidas no tabuleiro e remover itens. Os jogos são guardados no IndexedDB do navegador.
- Enciclopédia inicial de regras, tática, estratégia e finais.
- Catálogo introdutório de 25 aberturas e gambitos.
- Treinamento com 12 perguntas e explicações.
- Repertório pessoal e anotações guardados no armazenamento local do navegador.
- Links para coleções PGN de dez grandes mestres e tentativa de importação direta da coleção selecionada para o IndexedDB, sem escolher manualmente um arquivo.
- Revisão didática do último lance selecionado, com observações sobre captura, xeque, roque, promoção, desenvolvimento e centro.
- Integração de Stockfish 19 Lite single-threaded via Web Worker e WebAssembly, carregada sob demanda.

## Como estudar partidas dos mestres
1. Abra a seção Grandes mestres.
2. Em “Partidas online”, escolha um dos dez jogadores e toque em “Buscar partidas no aplicativo”.
3. Se a origem permitir acesso direto entre sites (CORS), a coleção é lida pelo navegador e salva na biblioteca local, sem exigir que você baixe e selecione o arquivo.
4. Se o navegador ou o servidor bloquear esse acesso, use o link PGN Mentor do perfil e a importação manual da biblioteca como alternativa.
5. Abra uma partida e clique em qualquer lance do histórico para navegar. A caixa “Revisão do lance selecionado” apresenta uma explicação didática baseada nas características visíveis do movimento.
6. Se quiser, carregue Stockfish e analise a posição atual.

A coleção externa é mantida pelo PGN Mentor e pode mudar. O projeto não copia nem promete conter todas as partidas existentes. A base é uma porta de entrada para importar os jogos que você quiser estudar.

## Limitações conhecidas
- Stockfish é um motor de avaliação, não um tutor conversacional. O uso do motor depende de internet, suporte a WebAssembly e disponibilidade do CDN. O funcionamento precisa ser confirmado no navegador e aparelho de cada usuário.
- A explicação didática do lance é uma inferência baseada no tabuleiro e não prova o que o jogador pensou. Nem todo lance tem um propósito único. A avaliação e a linha principal do Stockfish são ferramentas de apoio, não comentários humanos.
- A importação direta depende do endereço público do arquivo e das permissões CORS do PGN Mentor. Como o projeto é estático, não há servidor próprio para intermediar o acesso; se a origem bloquear, será necessário usar o fluxo manual.
- As aulas são resumos autorais. Os PDFs de Orfeu D'Agostini, Ludek Pachman e Bobby Fischer são referências para estudo; esta versão não contém uma transcrição ou revisão completa de cada capítulo.
- A lista de aberturas é introdutória, não um catálogo exaustivo de todas as variantes, gambitos, armadilhas ou refutações.
- O projeto é uma aplicação web estática; não tem contas, sincronização entre aparelhos, multiplayer ou tutor de IA em nuvem.

## Privacidade
Partidas importadas ficam no IndexedDB do navegador; repertório e anotações ficam no armazenamento local do navegador. Limpar os dados do site pode apagar essas informações. Não importe arquivos pessoais ou dados que não queira manter no aparelho.

## Créditos e licenças
- chess.js: biblioteca de regras de xadrez, distribuída sob licença BSD-2-Clause.
- Stockfish.js 19 Lite: motor de código aberto sob GNU GPL v3. A versão carregada é single-threaded e usa WebAssembly.
- PGN Mentor: fonte externa de coleções PGN disponibilizadas gratuitamente para estudo; consulte a página original para detalhes e condições.

Fontes:
- https://github.com/jhlywa/chess.js
- https://github.com/nmrugg/stockfish.js
- https://www.pgnmentor.com/files.html
