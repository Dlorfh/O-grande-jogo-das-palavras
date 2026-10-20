# PRD — O Grande Jogo das Palavras

**Versão:** 0.1  
**Status:** rascunho para validação  
**Data:** 15 de outubro de 2026

## 1. Resumo

Jogo casual de adivinhação semântica em português brasileiro, ambientado em investigações de ocorrências paranormais. A atmosfera toma Ordem Paranormal como referência solicitada, mas o universo, os casos e os textos serão originais e não canônicos. A pessoa digita palavras relacionadas a uma resposta secreta, recebe pistas sobre a relação de significado e pode iniciar partidas sem esperar por uma rodada diária. Registros de rádio, relatos impressos e cadernos de campo dão identidade às partidas. 

O primeiro lançamento será uma experiência web responsiva, gratuita, sem anúncios e sem conta. O progresso será salvo localmente no dispositivo. O mecanismo de similaridade, as regras de cada rodada e a forma da narrativa continuam pendentes de decisão; os percentuais exibidos nos mockups não representam comportamento de produto.

## 2. Problema e oportunidade

Jogos de palavras oferecem uma interação simples de aprender, mas o feedback precisa ser compreensível e parecer justo para que a pessoa queira continuar tentando. A hipótese do produto é que pistas baseadas em significado, combinadas com uma identidade narrativa própria, tornam a descoberta envolvente sem exigir cadastro ou sessões longas.

Essa hipótese ainda precisa ser validada com jogadores. Não há, neste PRD, metas de mercado ou retenção baseadas em pesquisa quantitativa.

## 3. Público e plataforma

- **Público prioritário:** adultos no Brasil que gostam de palavras, curiosidades e jogos casuais.
- **Idioma inicial:** português brasileiro.
- **Plataforma inicial:** web responsiva, com uso por toque e teclado.
- **Modelo de acesso:** gratuito, sem anúncios e sem conta obrigatória.
- **Persistência:** progresso guardado no navegador do dispositivo; sincronização entre dispositivos não faz parte do escopo inicial.

## 4. Objetivos

1. Permitir que uma pessoa comece uma partida sem cadastro ou configuração demorada.
2. Tornar a relação entre palpite e resposta compreensível por meio de feedback semântico.
3. Permitir iniciar novas partidas a qualquer momento.
4. Acrescentar contexto temático ou narrativo sem atrapalhar a ação principal.
5. Funcionar em telas pequenas e ser operável por teclado e tecnologias assistivas.

### Fora do escopo inicial

- Aplicativos nativos para Android ou iOS.
- Login, perfis públicos, sincronização em nuvem ou ranking entre jogadores.
- Anúncios, assinatura, compras ou conteúdo pago.
- Partidas multijogador, chat, conteúdo criado por usuários ou competição em tempo real.
- Um desafio diário obrigatório ou uma mecânica de letras em posições fixas.
- Reprodução de logotipos, personagens, textos, imagens, nomes de organizações ou outros materiais oficiais de franquias existentes.

## 5. Decisões confirmadas e pendentes

| Tema | Confirmado | Ainda precisa de decisão |
| --- | --- | --- |
| Mecânica | Adivinhação por significado, com palpites em palavras | Como medir proximidade e apresentar as pistas |
| Ritmo | Partidas ilimitadas, sem espera por uma nova rodada diária | Se cada partida tem limite de tentativas ou tempo |
| Narrativa | Investigação paranormal original; rádio, relato impresso e caderno são caminhos visuais em protótipo | Capítulos, temas independentes, ambientação ou coleção |
| Plataforma e público | Web responsiva; adultos no Brasil | Navegadores e versões mínimas suportadas |
| Acesso e negócio | Gratuito, sem anúncios e sem conta | Não há modelo comercial adicional definido |
| Dados | Progresso local, sem sincronização definida | Quais dados persistir, por quanto tempo e como exportar/apagar |
| Visual | Três direções estão prototipadas | Qual direção será escolhida ou combinada |
| Vocabulário | Português brasileiro | Fonte, palavras válidas, respostas, acentos, flexões e regionalismos |

**Distinção importante:** “partidas ilimitadas” significa poder começar novas rodadas sem bloqueio diário. Isso não define se uma partida individual permite tentativas ilimitadas.

## 6. Experiência principal

1. A pessoa abre o jogo e encontra uma ação clara para iniciar uma partida.
2. O jogo apresenta uma resposta secreta por meio de um contexto curto, tema ou narrativa.
3. A pessoa envia um palpite como palavra.
4. O jogo registra o palpite e informa, em texto, como ele se relaciona com a resposta. A forma exata desse feedback está pendente.
5. A pessoa pode continuar tentando, consultar eventuais pistas e encerrar a rodada conforme regras que ainda serão definidas.
6. Ao terminar, o jogo apresenta um resultado claro e permite começar outra partida.

O fluxo deve manter o campo de palpite e o feedback fáceis de encontrar. A narrativa não deve exigir leitura longa entre tentativas.

## 7. Requisitos funcionais

