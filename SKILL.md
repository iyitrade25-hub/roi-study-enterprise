---
name: roi-study-enterprise
description: >
  Use this skill whenever an Account Executive needs to build, structure, or present
  a ROI study (estudo de ROI / business case) for a B2B SaaS client. Triggers include:
  any mention of "ROI", "estudo de impacto", "business case", "renovação", "expansão",
  "apresentação de valor", or when the user shares transcripts, indicators, or operational
  data from a client and asks to extract value or build arguments for negotiation.

  Also trigger when the user wants to:
  - Analyze a meeting transcript to extract ROI evidence
  - Identify what data is missing to complete a ROI study
  - Build a deck or onepager to present results to a client
  - Prepare questions for a ROI interview with a client champion
  - Consolidate metrics from operational reports (spreadsheets, PPTs, dashboards)

  This skill covers the full ROI workflow: interview, data extraction, gap analysis,
  ROI calculation and executive deck generation.
---

# ROI Study: Enterprise AE Workflow

Esta skill codifica o processo completo de construção de um estudo de ROI para renovação
ou expansão de conta enterprise B2B SaaS. Funciona para qualquer ferramenta e qualquer
tipo de processo (financeiro, fiscal, compras, operações, manutenção, atendimento).

Ao longo do texto, **[Ferramenta]** se refere à solução SaaS cujo valor está sendo
demonstrado, e **[Cliente]** à empresa que a utiliza.

---

## Fase 1: Entendimento do Contexto

Antes de qualquer análise, estabeleça:

1. **Qual processo está sendo analisado?** (nome, área, empresa)
2. **Qual é o objetivo comercial?** (renovação, upsell, expansão, case de sucesso)
3. **O que foi recebido como input?** (transcript, PPT de indicadores, planilha, resumo)
4. **Quem são os stakeholders?** (quem vai receber a apresentação: gestor operacional, TI, diretoria?)

Se o usuário colar ou anexar material sem explicar o objetivo, pergunte o objetivo comercial
antes de prosseguir.

---

## Fase 2: Análise de Material de Input

### 2a. Transcrições de reunião
Ao receber um transcript, extraia ativamente:

- **Números mencionados** (valores financeiros, percentuais, prazos, volumes)
- **Dores do antes** (como era feito antes da ferramenta)
- **Ganhos citados** (redução de tempo, custo evitado, pessoas liberadas)
- **Casos concretos** (histórias reais, incidentes, exemplos)
- **Riscos ainda abertos** (o que ainda não foi quantificado)
- **Próximos passos mencionados** (dados prometidos, reuniões futuras)

Nunca confunda dados parciais com dados confirmados. Sinalize com clareza o que é
estimativa e o que é número confirmado.

### 2b. Apresentações e dashboards de indicadores
Ao receber um PPT ou planilha com métricas:

- Extraia dados de SLA com série histórica (Ano 1 → Ano 2 → Ano 3)
- Identifique a meta estabelecida internamente pelo cliente
- Calcule a variação percentual entre períodos
- Separe por empresa/unidade se houver múltiplas entidades
- Identifique o indicador com maior variação: este será o argumento âncora

### 2c. Relatórios internos do cliente
Se o cliente tiver documentos internos de resultado (relatórios de gestão, apresentações
à diretoria, inscrições em premiações internas), extraia o retorno financeiro documentado.
Este é o dado mais credível do ROI, porque foi validado pelo próprio cliente e não
estimado pelo fornecedor.

---

## Fase 3: Estrutura de Três Pilares do ROI

Organize sempre o ROI em três camadas. Adapte os nomes ao contexto do cliente, mas mantenha
a lógica:

### Pilar 1: Saving Direto (financeiro, mensurável)
O que o cliente deixou de pagar ou gastou menos. Exemplos:
- Multas, juros ou penalidades evitadas
- Horas de trabalho eliminadas × custo/hora
- Ferramentas ou sistemas substituídos

**Formato de argumento:** "De R$ X para R$ Y, redução de Z%"

### Pilar 2: Eficiência Operacional (tempo e pessoas)
O que ficou mais rápido, com menos gente, com menos erro. Exemplos:
- Tempo de processo antes vs. depois
- Headcount reduzido ou realocado na operação
- Volume processado cresceu sem aumentar equipe

**Formato de argumento:** "O que levava X agora leva Y, ganho de Z%"

### Pilar 3: Risco Coberto (patrimonial, regulatório, operacional)
O que o cliente não perdeu, não pagou, não quebrou. Exemplos:
- Ativos ou valores rastreados (em R$)
- Risco de parada operacional evitado
- Conformidade regulatória mantida
- Continuidade mesmo com troca de colaborador

**Formato de argumento:** "R$ X protegidos / risco Y eliminado"

---

## Fase 4: Gap Analysis (o que ainda falta)

Após analisar o material disponível, sinalize explicitamente as lacunas:

**Lacunas críticas** (bloqueiam o cálculo do ROI):
- Custo unitário do problema principal (multa, erro, retrabalho, item perdido)
- Valor total pago ou perdido em períodos específicos antes e depois
- Volume processado por período

**Lacunas importantes** (enriquecem mas não bloqueiam):
- Custo de hora de operação parada na área crítica
- Número de FTEs antes vs. depois, com custo/hora
- Benchmark do cenário anterior (estimativa aceita se confirmada pelo champion)

