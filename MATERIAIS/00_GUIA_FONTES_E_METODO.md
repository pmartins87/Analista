# Guia canônico de estudo pós-edital

Atualizado em: 03/10/2026

## Função deste arquivo

Este é o mapa de materiais do projeto. A planilha define **quando** estudar. Os cadernos em `MATERIAIS/` definem **o quê** estudar. O banco de questões define **como testar**. O Anki define **como reter**.

O candidato não deve gastar tempo escolhendo livro, aula ou fonte a cada sessão.

## Hierarquia de fontes

1. Edital, retificações e fontes oficiais.
2. Constituição, leis, RICD e RCCN oficiais.
3. Manuais institucionais e documentação técnica oficial.
4. Cadernos do projeto, produzidos a partir dessas fontes e bibliografia consagrada.
5. Gran Cursos, usado seletivamente como explicação complementar e banco de questões.
6. Bibliografia acadêmica, consultada por capítulo/tópico — não lida de capa a capa.
7. Fontes avulsas da internet somente quando resolverem lacuna específica.

## Material diário

Todo dia deve conter cinco componentes dentro da carga prevista:

1. **Revisão inicial (R)** — recuperação ativa + Anki devido.
2. **Núcleo específico (P2)** — principal matéria do dia.
3. **Processo/regimentos** — texto oficial ou processo legislativo.
4. **P1** — Português, Inglês, Administrativo, Constitucional ou TI.
5. **Aplicação** — questões, correção ou discursiva.

A revisão faz parte das horas líquidas. Não é uma tarefa extra.

## Revisão

### Anki
O pós-edital terá um baralho canônico novo, separado de versões anteriores:
`Analista 2027`.

Subbaralhos:
- P2::Linguística
- P2::ASR_Transcrição_IA
- P2::Processo_Regimentos
- P2::Ciência_Política
- P1::Português
- P1::Inglês
- P1::Administrativo
- P1::Constitucional
- P1::TI_Dados_IA
- Discursiva

Regra:
- revisar cartões devidos **todos os dias**;
- novos cartões entram somente de literalidade importante, conceitos de alta incidência, confusões reais e erros;
- preferência por cartões Cebraspe autossuficientes, não cartões escolares do tipo “defina X”;
- verso curto, mas explicativo;
- quando houver erro em questão, criar/ajustar cartão que ataque a causa do erro;
- domingo: revisão devidos e erros da semana; normalmente sem “encher” o baralho de novos cartões.

### Recuperação espaçada além do Anki
O Anki cuida de fatos e distinções. Temas amplos precisam de recuperação:
- D+1: explicar sem consulta por 5–10 min;
- D+7: mini-bateria/questão discursiva ou reconstrução de mapa;
- D+21: revisão por questões e erros.

Isso será embutido nos pacotes diários.

## Questões

A prova Cebraspe usa +1 / -1. Portanto:
- treinar C/E desde o início;
- marcar “certo” somente quando a proposição inteira estiver sustentada;
- não usar regra de chute fixa antes de simulados mostrarem o custo real da incerteza;
- toda questão original criada pelo projeto deve indicar gabarito, fundamento e pegadinha;
- questões oficiais podem ser usadas via Gran ou plataforma do candidato; o projeto não reproduz em massa material protegido.

## Discursiva

Começa na primeira semana, porque vale 60 pontos e cobra conhecimentos específicos:
- 2 questões de até 20 linhas, 15 pontos cada;
- 1 peça técnica de até 50 linhas, 30 pontos.

Treino:
1. primeiro: esqueleto de resposta;
2. depois: resposta em limite de linhas;
3. depois: tempo cronometrado;
4. reta final: prova discursiva completa.

## Fontes canônicas por bloco

### Edital
Cebraspe — página do concurso:
http://www.cebraspe.org.br/concursos/cd_26_analista

