# Anki Pós-Edital — Arquitetura Canônica

Atualizado em: 02/10/2026

## Decisão

O antigo gate AS0 (“descobrir qual versão está instalada”) deixa de bloquear o estudo.

Motivo:
- o edital alterou o escopo;
- o usuário determinou que Anki faça parte da revisão;
- manter dependência de baralhos pré-edital desconhecidos cria atraso sem benefício.

Será usado um baralho **novo**, com nome inequívoco:

`Analista 2027`

Os baralhos antigos podem permanecer no aparelho, mas não entram no cronograma até eventual auditoria.

## Subbaralhos

- Analista 2027::P2::Linguística
- Analista 2027::P2::ASR_Transcrição_IA
- Analista 2027::P2::Processo_Regimentos
- Analista 2027::P2::Ciência_Política
- Analista 2027::P1::Português
- Analista 2027::P1::Inglês
- Analista 2027::P1::Administrativo
- Analista 2027::P1::Constitucional
- Analista 2027::P1::TI_Dados_IA
- Analista 2027::Discursiva

## Tipo de cartão

Padrão principal: **Cebraspe autossuficiente**.

Frente:
- uma proposição julgável;
- contexto suficiente;
- uma pegadinha realista.

Verso:
- CERTO ou ERRADO;
- explicação curta e profunda;
- distinção nuclear;
- fonte quando normativa.

Não criar cartão “O que é X?” salvo quando a recuperação conceitual pura for realmente melhor.

## O que vira cartão

Entram:
- erro real;
- acerto com dúvida;
- literalidade normativa de alto valor;
- comparação fácil de confundir;
- prazo/quórum/competência;
- conceito central de P2;
- estrutura discursiva de alto rendimento.

Não entram:
- exemplos triviais;
- detalhes de baixíssimo valor;
- conteúdo já automatizado;
- parágrafos inteiros de teoria.

## Rotina diária

Dentro da carga líquida do dia:

1. **20–30 min** — revisar cartões devidos.
2. Estudar o conteúdo.
3. **10–15 min** — revisar os novos cartões do módulo do dia.
4. Erro relevante em questões gera cartão ou correção de cartão.

O Anki não adiciona 45 minutos além da carga. Ele ocupa parte do bloco de revisão/aplicação.

## Regras de novos cartões

Primeira passagem:
- alvo normal: 8–15 novos cartões em dia de conteúdo;
- máximo: 20 novos/dia;
- domingo: preferencialmente 0 novos, salvo erro importante.

Se houver backlog relevante:
- suspender novos;
- zerar devidos;
- retomar novos depois.

## FSRS / agendamento

Se a versão do Anki/AnkiDroid oferecer FSRS:
- usar o agendador moderno;
- não manipular intervalos manualmente;
- responder conforme recordação real, não para “forçar” agenda.

Se FSRS não estiver disponível, manter agendamento padrão e evitar ajustes exóticos.

## Tags

Formato:
- `edital2026`
- `p2_linguistica`, `p2_asr`, etc.
- tópico: `signo`, `diarizacao`, `pec`, `federalismo`;
- data de introdução: `d_2026_10_03`;
- `erro_real` quando vier de erro;
- `literalidade` para lei/regimento.

## Revisões D+1/D+7/D+21

Anki cuida de cartões. O pacote diário ainda agenda revisão de **estruturas amplas**:
- D+1: recuperar mapa/explicar sem olhar;
- D+7: questões novas;
- D+21: bateria mista/remediação.

Não criar cartão para substituir treino discursivo ou compreensão de fluxos inteiros.

## Arquivo de importação

Será fornecido TSV UTF-8 com colunas:
- Deck
- Front
- Back
- Tags

Ao importar no Anki:
- separador: tabulação;
- HTML: permitido, se disponível;
- campo 1 = deck/subbaralho quando o importador permitir; caso não permita, importar por arquivo/subbaralho conforme instruções do aplicativo.

## Auditoria permanente

Cartão deve ser aposentado/corrigido quando:
- ambíguo;
- depende de contexto ausente;
- gabarito admite leitura alternativa relevante;
- simplifica regra de modo perigoso;
- fonte normativa mudou.

O banco de erros é mais importante que “quantidade de cartões”.
