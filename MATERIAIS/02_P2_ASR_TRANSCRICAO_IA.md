# Caderno P2 — ASR, Transcrição, Degravação e IA aplicada

Atualizado em: 02/10/2026

## A1 — Fundamentos de ASR

**ASR (Automatic Speech Recognition)** é a conversão automática de sinal de fala em representação textual.

Pipeline conceitual clássico:
1. captura/normalização do áudio;
2. extração/representação acústica;
3. modelagem acústica e/ou end-to-end;
4. modelagem linguística/decodificação;
5. pós-processamento: pontuação, capitalização, normalização, diarização etc.

Modelos end-to-end modernos aprendem diretamente mapeamentos entre áudio e texto, reduzindo a separação rígida entre módulos clássicos.

### Erros e métricas
Métrica recorrente: **WER — Word Error Rate**.
WER = (substituições + deleções + inserções) / número de palavras da referência.

WER menor indica transcrição lexical mais próxima da referência, mas **não mede sozinho qualidade editorial/parlamentar**: pontuação, nomes próprios, identificação de oradores, números e fidelidade pragmática também importam.

### Áudio nativo em modelos multimodais
Modelos multimodais podem processar áudio diretamente em arquiteturas que integram múltiplas modalidades. Não confundir “modelo multimodal com áudio” com simples pipeline ASR + LLM textual: ambos podem produzir texto, mas a arquitetura/fluxo é diferente.

Fontes:
- Jurafsky & Martin, Speech and Language Processing;
- OpenAI Whisper README/model card.

---

## A2 — Whisper e serviços em nuvem

### Whisper
Modelo de reconhecimento de fala e tradução de fala, sequência-a-sequência, multilíngue, treinado em grande escala. Pode realizar:
- reconhecimento de fala;
- identificação de idioma;
- tradução de fala para inglês em configurações suportadas.

Pontos de prova:
- é ASR generalista, não ferramenta específica de registro parlamentar;
- saída automática exige revisão em contexto de alta responsabilidade;
- tamanho do modelo, ruído, sotaque e domínio afetam desempenho;
- transcrição automática não equivale a degravação editorial pronta.

### Google Cloud Speech-to-Text / Azure AI Speech / AWS Transcribe
Estudar por comparação funcional:
- transcrição batch e/ou streaming;
- timestamps;
- diarização/identificação de locutores, quando suportada;
- vocabulário/frases customizadas;
- pontuação automática;
- integração por API;
- tratamento de áudio e idiomas.

Não decorar preço, limites comerciais transitórios ou nomes de planos salvo se o edital/retificação trouxer.

---

## A3 — Diarização, pontuação e capitalização

### Diarização
Problema: **“quem falou quando?”**

Produz segmentação temporal por locutor. Não necessariamente identifica a identidade civil do locutor; muitas soluções rotulam SPEAKER_00, SPEAKER_01 etc.

Distinguir:
- diarização: separa segmentos por locutor;
- identificação/verificação de locutor: associa voz a identidade/modelo específico;
- ASR: converte fala em texto.

### Pontuação automática
Reconstrói sinais ausentes no fluxo acústico. Usa prosódia, contexto lexical e modelos linguísticos.

Risco parlamentar: pontuação pode mudar escopo, relações sintáticas e sentido. Deve ser passível de revisão humana.

### Capitalização
Recupera caixa adequada: início de período, nomes próprios, siglas etc. Também está sujeita a erros de entidades/nomenclatura institucional.

---

## A4 — Desafios do português brasileiro

Fatores:
- variação regional/social;
- fala espontânea;
- sobreposição de vozes;
- ruído/reverberação;
- velocidade de fala;
- nomes próprios;
- siglas;
- estrangeirismos;
- terminologia legislativa;
- números, datas e referências normativas;
- disfluências e autocorreções.

Em ambiente parlamentar, o domínio é altamente específico. Customização de vocabulário e revisão especializada podem reduzir erros críticos.

---

## A5 — Tempo real x batch

### Tempo real/streaming
Entrega hipóteses progressivas com baixa latência. Pode haver revisões do texto conforme chega mais contexto.

### Batch/offline
Processa gravação já disponível. Pode usar mais contexto e tolerar latência maior.

Trade-offs:
- latência;
- custo computacional;
- contexto disponível;
- estabilidade da hipótese;
- necessidade operacional.

Item Cebraspe típico: “tempo real” não significa necessariamente texto final imutável.

---

## A6 — Transcrição automática, degravação e revisão humana

### Transcrição automática
Saída gerada pelo sistema a partir do áudio.

### Degravação
Conversão do registro oral em texto escrito com grau de tratamento definido pela finalidade. Pode exigir:
- identificação de falantes;
- normalização;
- pontuação;
- tratamento de disfluências;
- marcação de trechos inaudíveis;
- preservação de conteúdo.

### Revisão humana
Validação/correção por pessoa, com critérios editoriais e de fidelidade.

**Não confundir:** uma saída ASR de alta acurácia ainda não é necessariamente um registro oficial pronto.

---

## A7 — HITL — Human in the Loop

HITL integra intervenção humana ao pipeline.

Exemplos:
- sistema transcreve;
- revisor corrige nomes, números, pontuação e locutores;
- alterações alimentam dicionários, regras ou dados de avaliação;
- casos de baixa confiança são escalados.

Benefícios:
- qualidade;
- auditabilidade;
- tratamento de exceções;
- controle de risco.

Custos:
- latência;
- necessidade de equipe;
- desenho de interface e fluxo;
- possibilidade de erro humano.

HITL não elimina automação; organiza cooperação humano-máquina.

---

## A8 — Fidelidade, qualidade e revisão