### RICD
Câmara — Regimento Interno:
https://www2.camara.leg.br/atividade-legislativa/legislacao/regimento-interno-da-camara-dos-deputados

Recortes exatos do edital:
- **P1 — Direito Constitucional e Regimento — item 7.1:** arts. 1º–24;
- **P1 — item 7.2:** arts. 65–94;
- **P1 — item 7.3:** arts. 226–251;
- **P1 — item 7.4:** arts. 262–273;
- **P2 — Processo Legislativo e Regimentos — item 2.1:** arts. 25–64 e 95–200.

A união prática dos recortes é: arts. 1º–200, 226–251 e 262–273. A união serve para controle global, mas as apostilas devem preservar a identificação de P1/P2 e do item exato do edital.

### RCCN
Senado/Congresso — Regimento Comum:
https://www25.senado.leg.br/web/atividade/legislacao/regimento-interno

Recorte combinado:
- arts. 1–103. O básico exige Título I e Título IV, capítulos II e III, até o art. 103; o específico exige arts. 1–71. A união prática é 1–103.

### Processo legislativo
Câmara — Entenda o processo legislativo:
https://www.camara.leg.br/entenda-o-processo-legislativo/

EVC Câmara:
https://evc.camara.leg.br/material/entenda-o-processo-legislativo/

Constituição Federal, especialmente arts. 44–75 e 59–69:
https://www2.camara.leg.br/atividade-legislativa/legislacao/constituicao1988

### Redação oficial
Manual de Redação da Presidência da República:
https://www.gov.br/pt-br/servicos/consultar-o-manual-de-redacao-da-presidencia-da-republica

LC 95/1998:
https://www.planalto.gov.br/ccivil_03/leis/lcp/lcp95.htm

### ASR, transcrição e IA
Jurafsky & Martin — Speech and Language Processing (3rd ed. online), capítulos de speech recognition/NLP:
https://web.stanford.edu/~jurafsky/slp3/

OpenAI Whisper — README/model card:
https://github.com/openai/whisper
https://github.com/openai/whisper/blob/main/model-card.md

Documentação oficial dos provedores citados no edital:
- Google Cloud Speech-to-Text
- Microsoft Azure AI Speech
- AWS Transcribe

Usar os cadernos do projeto como síntese; documentação dos provedores entra para diferenças de recurso, terminologia e fluxo.

### Administração/Governança
Constituição, Lei 8.112, Lei 9.784, Lei 8.429, Lei 14.133, LAI e LGPD nas versões oficiais do Planalto.

TCU — Referencial Básico de Governança Organizacional:
https://portal.tcu.gov.br/publicacoes-institucionais/cartilha-manual-ou-tutorial/referencial-basico-de-governanca-organizacional

### TI e segurança
CERT.br — Cartilha de Segurança para Internet:
https://cartilha.cert.br/

Microsoft Learn para Office 365/OneDrive/Teams e fundamentos de dados, quando aplicável.

### Ciência Política
TSE — O sistema eleitoral brasileiro: síntese e história:
https://www.tse.jus.br/institucional/catalogo-de-publicacoes/lista-do-catalogo-de-publicacoes/publicacoes/o/o-sistema-eleitoral-brasileiro-2013-2a-edicao

Bibliografia de consulta, não leitura integral:
- Norberto Bobbio, Nicola Matteucci e Gianfranco Pasquino — Dicionário de Política.
- Arend Lijphart — Modelos de Democracia.
- Robert Dahl — Poliarquia / Sobre a Democracia.
- Jairo Nicolau — Sistemas Eleitorais.
- Scott Mainwaring — sistemas partidários e presidencialismo no Brasil, como apoio seletivo.
- José Murilo de Carvalho — cidadania e formação política brasileira, leitura seletiva.

