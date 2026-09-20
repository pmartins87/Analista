# ANKI — Sistema de Flashcards do Projeto Analista

Atualizado em: **19/09/2026**

## Objetivo

Transformar conteúdo realmente cobrável, erros do aluno, literalidade normativa e padrões do Cebraspe em flashcards de alta precisão para Anki/AnkiDroid.

O sistema não deve maximizar quantidade de cartões. Deve maximizar **retenção útil para prova** e reduzir o risco de memorizar simplificações, paráfrases perigosas ou conteúdo impreciso.

## Regra de ouro

**Nenhum cartão entra no baralho validado se houver dúvida material sobre a correção da resposta.**

Quando a dúvida não puder ser resolvida de imediato, o conteúdo permanece como candidato/pendência e não deve ser exportado como cartão validado.

## Hierarquia de fontes

### 1. Regimentos, Constituição, leis, resoluções e demais normas

Usar prioritariamente a **fonte oficial vigente**.

Para RICD, RCCN e demais textos normativos:
- preservar a literalidade quando a redação exata puder ser cobrada;
- registrar artigo, parágrafo, inciso, alínea ou dispositivo correspondente;
- não transformar inferência em texto normativo;
- não substituir palavra relevante por sinônimo apenas para “facilitar”;
- distinguir claramente **trecho literal** de explicação;
- conferir vigência e alterações antes de consolidar cartão que dependa da redação atual.

Se um cartão C/E modificar uma palavra da norma, o verso deve explicar **qual elemento torna o item certo ou errado** e apresentar o dispositivo oficial pertinente.

### 2. Questões e padrão Cebraspe

Quando houver questão real relevante:
- priorizar prova e gabarito oficial;
- registrar banca, órgão/prova e ano quando disponíveis;
- estudar a lógica da pegadinha sem transformar uma questão isolada em regra geral;
- se houver anulação, mudança de gabarito ou controvérsia relevante, registrar isso explicitamente.

### 3. Português e matérias interpretativas

Para regras gramaticais, semânticas ou outros pontos com margem interpretativa:
- usar gramáticas, manuais ou fontes técnicas confiáveis;
- sempre que a forma de cobrança da banca for relevante, confrontar com questões reais do Cebraspe;
- registrar divergências relevantes;
- não apresentar heurística como definição;
- não consolidar como absoluta uma regra que dependa de contexto.

Material de curso, inclusive Gran, pode ser fonte de estudo, mas não prevalece sobre fonte oficial nem sobre evidência mais forte.

## Tipos prioritários de cartão

### A. Literalidade normativa

Frente focada em recuperar a redação exata ou um elemento específico da norma.

Exemplos de alvos:
- prazos;
- quóruns;
- competências;
- composição;
- vedações;
- exceções;
- condições;
- hipóteses de cabimento;
- ordem procedimental.

Evitar cartões que peçam a reprodução de parágrafos enormes. Preferir unidades atômicas sem destruir o contexto jurídico.

### B. Certo/Errado no estilo Cebraspe

Construir assertivas plausíveis e próximas do texto correto, especialmente com:
- troca de sujeito competente;
- troca de prazo;
- inversão de regra e exceção;
- uso de “sempre”, “somente”, “necessariamente”;
- substituição lexical que altere o alcance;
- confusão entre institutos próximos.

O objetivo é treinar discriminação fina, não fabricar pegadinhas artificiais ou ambíguas.

### C. Conceito + critério diagnóstico

Usar quando o aluno precisa distinguir conceitos próximos.

O verso deve conter:
1. definição técnica;
2. critério prático de identificação;
3. contraste com o conceito confundível;
4. exemplo curto, quando útil.

### D. Cartão derivado de erro

Erros reais do aluno têm prioridade alta.

O cartão deve atacar a **causa do erro**, não apenas repetir a questão original. Se o erro revelar confusão entre dois conceitos, criar cartão de contraste; se revelar desconhecimento literal, criar cartão normativo; se revelar falso atalho, registrar o critério correto.

## Critérios de qualidade antes da publicação

Um cartão validado deve passar pelos seguintes gates:

### V1 — Fonte
A resposta está sustentada por fonte adequada ao tipo de conteúdo.

### V2 — Precisão
Não há simplificação capaz de produzir erro em prova.

### V3 — Atomicidade
O cartão testa preferencialmente uma unidade de conhecimento por vez.

### V4 — Clareza
Existe uma resposta objetivamente avaliável. Cartões vagos ou com múltiplas respostas defensáveis devem ser reescritos.

### V5 — Valor de prova
O conteúdo é cobrável, recorrente, fonte de erro, exceção importante ou elemento de alta utilidade.

### V6 — Estilo Cebraspe
Quando pertinente, o cartão treina distinções finas e interpretação compatíveis com a banca, sem sacrificar correção técnica.

Somente após V1–V6 o cartão pode ser marcado como **VALIDADO**.

## Estados

- **CANDIDATO** — identificado durante estudo, ainda não verificado.
- **VALIDADO** — passou pelos gates e pode ser exportado.
- **REVISAR** — fonte ou redação mudou, surgiu controvérsia ou o cartão demonstrou ambiguidade.
- **APOSENTADO** — duplicado, desatualizado, inútil ou substituído por cartão melhor.

## Estrutura mínima dos dados

Cada cartão deve poder ser rastreado pelos seguintes campos:

- ID
- Frente
- Verso
- Tipo
- Disciplina
- Assunto
- Fonte
- Dispositivo/questão
- Status
- Tags
- Origem do cartão: aula, leitura, erro, questão, revisão etc.
- Data de validação/revisão

Campos adicionais podem ser incluídos se aumentarem rastreabilidade sem tornar a manutenção pesada.

## Tags sugeridas

Exemplos:
- `ricd`
- `rccn`
- `portugues`
- `cebraspe`
- `literalidade`
- `prazo`
- `competencia`
- `excecao`
- `erro_aluno`
- `pegadinha`
- `revisar_fonte`

## Regras de redação

- Frente curta o suficiente para saber exatamente o que está sendo perguntado.
- Verso completo o suficiente para corrigir o raciocínio.
- Não esconder no enunciado a informação que deveria ser recuperada.
- Não criar cartões apenas porque uma informação apareceu no material.
- Não usar mnemônico como substituto da regra.
- Não inserir explicação especulativa no mesmo plano visual de um trecho literal.
- Quando houver trecho literal, identificá-lo claramente como tal.
- Em cartão C/E, justificar o gabarito; não deixar apenas “Certo” ou “Errado”.

## Controle de duplicatas

Antes de criar novo cartão:
1. procurar cartão sobre o mesmo dispositivo/conceito;
2. se já existir, preferir melhorar o existente;
3. criar outro apenas quando testar uma dimensão cognitivamente diferente e útil.

Exemplo: um cartão sobre o prazo e outro sobre a autoridade competente podem coexistir; três cartões que apenas reformulam a mesma pergunta não.

## Fluxo permanente do projeto

Durante aulas, leitura, correção de questões e conversas:
1. identificar candidatos a cartão;
2. registrar a origem;
3. validar a fonte;
4. aplicar V1–V6;
5. evitar duplicidade;
6. incorporar os validados ao banco mestre;
7. exportar periodicamente em formato compatível com Anki/AnkiDroid;
8. revisar ou aposentar cartões quando a fonte mudar ou surgir erro.

## Regra especial para alterações normativas

Cartões de norma **não são considerados eternos**.

Sempre que houver alteração relevante do RICD, RCCN, Constituição, lei, resolução ou edital:
- localizar cartões afetados;
- comparar com a nova redação;
- atualizar ou aposentar os cartões;
- registrar a revisão.

## Princípio de segurança epistemológica

É melhor deixar de criar um cartão hoje do que memorizar uma informação errada por meses.

O baralho validado deve ser tratado como material de alta confiança.


## Baseline v1 — 20/09/2026

Foi gerado o primeiro baralho pré-edital validado do projeto.

### Arquitetura decidida

Não serão mantidas cópias independentes dos mesmos cartões em um baralho "Estudo" e outro "Revisão".

Motivo: o Anki já mantém, para cada nota/cartão, um histórico de aprendizagem e um agendamento de repetição espaçada. Duplicar a mesma informação em dois baralhos cria dois históricos e pode gerar revisões redundantes.

Estrutura oficial:

- `Analista::Estudo::Português`
- `Analista::Estudo::RICD`
- `Analista::Estudo::RCCN`

A revisão normal é feita pelo próprio agendamento do Anki. Revisões reforçadas devem usar baralho filtrado/tags, sem duplicação de notas.

Consulta-base para revisão direcionada:

`deck:"Analista::Estudo" (tag:erro_aluno OR tag:dificil OR tag:prioridade_1) is:due`

### Conteúdo do baseline

Total: **78 cartões VALIDADO**

- Português: **30**
- RICD: **30**
- RCCN: **18**

O baseline é deliberadamente pequeno e de alta confiança. Não existe meta de "cobrir tudo" antes do edital.

### Critério de seleção pré-edital

Foram priorizados:

1. tópicos historicamente cobrados no cargo/equivalente;
2. temas recorrentes e discriminativos no padrão Cebraspe;
3. RICD e RCCN com alta densidade de prazos, competências, quóruns, exceções e literalidade;
4. erros e dúvidas reais do aluno em Português;
5. conteúdos de baixo arrependimento enquanto o edital específico de Registro e Redação ainda não foi publicado.

### Fonte normativa do baseline

- RICD: **texto oficial vigente da Câmara**, atualizado até a Resolução da Câmara dos Deputados nº 34/2026.
- RCCN: **compilação oficial do Congresso Nacional/Senado** disponível em 2026.
- As apostilas do Gran são material auxiliar e nunca prevalecem sobre a redação oficial vigente.

### Artefato gerado

Pacote: `Analista_Anki_Estudo_v1.zip`

Conteúdo do pacote:
- `Analista_Anki_Estudo_v1.txt` — importação principal;
- arquivos separados por Português, RICD e RCCN;
- `Analista_Anki_Estudo_v1_Auditoria.tsv` — rastreabilidade por ID, disciplina, assunto, prioridade, fonte e referência;
- `LEIA-ME_Anki_Estudo_v1.md`.

O formato principal usa importação textual UTF-8 do Anki, com colunas Frente, Verso, Deck e Tags.

### Gate para expansão

Antes do edital:
- incorporar erros reais do aluno e pontos de alta recorrência;
- evitar crescimento volumétrico por mera cobertura de apostila.

Após publicação do edital:
1. verticalizar o conteúdo;
2. recalcular prioridades por peso/incidência;
3. incluir novas disciplinas confirmadas;
4. auditar todos os cartões normativos afetados por alterações;
5. gerar v2 do baralho.