Prioridade **P0** indica requisito necessário para o MVP. Regras marcadas como pendentes não devem ser inferidas dos exemplos dos protótipos.

| ID | Prioridade | Requisito |
| --- | --- | --- |
| RF-01 | P0 | A pessoa deve poder iniciar uma partida sem criar conta. |
| RF-02 | P0 | A interface e as instruções do MVP devem estar em português brasileiro. |
| RF-03 | P0 | Deve ser possível iniciar novas partidas sem aguardar uma virada diária. |
| RF-04 | P0 | A pessoa deve poder enviar palpites como palavras e receber feedback relacionado ao significado. O algoritmo, a escala e os textos de feedback são decisões pendentes. |
| RF-05 | P0 | O sistema deve informar quando um palpite estiver vazio, repetido ou fora do vocabulário aceito, depois que essas regras forem definidas. |
| RF-06 | P0 | O jogo deve preservar o progresso local de uma partida ativa ao recarregar a página, quando o armazenamento do navegador estiver disponível. |
| RF-07 | P0 | Deve existir uma ação compreensível para apagar ou reiniciar o progresso local, com prevenção contra remoção acidental. |
| RF-08 | P0 | A partida deve ter um contexto temático ou narrativo curto, sem ocultar a ação de adivinhar. O formato narrativo permanece pendente. |
| RF-09 | P0 | A interface deve comunicar o resultado de cada palpite por texto, não apenas por cor ou posição visual. |
| RF-10 | P0 | A pessoa deve receber uma conclusão clara ao acertar ou ao atingir a condição de encerramento, que ainda será definida. |
| RF-11 | P1 | Após a rodada, o jogo pode apresentar definição, exemplo de uso, curiosidade ou trecho narrativo. Conteúdo e prioridade estão pendentes. |
| RF-12 | P1 | Estatísticas, coleções, conquistas e compartilhamento ficam fora do MVP até confirmação de prioridade. |

## 8. Vocabulário e conteúdo

- O produto deve priorizar palavras compreensíveis para adultos no Brasil e revisar respostas quanto a familiaridade e ambiguidade.
- O VOLP da Academia Brasileira de Letras é uma referência possível para ortografia e formas registradas; não deve ser tratado automaticamente como lista de respostas do jogo.
- A equipe deve definir separadamente o conjunto de palpites aceitos e o conjunto de respostas possíveis.
- Antes de importar, redistribuir ou adaptar bases lexicais, verificar licença e condições de uso.
- Devem ser decididos: acentos e cedilha, flexões, plural, conjugações, nomes próprios, estrangeirismos, regionalismos, gírias, palavras raras e variantes ortográficas.
- Caso a resposta tenha mais de um sentido comum, o contexto ou as pistas devem reduzir a ambiguidade.
- Conteúdo visual, fontes, textos e imagens devem ter origem e direitos de uso verificados antes do lançamento.

## 9. Acessibilidade e usabilidade

Meta proposta para o MVP: WCAG 2.2 nível AA, com validação manual além de checagens automatizadas.

- Todas as ações devem funcionar por teclado, com ordem de foco previsível e indicador de foco visível.
- O campo de palpite deve ter rótulo acessível; mensagens de validação e novos resultados devem ser anunciados por tecnologia assistiva sem interromper a escrita.
- Acerto, erro e proximidade não podem depender apenas da cor; usar texto ou outro sinal perceptível.
- Texto normal deve atender ao contraste mínimo WCAG AA de 4,5:1; controles e limites visuais relevantes devem ser avaliados também.
- A interface deve permanecer utilizável com ampliação de texto, zoom e viewport estreita, sem perda de conteúdo ou rolagem horizontal desnecessária.
- Respeitar `prefers-reduced-motion`; animação não pode ser o único meio de comunicar um estado.
- Mensagens devem usar linguagem direta e explicar o que aconteceu e qual é o próximo passo.

## 10. Requisitos não funcionais

- **Responsividade:** layout funcional em celular, tablet e desktop; validar a partir de 320 px de largura.
- **Persistência:** armazenamento local, sem conta. Se o navegador bloquear ou não oferecer armazenamento, a partida ainda deve poder continuar, com aviso apropriado.
- **Privacidade:** coletar apenas dados necessários ao funcionamento. Não adicionar publicidade ou rastreamento de terceiros ao MVP.
- **Desempenho:** apresentar a interface e permitir um palpite sem espera perceptível; a meta técnica exata deve ser definida quando a arquitetura de feedback for escolhida.
- **Compatibilidade:** definir e testar a matriz de navegadores antes do lançamento.
- **Segurança:** tratar texto digitado como entrada não confiável e não executar conteúdo fornecido pelo jogador.

## 11. Métricas de validação

As métricas abaixo são propostas para pesquisa e não metas já aprovadas:

- proporção de participantes que entende a primeira pista sem explicação externa;
- proporção que conclui uma primeira partida;
- compreensão relatada do motivo pelo qual um palpite foi considerado próximo ou distante;
- partidas iniciadas novamente após a primeira sessão;
- frequência de palavras inválidas, repetidas ou contestadas;
- acessibilidade do fluxo em avaliação por teclado e leitor de tela.