### Linguística/textualidade
Bibliografia de consulta:
- Ferdinand de Saussure — Curso de Linguística Geral.
- Ingedore Koch — Coesão Textual; Desvendando os Segredos do Texto.
- Luiz Antônio Marcuschi — Produção Textual, Análise de Gêneros e Compreensão; Da Fala para a Escrita.
- José Luiz Fiorin — Introdução à Linguística / Elementos de Análise do Discurso, conforme o tópico.
- Mikhail Bakhtin — Estética da Criação Verbal, especialmente gêneros do discurso.
- Evanildo Bechara — Moderna Gramática Portuguesa.
- Cunha & Cintra — Nova Gramática do Português Contemporâneo.

Não ler essas obras integralmente antes da prova. Os cadernos indicam o conceito-alvo e a obra serve para resolver dúvida ou aprofundar ponto vermelho.

## Gran Cursos

Usar seletivamente. O Gran não é fonte de verdade do cronograma.

Materiais já disponíveis no projeto:
- Português: PDFs de sintaxe simples/composta, classes, concordância/regência/crase/pontuação, coesão/semântica/reescrita, interpretação, gêneros e cadernos de questões Cebraspe.
- RICD: PDFs de disposições preliminares/estrutura e sessões/exercício do mandato.
- RCCN: PDF de Regimento Comum.

Quando o Gran publicar material pós-edital:
- usar se cobrir exatamente o item do edital;
- não esperar o Gran para iniciar;
- não assistir linearmente por obrigação;
- usar aula/PDF quando o caderno do projeto ou a fonte oficial não forem suficientes.

## Cadernos canônicos

- `01_P2_LINGUISTICA_TEXTO_REDACAO.md`
- `02_P2_ASR_TRANSCRICAO_IA.md`
- `03_P2_PROCESSO_REGIMENTOS.md`
- `04_P2_CIENCIA_POLITICA.md`
- `05_P1_PORTUGUES_INGLES.md`
- `06_P1_ADMIN_CONST_TI.md`
- `07_DISCURSIVA_PECA_TECNICA.md`
- `08_BANCO_QUESTOES_CEBRASPE_STYLE.md`
- `09_ANKI_POS_EDITAL.md`
- `PACOTES_DIARIOS.md`

## Critério de encerramento de uma sessão

Uma sessão só está “feita” quando:
- o conteúdo-alvo foi visto;
- o aluno consegue recuperar a regra/estrutura central sem olhar;
- houve aplicação (questão, exemplo, mapa ou escrita);
- erros relevantes foram registrados ou convertidos em cartão;
- o checkbox `Feito?` foi marcado na planilha.


## Padrão canônico das 106 apostilas diárias — decisão de 03/10/2026

As apostilas A001–A106 são a unidade diária de estudo. O mapa dos 106 dias deve permanecer previamente definido; a redação detalhada de cada apostila pode ser produzida progressivamente, incorporando desempenho e erros reais sem improvisar a cobertura global.

### Regra pedagógica obrigatória

Apostila diária não pode ser mero roteiro nem lista de conceitos. Deve ser material autossuficiente para a sessão, com ciclo recorrente **teoria → exemplo concreto → questão → correção/fundamento**, repetido ao longo do conteúdo. Instruções vagas como “estudar X pelo ChatGPT” não satisfazem o padrão.

Para cada conceito novo:
1. explicar em linguagem precisa e concreta, evitando definições circulares ou que apenas troquem um termo desconhecido por outros;
2. apresentar pelo menos um exemplo e, quando houver confusão provável, um contraexemplo/contraste;
3. identificar a fonte conceitual ou normativa usada e permitir rastreabilidade para aprofundamento;
4. inserir aplicação imediata em questão, preferencialmente **questão oficial Cebraspe/Cespe pertinente**, com identificação da prova/ano quando disponível;
5. quando não houver questão oficial adequada, usar questão autoral explicitamente rotulada **CEBRASPE-style**, nunca apresentada como oficial;
6. comentar o gabarito pelo fundamento e pela pegadinha, não apenas indicar C/E.

