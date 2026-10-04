# A001 — Registro pós-estudo e Anki

Data: 03/10/2026  
Status: **APOSTILA CONCLUÍDA; BASE ANKI CRIADA; D+1 PENDENTE**

## Cobertura
- P2 Linguística item 1 — concluído.
- P1 Português itens 1 e 2 — concluídos.
- P1 Constitucional/Regimento item 7.1 — parcial: RICD 1º–15 concluídos; 16–24 pendentes.

## Questões
Resultado válido do caderno extraordinário: **44 itens (R17 e R24 excluídos), 43 acertos, 1 erro, líquido 42/44**. Erro real: item 42, sinonímia contextual (`mais ou menos` x `comedidamente`).

A versão estudada da A001 continha 12 itens autorais. Resultado informado: **12/12**, com percepção de dificuldade muito baixa e tempo muito inferior ao previsto.

Após o feedback:
- a A001 foi recalibrada para bateria mista de 20 itens;
- foram inseridas questões oficiais completas de Português e RICD;
- Linguística recebeu itens inéditos mais exigentes;
- resolução e correção passaram a ter tempos separados;
- a bateria nova será executada na D+1 da A002, sem reabrir a conclusão da A001.

## Anki — artefatos existentes
Foram criados **16 cartões-base**, separados por matéria:
- `A001_P1_Portugues.tsv` — 3 cartões;
- `A001_P2_Linguistica.tsv` — 5 cartões;
- `A001_P1_Constitucional_Regimentos.tsv` — 8 cartões.

Índice: [A001_INDEX.md](A001_INDEX.md)

A seleção usou aderência ao edital, padrões Cebraspe, regra vigente e potencial discriminativo. O cartão sobre composição da Mesa registra expressamente: art. 14, §1º = Presidente + 2 Vice-Presidentes + 4 Secretários; os 4 Suplentes são previstos separadamente no §2º.

A002 poderá acrescentar cartões apenas se surgirem erros reais ou acertos com dúvida. **Não existe quota mínima de cartões por apostila.**

Nenhum arquivo foi sincronizado automaticamente com Anki/AnkiDroid.

## Correção de consistência do PDF canônico — 03/10/2026

Foi detectada uma frase residual do **primeiro pacote provisório** incorporado ao PDF consolidado: **16 cartões = 9 RICD + 7 Linguística**. Essa composição deixou de ser válida após a auditoria final da A001, que redistribuiu a seleção entre as três matérias estudadas.

No momento em que a divergência foi identificada, o índice canônico registrava **15 cartões = 3 Português + 8 Constitucional/Regimentos + 4 Linguística**. Em seguida, após a correção do caderno, o erro real do item 42 (`mais ou menos` x `comedidamente`) foi incorporado ao Anki de Linguística. A base canônica atual passou a ser:
- P1 Português — **3**;
- P1 Constitucional/Regimentos — **8**;
- P2 Linguística — **5**;
- total atual — **16 cartões-base**.

O número **16 atual não é o mesmo pacote antigo 9+7**: é a base auditada 3+8+5, já com o cartão `erro_real`.

Para impedir nova divergência, o PDF canônico da A001 deixou de exibir quantidade fixa de cartões e passou a remeter à planilha para a **contagem vigente**. O link/ID do PDF permaneceu o mesmo e a paginação não foi alterada. A planilha e `A001_INDEX.md` são a referência operacional para o Anki vivo.

## Pacote único APKG — 03/10/2026

Foi criado `anki/A001_Anki_16_cartoes.apkg` com os **16 cartões canônicos atuais**, distribuídos em:
- `Analista::P1::Português` — 3;
- `Analista::P1::Constitucional_Regimentos` — 8;
- `Analista::P2::Linguística` — 5.

O APKG passou por auditoria estrutural: arquivo reconhecido como pacote Anki, coleção SQLite íntegra, **16 notas e 16 cartões**, sem mídia externa. Os TSVs continuam preservados como fonte auditável e contingência.

A criação do pacote **não equivale a importação nem sincronização** no Anki/AnkiDroid do candidato.

## Correção de compatibilidade AnkiDroid — 03/10/2026

O primeiro `.apkg` gerado manualmente falhou no AnkiDroid com `500: JsonError { info: "decoding decks: JsonError" }`. A causa foi identificada no schema legado da coleção: os objetos de baralho estavam sem os campos obrigatórios de contadores diários (`lrnToday`, `revToday`, `newToday`, `timeToday`).

O pacote `A001_Anki_16_cartoes.apkg` foi regenerado no mesmo caminho do GitHub, com esses campos incluídos. A coleção continua com **16 notas e 16 cartões**, SQLite íntegro. O link da planilha não mudou.

## Reabertura do Anki A001 para expansão — 04/10/2026

A base de 16 cartões foi considerada **subdimensionada** para o uso pretendido. A A001 permanece concluída como estudo, mas seu artefato Anki será expandido sob a nova política de alta densidade.

Direção:
- ampliar fortemente RICD 1–15, cobrindo unidades semânticas testáveis, exceções, competências, prazos, composições, vacâncias e remissões resolvidas;
- ampliar Linguística com teoria e contrastes, não apenas itens derivados de questões;
- Português recebe cartões somente para mecanismos reutilizáveis e erros relevantes;
- preservar os cartões atuais úteis, inclusive o `erro_real` da Q42.
- usar a Q42 como semente: manter o cartão específico `mais ou menos` x `comedidamente` e acrescentar cartões de mesma estrutura, priorizando questões oficiais Cebraspe/Cespe de nível comparável sobre sinonímia contextual, substituição lexical e mudança de sentido.
- em cartões derivados de questão oficial, usar o trecho mínimo autossuficiente que preserve a decisão do item, em vez de carregar texto desnecessário.

A expansão do Anki **não reabre a cobertura da apostila nem altera o status do Edital Verticalizado**; altera apenas o instrumento de retenção.

## Substituição concluída — base densa A001 — 04/10/2026

A base provisória de 16 cartões foi substituída pelo pacote canônico `A001_Anki_DENSO.apkg`.

Composição atual:
- P1 Português — **9**;
- P1 Constitucional/Regimentos — **122**;
- P2 Linguística — **24**;
- total — **155 cartões**.

Critério: alta densidade para RICD 1–15, com cartões de literalidade, competência, prazo, quórum, condição, exceção, composição, vacância, remissões e inversões plausíveis de Cebraspe; Linguística foi ampliada com teoria e contrastes; Português ficou concentrado em mecanismos transferíveis e questões/erros de alto valor.

O cartão `erro_real` da Q42 foi preservado. A expansão também incluiu cartões vizinhos do mesmo mecanismo sem apagar o erro original.

QA do APKG:
- SQLite `integrity_check = ok`;
- **155 notas / 155 cartões**;
- **0 frentes duplicadas**;
- **0 GUIDs duplicados**;
- sem mídia externa;
- 16 cartões anteriores preservados com seus identificadores internos para minimizar duplicação em importação incremental;
- schema de decks mantém os campos necessários ao AnkiDroid que corrigiram o erro anterior de `decoding decks`.

Os TSVs antigos de 16 cartões ficam apenas como histórico e não são a base de importação atual. Nenhuma sincronização com Anki/AnkiDroid foi alegada ou realizada.

## Lições permanentes
- Anki fora da apostila;
- candidato não redige cartões;
- não selecionar cartão apenas por conter prazo/número/competência;
- registrar todos os artefatos e links na planilha;
- só marcar `Anki?` na verticalização quando o material correspondente tiver sido efetivamente incorporado/revisado conforme o controle do projeto.