**Lacunas residuais** (para uma versão futura do estudo):
- Ganhos indiretos entre áreas (compartilhamento de recursos, padronização)
- Custos evitados de longo prazo (compras emergenciais, contratações adiadas)

---

## Fase 5: Roteiro de Entrevista com o Champion

Quando o usuário precisar preparar perguntas para uma reunião de ROI, organize por objetivo:

### Para fechar saving direto:
- "Qual era o volume médio de X (multas, retrabalho, erros) antes da implementação?"
- "Você tem algum registro do custo total acumulado antes de Y?"
- "Quanto custa em média uma ocorrência desse problema?"

### Para construir o benchmark do antes:
- "Como era feito o controle antes: planilha, e-mail, sistema?"
- "Quantas pessoas estavam envolvidas nesse processo?"
- "Você lembra de algum caso concreto de perda ou problema que nunca mais se repetiu?"

### Para quantificar risco operacional:
- "Alguma vez a falta de controle causou parada ou interrupção da operação?"
- "Quanto custa uma hora de operação parada na área mais crítica?"
- "Com o processo atual, o que acontece se o responsável sair da empresa?"

### Para abrir expansão:
- "Existe algum outro processo com o mesmo perfil de risco que ainda é gerenciado fora da plataforma?"
- "Quais melhorias você já identificou que ainda não foram implementadas?"

O banco completo, organizado por tipo de processo, está em `references/interview-questions.md`.

---

## Fase 6: Geração do Deck Executivo

Quando o usuário pedir um deck, siga esta estrutura de 7 slides. Adapte o conteúdo
ao cliente, mas mantenha a ordem narrativa:

```
Slide 1: Capa
  Título do processo + empresa + período
  3 números âncora visíveis já na capa (saving, eficiência, risco)

Slide 2: O que está em jogo
  Volume financeiro sob gestão / escala do processo
  Por que esses números importam (conexão com risco)

Slide 3: Saving Direto
  Comparativo antes × depois com números reais
  Meta vs. resultado atual
  Nota explicando exceções ou casos isolados

Slide 4: Ganho de SLA
  Gráfico evolutivo (série histórica de 2 ou 3 períodos)
  Cards laterais com % de melhoria por empresa/unidade
  Linha de meta interna do cliente

Slide 5: Eficiência Operacional
  3 big numbers (tempo, pessoas, volume)
  Gráfico de volume crescendo com SLA melhorando
  Outros SLAs relevantes do processo

Slide 6: Controle e Visibilidade
  Checklist antes × depois
  Caso concreto (história real do cliente)
  Citação direta do champion

Slide 7: ROI Consolidado
  3 pilares com número âncora cada
  CTA para próximos passos ou lacunas abertas
```

O copy sugerido para cada slide está em `references/roi-template.md`.

### Identidade visual
Use a paleta da marca do cliente quando disponível. Na ausência dela, prefira uma paleta
neutra e sóbria (por exemplo azul-marinho, cinza e branco).
Consulte a skill `pptx` para implementação técnica.

---

## Regras de Argumentação

**Use números do próprio cliente sempre que possível.** Dados validados internamente
pelo cliente são muito mais poderosos que estimativas do fornecedor.

**Separe o que é documentado do que é estimativa.** Nunca misture os dois sem sinalizar.
Um dado confirmado vale mais que três estimativas.

**Mostre a curva de maturidade, não só o estado atual.** A evolução ao longo de dois ou
três períodos é o argumento mais difícil de refutar: o cliente não pode negar os próprios
dados históricos.

**Explique os outliers antes que o cliente pergunte.** Se houve exceções (por exemplo,
ocorrências pontuais no período pós-implementação), antecipe com a causa raiz documentada.
Isso demonstra honestidade e fortalece a credibilidade do estudo.

**O pilar de risco coberto é frequentemente subestimado.** Milhões em valores rastreados
costumam impressionar mais que dezenas de milhares economizados, mesmo que o segundo seja
saving direto e o primeiro seja proteção de risco. Use ambos, mas abra com o que for maior.

---

## Referências

- `references/roi-template.md`: template de slides com copy sugerida por seção
- `references/interview-questions.md`: banco completo de perguntas por tipo de processo

---

## Exemplo Ilustrativo (fictício)

> Empresa, números e resultados abaixo são inventados, apenas para demonstrar o formato
> esperado de saída. Não representam nenhum cliente real.

**Cliente:** Distribuidora Exemplo S.A. (3 unidades)
**Processo:** Aprovação de compras e pagamento a fornecedores
**Objetivo:** Renovação após 2 anos de uso

**Dados coletados:**
- Juros e multas por atraso de pagamento antes: ~R$ 240k/ano
- Juros e multas após a implementação: ~R$ 30k/ano → **–87,5%**
- Ciclo de compra: 10 dias → 3 dias → **–70%**
- Aprovações fora do sistema (e-mail, mensagem, verbal): 40% → 5%
- Headcount no processo: 4 pessoas → 2 pessoas, sem perda de SLA
- Volume de pedidos cresceu 35% no período sem aumento de equipe
- Volume anual de compras rastreado na plataforma: R$ 18M

**Como os pilares ficam:**
- Saving Direto: R$ 210k/ano em juros e multas evitados
- Eficiência Operacional: ciclo 70% mais rápido e 2 FTEs realocados
- Risco Coberto: R$ 18M/ano com trilha de aprovação auditável

**Resultado esperado:** deck de 7 slides pronto para apresentação à diretoria.