### Densidade de questões

Resolver o máximo de questões úteis durante os 106 dias é objetivo explícito. Questões não devem ficar concentradas apenas em um bloco final: devem aparecer intercaladas com a teoria (“assunto → questão → assunto → questão”), além das baterias, revisões e simulados programados. Priorizar questões oficiais Cebraspe do mesmo tema e nível; usar questões autorais para preencher lacunas ou testar distinções específicas.

### Fontes e confiança

Toda apostila deve terminar com seção **Fontes desta apostila**, discriminando, por bloco, as fontes efetivamente utilizadas. Em regimentos/leis, prevalece a fonte oficial e a literalidade. Em Linguística/Português, usar bibliografia consagrada indicada neste guia e provas oficiais Cebraspe; materiais do Gran podem complementar explicação e questões, sem substituir fonte oficial quando houver. Afirmações cuja formulação varie por corrente teórica devem indicar o enquadramento (por exemplo, “na formulação saussuriana”).

### Aderência obrigatória ao edital verticalizado — regra vinculante de 03/10/2026

O **Edital nº 1/2026 e eventuais retificações** definem o universo de conteúdo. A aba **Edital Verticalizado** da planilha operacional é a tradução de controle desse universo e deve ser conferida antes de redigir ou liberar cada apostila.

Regras obrigatórias para A001–A106:
1. nenhum bloco de estudo entra na apostila sem estar vinculado a **prova (P1/P2/P3), disciplina e item/subitem exato do edital**;
2. o início da apostila deve trazer um **Mapa do edital coberto no dia**, com a numeração exata;
3. ao terminar cada tópico de estudo, registrar de forma explícita: **“COM ISSO, VIMOS: [prova] — [disciplina] — item [número] — [tópico]”**;
4. quando a sessão cobrir apenas parte de um item, registrar **COBERTURA PARCIAL**, especificar exatamente o trecho estudado e o que permanece pendente; item parcial não pode ser marcado como integralmente estudado;
5. conceitos auxiliares podem ser explicados apenas quando necessários para compreender/resolver o item do edital e devem ser tratados como apoio, não como novo conteúdo programático;
6. toda questão autoral deve trazer a indicação do item do edital testado; questões oficiais devem ser vinculadas ao mesmo item quando inseridas;
7. antes de liberar a apostila, cruzar seu índice com a aba **Edital Verticalizado**. Se não houver correspondência justificável com um item do edital, o conteúdo deve ser removido da unidade diária;
8. em caso de conflito entre plano anterior, apostila, curso, memória ou resumo e o edital vigente, **o edital vigente prevalece**.

Exemplo vinculante para RICD: arts. 1º–24 pertencem a **P1, item 7.1**; arts. 25–64 e 95–200 pertencem a **P2, item 2.1**. Não fundir esses recortes ao indicar o que foi efetivamente estudado, mesmo que a união prática seja usada para controle global.

Ao usar o arquivo oficial da Resolução nº 17/1989, distinguir a **Resolução que aprova o Regimento** de seu **texto anexo (RICD)**. Os arts. 1º–8º iniciais da Resolução não se confundem com os arts. 1º–8º do RICD. Quando o edital indicar “RICD: arts. ...”, estudar os artigos do texto regimental anexo, salvo menção expressa do edital à parte preambular da Resolução.

### Resumo estratégico obrigatório em blocos normativos — decisão de 03/10/2026

Depois da leitura literal de cada bloco de RICD, RCCN, Constituição, lei ou resolução, a própria apostila deve trazer um **resumo estratégico pós-leitura**. O resumo serve como compressão para revisão; não substitui a fonte oficial e não amplia o edital.

