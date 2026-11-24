# Chess Master AI — plano de desenvolvimento

Este repositório está sendo desenvolvido como uma plataforma de estudo de xadrez, não apenas como um jogo.

## Requisitos do projeto

### 1. Regras e tabuleiro
- Movimentos legais de todas as peças.
- Roque, en passant, promoção com escolha da peça, xeque, xeque-mate, afogamento e empates.
- Histórico de lances, desfazer/refazer, virar tabuleiro, importar/exportar PGN e FEN.
- Partidas locais contra outra pessoa e, em etapa posterior, contra motor.

### 2. Enciclopédia de xadrez
- Regras e movimentos de peças.
- Táticas: garfo, cravada, espeto, ataque descoberto, desvio, sobrecarga, atração, interferência, bloqueio, remoção do defensor, ataques duplos e padrões de mate.
- Estratégia: centro, desenvolvimento, espaço, estrutura de peões, casas fortes/fracas, colunas e diagonais, peças boas/ruins, iniciativa, profilaxia, planos de ataque e defesa.
- Aberturas, defesas, sistemas, linhas principais, variantes, gambitos, armadilhas, respostas e refutações.
- Finais de peões, torres, peças menores e damas.
- Tutoriais passo a passo, tabuleiros demonstrativos e exercícios com explicações.

### 3. Partidas e grandes mestres
Jogadores solicitados: Magnus Carlsen, Hikaru Nakamura, Garry Kasparov, Bobby Fischer, Emanuel Lasker, José Raúl Capablanca, Anatoly Karpov, Mikhail Tal, Paul Morphy e Fabiano Caruana.

Cada partida incluída deverá ter, quando houver dados confiáveis: PGN, reprodução lance a lance, contexto, plano, ameaças, alternativas, momentos críticos, erros e revisão. Não afirmar que o banco contém literalmente todas as partidas já disputadas; ampliar com coleções PGN verificadas e respeitar as licenças das fontes.

### 4. Livros enviados pelo usuário
- *Xadrez Básico* — Orfeu Gilberto D'Agostini.
- *Estratégia Moderna do Xadrez* — Ludek Pachman.
- *Minhas 60 Melhores Partidas* — Bobby Fischer.

Usar os livros como fontes de estudo. Criar explicações originais, resumos, exercícios e posições próprias, mantendo fidelidade ao que cada obra realmente ensina. Não reproduzir integralmente os livros nem transcrever grandes trechos protegidos. O conteúdo integral de cada PDF precisa ser conferido antes de afirmar que todos os capítulos foram cobertos.

Também foi solicitado *Meus Grandes Predecessores I–V*, de Garry Kasparov; esses volumes não fazem parte dos três PDFs inicialmente enviados.

### 5. Motor e análise
- Integrar Stockfish por uma distribuição web/WASM apropriada e licenciada.
- Mostrar avaliação, melhor lance e variantes com profundidade configurável.
- Comparar lance jogado com sugestão do motor.
- Distinguir avaliação do motor de explicação pedagógica: a explicação não deve inventar intenção psicológica do jogador.

### 6. Professor e progresso
- Tutor que explique conceitos e posições em linguagem adequada ao nível.
- Treinos de tática, cálculo, estratégia e finais.
- Repertório, anotações, histórico e progresso salvos localmente.
- Recursos de IA externos somente quando houver integração real configurada; não simular IA.

## Critérios de qualidade
- Interface responsiva em celular e computador, acessível e em português.
- Não exibir controles sem funcionamento.
- Tratar falhas de rede, carregamento de bibliotecas e PGNs inválidos.
- Testar regras especiais, importação/exportação, motor e navegação antes de marcar recursos como concluídos.
- Manter o site publicado pelo GitHub Pages.

## Estado inicial
O arquivo inicial `index.html` é um protótipo simples. Ele ainda não contém Stockfish, banco amplo de partidas, comentários completos, tutor de IA nem a enciclopédia solicitada. Este documento registra o escopo; não significa que esses recursos já estejam implementados.
