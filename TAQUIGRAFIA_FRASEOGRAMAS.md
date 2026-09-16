# Taquigrafia — vocabulário e fraseogramas de alto rendimento

Atualizado em: **16/09/2026**

## Objetivo

Construir uma biblioteca pequena e progressiva de abreviações/fraseogramas para o Método Oscar Leite Alves, priorizando formas que realmente reduzam o custo gráfico em ditados parlamentares.

Este documento **não altera a decisão estratégica do projeto**: a prova prática de taquigrafia da Câmara 2026 ainda não está confirmada. A trilha funciona como hedge pré-edital e deve ser recalibrada assim que o edital for publicado.

## Evidência de que linguagem parlamentar é o corpus correto

- Câmara 2012: prova prática manual com método de livre escolha; dois ditados de 5 min, a aproximadamente 105 e 110 palavras por minuto.
- Senado 2023: apanhamento de **pronunciamento parlamentar contemporâneo**, 80 palavras por minuto, 5 min; o texto era sorteado entre quatro gravações.

Logo, discursos parlamentares reais são uma aproximação muito melhor do domínio da prova do que textos genéricos.

## Evidência quantitativa disponível

Corpus aberto de 555 documentos da Câmara, sessão do impeachment de abril de 2016, após remoção de stopwords e parte do ruído:

| termo | ocorrências |
|---|---:|
| sr | 1.629 |
| voto | 1.054 |
| presidente | 806 |
| deputado | 598 |
| votos | 528 |
| Brasil | 456 |
| país | 279 |
| impeachment | 234 |
| plenário | 202 |
| democracia | 177 |
| brasileiro | 161 |
| deputados | 159 |
| partido | 141 |
| respeito | 138 |
| governo | 119 |
| Casa | 118 |
| processo | 114 |
| Constituição | 110 |
| responsabilidade | 104 |
| federal | 88 |
| República | 76 |

### Interpretação correta

A frequência bruta **não basta**. O mesmo corpus mostra termos altamente dependentes do assunto (por exemplo, “impeachment”). Um sinal especial só é bom investimento quando combina:

1. alta frequência;
2. estabilidade entre diferentes temas e oradores;
3. economia gráfica relevante;
4. baixa chance de colisão/ambiguidade;
5. recuperação automática na tradução.

Direções editoriais, nomes próprios, siglas partidárias e vocabulário de uma pauta específica não devem dominar a biblioteca.

## Princípio central: fraseogramas pagam mais que palavras isoladas

Uma forma especial para uma palavra já curta pode economizar pouco. Um único gesto seguro para duas, três ou quatro palavras pode eliminar vários movimentos e, principalmente, impedir atraso acumulado durante o ditado.

### P0 — não reinventar o que Leite Alves já abrevia

Material do método já apresenta abreviações para expressões como:

- sem dúvida;
- à medida que;
- a respeito de / da / do;
- ao mesmo tempo;
- ao passo que;
- tanto quanto;
- todas as vezes.

Essas formas devem ser aprendidas na versão canônica antes de criar alternativas pessoais.

## Fraseogramas funcionais/discursivos — foco principal

O Método Maron é útil aqui como fonte de candidatos. Sua lista ampliada afirma explicitamente que **a frequência de uso mostra a conveniência da criação de um novo taquigrama** e contém muitas expressões funcionais recorrentes. Isso não significa copiar a forma gráfica Maron para o Leite Alves; significa usar a existência do taquigrama Maron como evidência de que a expressão merece ser testada para um equivalente compatível com Leite Alves.

### Tier S — prioridade máxima

Expressões com forte combinação de frequência provável, estabilidade temática e economia gráfica:

1. **de acordo com** — já possui taquigrama no Maron.
2. **em relação a** — Maron.
3. **a respeito de / da / do** — já existe no Leite Alves e também no Maron.
4. **ao mesmo tempo** — já existe no Leite Alves e no Maron.
5. **por outro lado** — Maron.
6. **no entanto** — Maron.
7. **além disso** — Maron.
8. **ou seja** — Maron.
9. **por exemplo** — Maron.
10. **no que diz respeito** — Maron; quatro palavras comprimidas, ROI gráfico muito alto.
11. **no que se refere** — Maron; quatro palavras, ROI alto.
12. **na medida em que** — Maron; quatro palavras, ROI alto.