Quando houver remissões, o resumo deve ser seguido de um **Mapa de Remissões Resolvidas** com, no mínimo:
- dispositivo de origem;
- dispositivo/norma de destino;
- conteúdo referenciado em síntese fiel;
- resultado semântico da combinação;
- pegadinha ou forma plausível de cobrança Cebraspe, quando relevante;
- identificação **APOIO — REMISSÃO** quando o destino não for conteúdo autônomo do edital.

O objetivo é permitir que, depois da primeira leitura da fonte, o candidato revise pela apostila sem ter de abrir em sequência diversos artigos e diplomas apenas para reconstruir referências cruzadas. A unidade a memorizar não é só o número do artigo remetido, mas a **regra normativa completa resultante da remissão**.

Esse padrão é obrigatório da A001 à A106 sempre que houver conteúdo normativo com remissões.

### Regra de remissões normativas no RICD/RCCN — decisão de 03/10/2026

Remissão expressa no texto normativo não será estudada apenas como número de artigo. Para fins de prova Cebraspe, deve-se distinguir **texto de remissão** e **regra resolvida**.

Procedimento:
1. quando um dispositivo do RICD remeter a outro dispositivo do próprio RICD que esteja no edital, abrir a referência e estudar a consequência normativa completa que foi incorporada;
2. quando a remissão for à Constituição ou a outra norma que também esteja no edital, resolver a referência e integrar os dois textos;
3. quando a remissão for a norma/dispositivo externo que não constitua conteúdo autônomo do edital, estudar somente o fragmento indispensável para compreender a regra do RICD, rotulado **APOIO — remissão**, sem criar checkbox de cobertura externo;
4. em questões e Anki, treinar tanto a formulação literal (“nos termos do art. X”) quanto a formulação **desreferenciada**, em que a banca substitui o número do artigo pelo conteúdo efetivo do dispositivo referido;
5. registrar remissões com alta capacidade de alterar competência, sujeito, prazo, quórum, prerrogativa, condição ou exceção como pontos de alta prioridade.

Evidência Cebraspe: Câmara/Analista/Técnica Legislativa/2012, item 104, cobrou diretamente uma prerrogativa do Líder do Governo. O art. 11 do RICD não reproduzia a prerrogativa; remetia aos incisos I, III e IV do art. 10. A banca apresentou no item o conteúdo do art. 10, III (“participar... dos trabalhos de qualquer Comissão... sem direito a voto”), demonstrando que uma remissão interna pode ser cobrada já **resolvida**.

Aplicações prioritárias no recorte inicial:
- art. 9º → CF, art. 17, § 3º: requisito para existência de Liderança partidária;
- art. 10, I → arts. 66, §§ 1º e 3º, e 89 do RICD: uso da palavra/Comunicações de Liderança;
- art. 10, V → art. 8º, III: registro/documentação dos candidatos à Mesa;
- art. 11 e art. 11-A → art. 10, I, III e IV: prerrogativas das Lideranças do Governo e da Minoria;
- art. 15, II → CF, art. 57, § 5º: constituição da Mesa do Congresso Nacional.

Não é necessário transformar toda remissão em estudo ilimitado da norma externa. A unidade mínima de estudo é a **regra importada pela remissão**, preservado o recorte do edital.

### Gate de qualidade antes de liberar uma apostila

Não liberar como pronta se houver: conceito abstrato sem exemplo; definição circular; seção sem fonte rastreável; questão autoral não rotulada; conteúdo regimental sem conferência oficial; bloco teórico relevante sem aplicação; tópico sem prova/disciplina/item exato do edital; encerramento de tópico sem registro do item coberto; cobertura parcial apresentada como integral; ou divergência com o edital verticalizado/mapa A001–A106 sem justificativa.

### Correção da A001

A versão inicial da A001 (03/10/2026) foi considerada abaixo deste padrão, especialmente no item 2.7 (referente, referência, representação e sentido) e pela baixa integração de questões com a teoria. Deve ser revisada integralmente segundo este padrão; a falha é tratada como correção metodológica para A001–A106, não como exceção pontual.