Dimensões:
- fidelidade semântica;
- completude;
- precisão lexical;
- identificação correta de falantes;
- pontuação;
- padronização;
- rastreabilidade;
- tempo de entrega.

### Falso dilema
“Literalidade máxima” e “texto publicável” não são sempre a mesma coisa. Um registro oficial pode exigir tratamento formal sem autorizar alteração substantiva do discurso.

### Controle de qualidade
Mecanismos citados no edital:
- dupla revisão;
- amostragem/auditoria;
- SLA;
- verificação de termos sensíveis;
- comparação com áudio;
- logs/rastreabilidade.

**SLA** formaliza níveis de serviço (tempo, disponibilidade, qualidade etc.). Não é sinônimo de métrica de qualidade.

---

## A9 — Normalização

Casos críticos:
- números;
- datas;
- valores monetários;
- siglas;
- abreviaturas;
- nomes próprios;
- termos técnicos;
- dispositivos legais.

Exemplo: áudio “artigo cinco parágrafo primeiro” pode exigir padronização conforme convenção editorial adotada.

Regra: normalizar forma sem inventar conteúdo.

---

## A10 — CAT tools e ferramentas de apoio

CAT = Computer-Assisted Translation, mas o edital usa a ideia mais ampla de ferramentas de apoio à revisão/produção linguística.

Recursos possíveis:
- memória terminológica;
- glossários;
- busca/concordância;
- comparação de versões;
- QA automatizado;
- segmentação;
- consistência lexical.

No contexto de registro/redação, ferramentas análogas podem apoiar consistência e revisão sem substituir julgamento editorial.

---

## A11 — Vocabulário parlamentar e adaptação de domínio

Problema: modelos generalistas erram termos raros, siglas, nomes e fórmulas legislativas.

Técnicas:
- phrase hints/context biasing;
- glossários;
- custom vocabulary;
- fine-tuning/adaptação quando disponível;
- pós-correção baseada em dicionários;
- recuperação de contexto institucional;
- listas dinâmicas de parlamentares/matérias.

Risco: reforço excessivo pode introduzir palavra esperada que não foi efetivamente pronunciada. Fidelidade ao áudio prevalece.

---

## A12 — IA aplicada a parlamentos

Usos do edital:
- transcrição;
- sumarização;
- indexação;
- busca;
- pesquisa semântica;
- geração automática de atas/resumos;
- tradução/multilinguismo;
- modelos especializados em português.

### Sumarização
Pode ser:
- extrativa;
- abstrativa.

Riscos:
- omissão;
- alucinação;
- enviesamento de saliência;
- atribuição errada de posição;
- perda de ressalvas.

### Busca semântica
Recupera conteúdo por proximidade de significado, não apenas coincidência literal. Pode usar embeddings/vetores.

### Indexação
Associa metadados/descritores a segmentos/documentos para recuperação.

---

## A13 — LGPD, direitos autorais, ética e segurança

### LGPD
Áudio e transcrições podem conter dados pessoais. Processamento no poder público deve observar finalidade, necessidade, segurança, transparência e bases/regras aplicáveis.

Não decorar apenas consentimento: consentimento é uma das bases, e o poder público possui regras próprias.

### Direitos autorais
Distinguir:
- conteúdo protegido;
- obra oficial/atos normativos em condições específicas;
- uso de bases/dados;
- licenças de software/modelos.

### Ética
Pontos:
- transparência sobre automação;
- revisão humana proporcional ao risco;
- não fabricar fala;
- preservação da integridade documental;
- controle de vieses;
- responsabilização.

### Segurança do pipeline
Riscos:
- vazamento de áudio;
- credenciais/API;
- armazenamento indevido;
- ataques a sistemas;
- alteração de transcrição;
- logs contendo dados sensíveis.

Controles:
- autenticação/autorização;
- criptografia;
- segmentação;
- menor privilégio;
- versionamento/logs;
- backups;
- gestão de fornecedores;
- revisão de saída.

---

## A14 — Comparações que a banca pode explorar

| Conceitos | Distinção nuclear |
|---|---|
| ASR x diarização | o que foi dito x quem falou quando |
| diarização x identificação | agrupar vozes x atribuir identidade |
| streaming x batch | baixa latência progressiva x processamento posterior |
| transcrição x degravação | saída textual x produto textual tratado conforme finalidade |
| WER x qualidade editorial | erro lexical x qualidade institucional multidimensional |
| ASR + LLM x áudio nativo multimodal | pipeline em etapas x processamento multimodal integrado |
| automação x HITL | execução automática x fluxo com decisão/revisão humana |
| busca lexical x semântica | termos idênticos x proximidade de significado |
| resumo x registro oficial | condensação x preservação do registro |

---

## Fontes canônicas

Jurafsky & Martin:
https://web.stanford.edu/~jurafsky/slp3/

Whisper:
https://github.com/openai/whisper
https://github.com/openai/whisper/blob/main/model-card.md

Google Cloud Speech-to-Text:
https://cloud.google.com/speech-to-text/docs

Microsoft Azure AI Speech:
https://learn.microsoft.com/azure/ai-services/speech-service/

AWS Transcribe:
https://docs.aws.amazon.com/transcribe/

LGPD:
https://www.planalto.gov.br/ccivil_03/_ato2015-2018/2018/lei/l13709.htm

CERT.br:
https://cartilha.cert.br/

## Uso no estudo

Na primeira passagem, dominar definições, comparações e fluxo.
Na segunda passagem, priorizar cenários (“qual componente resolve qual problema?”).
Na discursiva, sempre ligar tecnologia a qualidade, revisão humana, proteção de dados e fidelidade institucional.