### Tier A — muito fortes

13. **à medida que** — já existe no Leite Alves.
14. **ao passo que** — já existe no Leite Alves.
15. **em outras palavras** — Maron.
16. **de modo que** — Maron.
17. **de maneira que** — Maron.
18. **em decorrência de** — Maron.
19. **por intermédio de** — Maron.
20. **razão pela qual** — Maron.
21. **a fim de** — Maron; o próprio manual mostra que o taquigrama é formado pela junção dos sinais que normalmente ficariam separados.
22. **bem como** — Maron.
23. **apesar de** — Maron.
24. **por isso / por isso mesmo** — Maron.
25. **por conseguinte** — Maron.

### Tier B — úteis, mas só depois dos tiers S/A

- pelo menos;
- pelo contrário;
- por esta razão;
- de qualquer modo;
- de qualquer maneira;
- desta maneira;
- do mesmo modo como;
- em contrapartida;
- em geral;
- em primeiro lugar;
- em segundo lugar;
- em seguida;
- na realidade;
- na verdade;
- nessas condições;
- nesse sentido;
- neste sentido;
- neste momento;
- no momento em que;
- no que concerne;
- cada vez mais;
- cada vez menos;
- mais uma vez;
- muitas vezes;
- poucas vezes;
- se não me engano;
- seja qual for;
- tanto quanto;
- todas as vezes.

## Candidatos personalizados ainda não encontrados nas listas verificadas

São expressões muito promissoras no português formal/parlamentar, mas nesta rodada não foram localizadas como fraseogramas nas listas Leite Alves e Maron consultadas. Precisam de validação por corpus antes de ganhar símbolo permanente:

- **a partir de**;
- **por meio de**;
- **no sentido de**;
- **tendo em vista**;
- **uma vez que**;
- **com base em**;
- **em função de**;
- **em virtude de**;
- **em razão de**;
- **diante de**;
- **de forma que**;
- **por sua vez**;
- **em nome de**.

A ausência numa lista não significa que não exista em outra edição ou sistema; significa apenas “não confirmado nas fontes verificadas até aqui”.

## Regra de desenho no Leite Alves

Para cada expressão promovida:

1. Preferir **junção/redução de sinais já conhecidos** a um desenho totalmente arbitrário.
2. Tentar preservar uma pista fonética ou visual da expressão.
3. Buscar um único movimento ou o menor número possível de mudanças de direção.
4. Evitar levantar a caneta quando isso não trouxer clareza.
5. Não reutilizar forma que possa colidir com palavra/abreviação já existente.
6. Se o fraseograma exigir reflexão para ser lembrado, ele ainda não está pronto para uso em ditado.

## P1 — candidatos parlamentares institucionais

Primeiro lote institucional recomendado para validação prática:

1. Sr. Presidente / Sra. Presidente
2. Vossa Excelência (V. Exa.)
3. Câmara dos Deputados
4. Congresso Nacional
5. projeto de lei
6. Constituição Federal
7. Governo Federal
8. Presidente da República
9. ordem do dia
10. pela ordem
11. questão de ordem
12. com a palavra
13. uso da palavra
14. nesta Casa / desta Casa
15. povo brasileiro

Para uma prova da Câmara, “Câmara dos Deputados” deve preceder “Senado Federal” na prioridade. “Senado Federal” continua útil como vocabulário institucional e em discursos sobre o Congresso.

### P2 — famílias temáticas de alto reaproveitamento

Validar depois do P1:

- políticas públicas;
- serviço público;
- recursos públicos;
- segurança pública;
- saúde pública;
- educação pública;
- administração pública;
- direitos humanos;
- desenvolvimento econômico;
- responsabilidade fiscal;
- interesse público;
- interesse nacional;
- sociedade brasileira;
- Estado brasileiro;
- Poder Executivo / Legislativo / Judiciário;
- Supremo Tribunal Federal;
- Ministério Público.