Definir metas numéricas somente após teste inicial com adultos brasileiros. Se forem coletados eventos de uso, documentar a finalidade, minimizar os dados e decidir consentimento, retenção e exclusão antes da implementação.

## 12. Critérios de aceite do MVP

1. Uma pessoa consegue abrir e iniciar uma partida sem login, anúncio ou etapa de compra.
2. É possível enviar um palpite por teclado e por toque, receber retorno textual e continuar a interação.
3. O estado de uma partida em andamento é restaurado após recarregar a mesma página no mesmo navegador, quando o armazenamento local estiver disponível.
4. A pessoa consegue apagar o progresso local e entende que isso remove os dados daquele dispositivo.
5. É possível iniciar outra partida sem esperar por um desafio diário.
6. As regras de validade dos palpites, condição de vitória e fim da rodada estão documentadas antes de liberar conteúdo real.
7. Cor não é o único sinal de estado; foco, mensagens e controles são utilizáveis por teclado.
8. A interface é verificada em celular e desktop, sem sobreposição ou perda de controles.
9. As respostas e pistas usadas no lançamento passam por revisão linguística e de ambiguidade.
10. Nenhuma pontuação ilustrativa dos mockups é apresentada como cálculo real no produto.

## 13. Riscos e mitigação

| Risco | Mitigação proposta |
| --- | --- |
| O feedback semântico parece arbitrário | Testar exemplos com falantes de português brasileiro; explicar a pista em linguagem natural e permitir revisar palavras contestadas. |
| Palavras válidas parecem injustas ou obscuras | Curar respostas por frequência e familiaridade; separar respostas de palpites aceitos. |
| Partidas ilimitadas ficam repetitivas | Planejar variedade de respostas e temas; medir repetição percebida em testes. |
| A narrativa atrasa o jogo | Manter textos curtos e sempre deixar o campo de palpite evidente. |
| O progresso local é perdido | Explicar que o dado fica neste dispositivo; oferecer reinício consciente e não prometer sincronização. |
| Direitos sobre listas, imagens ou referências de terceiros não estão claros | Verificar licença, atribuição e permissão comercial; manter textos, identidade e elementos narrativos originais. |

## 14. Direções visuais em avaliação

Os protótipos são alternativas para teste, não decisões de marca. A ambientação toma Ordem Paranormal como referência tonal, sem reutilizar elementos oficiais ou apresentar o jogo como produto afiliado:

- **Frequência anômala:** transmissão interceptada, contato perdido e tensão de investigação.
- **O folheto interditado:** relato popular impresso, palavra apagada e reconstrução de testemunho.
- **Caderno da ocorrência:** arquivo de campo, registro de evidências e organização de hipóteses.

Avaliar qual direção deixa a mecânica mais clara, é lembrada pelo público e mantém boa legibilidade. É possível combinar elementos, desde que a escolha seja validada.

## 15. Decisões abertas, em ordem de impacto

1. Qual método mede proximidade semântica: ranking, categorias, pistas escritas, ou combinação?
2. Que relação semântica conta como proximidade: sinônimo, associação, contexto de uso ou outra?
3. Qual é a condição de acerto e encerramento? Há limite de palpites, tempo, dicas e revelação da resposta?
4. A narrativa é contínua, episódica ou apenas ambientação? O que muda quando uma palavra é descoberta?
5. Quais palavras podem ser respostas e quais variantes serão aceitas como palpite?
6. Como as partidas ilimitadas escolhem respostas e evitam repetição no histórico local?
7. O que deve ser mostrado ao final: definição, exemplo, curiosidade, progresso ou apenas próxima partida?
8. Qual direção visual será escolhida após teste com usuários?
9. Quais métricas de uso são necessárias e que política de retenção/exclusão se aplica ao progresso local?

## 16. Referências de pesquisa

- [Wordle — New York Times Games](https://www.nytimes.com/games/wordle/index.html): referência de regras de tentativas e tamanho fixo da palavra; não determina as regras deste produto.
- [Wordle: celebração do 1.000º desafio — The New York Times Company](https://www.nytco.com/press/wordle/): relato da própria empresa sobre ritual diário e compartilhamento social.
- [Contexto](https://contexto.me/): comparável de adivinhação semântica com opções diária e ilimitada.
- [Vocabulário Ortográfico — Academia Brasileira de Letras](https://www.academia.org.br/nossa-lingua/vocabulario-ortografico): referência ortográfica do português, com atenção à vertente brasileira.
- [WCAG 2.2: uso de cor](https://www.w3.org/WAI/WCAG22/Understanding/use-of-color.html), [teclado](https://www.w3.org/WAI/WCAG22/Understanding/keyboard.html) e [contraste](https://www.w3.org/WAI/WCAG22/Understanding/contrast-minimum.html): critérios de acessibilidade web.
- [10 heurísticas de usabilidade — Nielsen Norman Group](https://www.nngroup.com/articles/ten-usability-heuristics/): referência para feedback de estado, prevenção de erros e clareza de interface.