## Palavras isoladas que merecem monitoramento

Presidente, deputado/deputada, parlamentar, governo, federal, nacional, plenário, comissão, projeto, proposta, Constituição, legislação, processo, democracia, Brasil/brasileiro, responsabilidade, desenvolvimento, administração, segurança, educação, saúde, orçamento e recursos.

**Regra:** antes de inventar uma forma integral própria, verificar se as terminações e simplificações normais do Leite Alves já tornam a palavra suficientemente rápida. Palavras como “responsabilidade”, “administração” e “desenvolvimento” podem obter boa economia pelas terminações do método.

## Famílias modulares preferíveis a dezenas de sinais independentes

Sempre que possível, construir uma lógica reutilizável:

- raiz/sinal de PRESIDENTE + variante de tratamento;
- raiz FEDERAL combinável com Governo, Constituição, Senado etc.;
- raiz PÚBLICO/PÚBLICA combinável com serviço, políticas, recursos, saúde etc.;
- raiz BRASIL combinável com brasileiro/brasileira(s), se o método permitir de forma clara.

Objetivo: reduzir custo de memória e evitar uma biblioteca caótica.

## Score de promoção de um novo fraseograma

Avaliar cada candidato por:

**Utilidade = frequência × economia gráfica × estabilidade temática × clareza / (risco de colisão + custo de memorização)**

Não precisa haver cálculo numérico exato; a fórmula define os critérios de decisão.

## Gate TQ-F1 — biblioteca inicial

Status: **EM EXECUÇÃO**

- aprender primeiro as abreviações canônicas do Leite Alves;
- testar no máximo 10 novos fraseogramas por lote;
- manter biblioteca personalizada inicial limitada a aproximadamente 30–50 formas;
- não ampliar enquanto as atuais não forem reconhecidas e produzidas automaticamente.

### Promoção

Um fraseograma personalizado entra no repertório permanente se:

- reaparecer em vários textos/oradores, não apenas numa pauta;
- gerar economia perceptível de escrita;
- puder ser lido de volta sem depender de adivinhação;
- não colidir com sinal já existente.

### Rejeição/aposentadoria

Descartar ou redesenhar se:

- for temático demais;
- aparecer raramente em diferentes ditados;
- causar hesitação suficiente para anular a economia;
- produzir confusão recorrente na tradução.

## Próxima análise necessária

O ideal é formar um corpus diretamente dos ditados usados no treino e calcular:

- unigramas (palavras);
- bigramas, trigramas e quadrigramas;
- frequência por 1.000 palavras;
- dispersão: em quantos ditados diferentes a expressão aparece;
- ganho potencial estimado;
- ranking final para criação de fraseogramas.

A dispersão é crucial: uma expressão que aparece 20 vezes num único texto é menos valiosa do que outra que aparece 10 vezes distribuída por 8 ditados.

## Fontes

- Câmara dos Deputados, concurso 2012 — prova prática de Taquígrafo Legislativo: https://www2.camara.leg.br/transparencia/recursos-humanos/concursos/concursos-novos-1/g2-edital-no-10
- Senado Federal, concurso 2022/2023 — prova prática de taquigrafia: https://www12.senado.leg.br/transparencia/hotsite-concurso/arquivos/edital_02_prova_pratica_taquigrafia.pdf
- Corpus e processamento de discursos da Câmara: https://bookdown.org/davi_moreira/txt4cs/processamento.html
- PoliS — corpus de discursos da Câmara: https://github.com/dcaled/polis
- Ulysses Tesemõ — corpus legislativo brasileiro: https://github.com/ulysses-camara/ulysses-tesemo
- Curso/compilação do Método Leite Alves com seção de abreviações: https://pt.scribd.com/document/58462024/Sampaio-Caderno-de-Taquigrafia
- Lista ampliada de taquigramas do Método Maron: https://pt.scribd.com/document/598321125/Taquigramas-Do-Metodo-Maron-2011-1
