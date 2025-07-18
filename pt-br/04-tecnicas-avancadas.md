# Técnicas Avançadas de Prompting

Este capítulo apresenta metodologias sofisticadas de prompting que podem transformar a qualidade e eficácia do seu trabalho jornalístico com IA. Essas técnicas vão além do prompting básico e oferecem abordagens estruturadas para problemas complexos.

## 1. Chain-of-Thought (Cadeia de Pensamento)

### Conceito
O Chain-of-Thought prompting encoraja o modelo a mostrar seu processo de raciocínio passo a passo, resultando em respostas mais precisas e verificáveis.

### Aplicação em Jornalismo

#### Análise de Dados Complexos
```
"Analise estes dados de criminalidade da cidade de São Paulo nos últimos 5 anos. Pense passo a passo:

1. Primeiro, identifique as tendências gerais nos números
2. Em seguida, identifique padrões sazonais ou geográficos
3. Depois, compare com dados de contexto (população, políticas públicas)
4. Finalmente, formule hipóteses sobre as causas das variações

Para cada passo, mostre seu raciocínio e as evidências que sustentam suas conclusões.

Dados: [inserir dados estruturados]"
```

#### Verificação de Informações
```
"Vou te dar uma afirmação de um político. Quero que você avalie sua veracidade pensando em etapas:

Afirmação: "O Brasil reduziu a pobreza em 60% nos últimos 10 anos"

Etapa 1: Identifique os elementos verificáveis desta afirmação
Etapa 2: Determine que tipo de dados seriam necessários para verificar
Etapa 3: Avalie a plausibilidade baseada em conhecimento geral
Etapa 4: Indique possíveis fontes para checagem
Etapa 5: Classifique preliminarmente como: verificável/não verificável, plausível/implausível

Mostre seu raciocínio para cada etapa."
```

## 2. Tree-of-Thoughts (Árvore de Pensamentos)

### Conceito
Esta técnica explora múltiplos caminhos de raciocínio simultaneamente, permitindo backtracking e refinamento de ideias.

### Aplicação Prática

#### Desenvolvimento de Pauta Investigativa
```
"Tenho indícios de irregularidades em contratos de merenda escolar. Vamos explorar diferentes caminhos investigativos:

RAMO 1 - Análise Financeira:
- Investigar valores dos contratos
- Comparar preços com mercado
- Analisar histórico dos fornecedores

RAMO 2 - Análise Processual:
- Examinar processo licitatório
- Verificar cumprimento de prazos
- Checar documentação exigida

RAMO 3 - Impacto na Ponta:
- Qualidade da merenda entregue
- Relatos de estudantes e professores
- Dados nutricionais

Para cada ramo, desenvolva:
1. Fontes de informação específicas
2. Documentos necessários
3. Pessoas-chave para entrevistar
4. Possíveis obstáculos
5. Força probatória esperada

Depois, avalie qual combinação de ramos oferece a melhor estratégia investigativa."
```

## 3. ReAct (Reasoning and Acting)

### Conceito
Combina raciocínio com ações específicas, criando um ciclo iterativo de pensamento e execução.

### Estrutura ReAct para Jornalismo

```
"Vou investigar alegações de superfaturamento em obra pública. Use o método ReAct:

PENSAMENTO: [Analise a situação e determine próximos passos]
AÇÃO: [Especifique que ação tomar]
OBSERVAÇÃO: [Avalie resultados da ação]
PENSAMENTO: [Reajuste estratégia baseado nos resultados]
AÇÃO: [Nova ação baseada no aprendizado]

Comece com:
PENSAMENTO: Preciso estabelecer uma estratégia para investigar alegações de superfaturamento na construção do hospital municipal. Quais são os primeiros passos mais eficazes?

Continue o ciclo por pelo menos 5 iterações, construindo uma estratégia investigativa robusta."
```

## 4. Few-Shot Prompting Avançado

### Técnica de Exemplificação Progressiva

#### Para Entrevistas Investigativas
```
"Vou te mostrar exemplos de como fazer perguntas investigativas eficazes, depois você criará similares para nosso caso:

EXEMPLO 1 - Pergunta Direta com Evidência:
"Temos aqui o contrato assinado pelo senhor em março, no valor de R$ 2 milhões. Como explica que a empresa beneficiada foi criada apenas duas semanas antes da licitação?"

EXEMPLO 2 - Pergunta de Confronto Educada:
"O senhor declarou ontem que não conhece o empresário João Silva. Mas temos aqui 15 fotos dos dois juntos em eventos nos últimos dois anos. Pode nos ajudar a entender essa aparente contradição?"

EXEMPLO 3 - Pergunta Sequencial:
"Vamos por partes: primeiro, confirma que assinou este documento? Segundo, lembra das circunstâncias? Terceiro, pode explicar por que o processo foi acelerado?"

Agora crie 5 perguntas no mesmo estilo para este caso:
Situação: Secretário de Saúde que autorizou compra de equipamentos com preço 300% acima do mercado de uma empresa ligada a seu cunhado.

Evidências disponíveis: [listar evidências]
```

## 5. Prompt Chaining (Encadeamento de Prompts)

### Metodologia
Quebrar tarefas complexas em prompts sequenciais, onde cada saída alimenta o próximo prompt.

#### Série Investigativa: Da Denúncia à Publicação

**Prompt 1 - Análise Inicial:**
```
"Recebi esta denúncia anônima sobre corrupção na prefeitura. Analise a credibilidade inicial:

Denúncia: [texto da denúncia]

Avalie:
1. Consistência interna da narrativa
2. Especificidade das informações
3. Verificabilidade das alegações
4. Possíveis motivações do denunciante
5. Sinais de alerta (muito vago ou muito específico)

Resultado: [resumo + recomendação de prosseguir ou não]"
```

**Prompt 2 - Estratégia de Verificação:**
```
"Baseado na análise anterior: [inserir resultado do Prompt 1]

Desenvolva uma estratégia de verificação de 30 dias:

Semana 1: [ações prioritárias]
Semana 2: [aprofundamento]
Semana 3: [confirmações cruzadas]
Semana 4: [preparação para publicação]

Para cada semana, especifique:
- Documentos a buscar
- Pessoas a contactar
- Pedidos de informação a fazer
- Deadlines internos"
```

**Prompt 3 - Preparação de Entrevistas:**
```
"Com base na estratégia desenvolvida: [inserir resultado do Prompt 2]

Crie roteiros de entrevista para cada pessoa-chave identificada:

Para cada entrevistado, desenvolva:
1. Objetivos específicos da conversa
2. Perguntas de aquecimento
3. Perguntas centrais
4. Perguntas de confronto (se aplicável)
5. Documentos para apresentar
6. Estratégia para obter documentos adicionais"
```

## 6. Role-Playing Prompts

### Simulação de Múltiplas Perspectivas

```
"Vamos simular uma mesa redonda sobre a nova lei de proteção de dados pessoais. Você representará diferentes perspectivas:

ADVOGADO ESPECIALISTA EM TECNOLOGIA:
[Posição sobre aspectos legais e técnicos]

REPRESENTANTE DE EMPRESA DE TECNOLOGIA:
[Preocupações com compliance e custos]

ATIVISTA DE DIREITOS DIGITAIS:
[Foco em proteção do cidadão]

PARLAMENTAR AUTOR DA LEI:
[Defesa das intenções da legislação]

Para cada perspectiva, forneça:
1. Principais argumentos
2. Preocupações específicas
3. Propostas de solução
4. Críticas às outras perspectivas

Depois, identifique:
- Pontos de consenso
- Conflitos irreconciliáveis
- Áreas para negociação
- Perguntas que um jornalista deveria fazer a cada um"
```

## 7. Prompts de Verificação Cruzada

### Metodologia Anti-Viés

```
"Vou te apresentar uma análise que fiz sobre [TÓPICO]. Quero que você faça uma verificação crítica:

MINHA ANÁLISE: [inserir análise original]

VERIFICAÇÃO SOLICITADA:
1. Contra-argumentos: Que evidências contradizem minha análise?
2. Perspectivas ausentes: Que pontos de vista não considerei?
3. Vieses potenciais: Que preconceitos podem ter influenciado minha interpretação?
4. Lacunas de informação: Que dados importantes estão faltando?
5. Alternativas explicativas: Que outras interpretações são possíveis?

RESULTADO ESPERADO:
- Lista de pontos fracos na análise original
- Sugestões de como fortalecer os argumentos
- Recomendações de fontes adicionais
- Versão revisada mais equilibrada"
```

## 8. Prompts Metacognitivos

### Prompts que Refletem sobre o Próprio Processo

```
"Após analisar este documento governamental de 200 páginas sobre gastos públicos, quero que você reflita sobre seu próprio processo de análise:

DOCUMENTO: [inserir ou referenciar documento]

META-ANÁLISE SOLICITADA:
1. Como você priorizou quais seções analisar primeiro?
2. Que critérios usou para identificar informações relevantes?
3. Que preconceitos ou limitações podem ter influenciado sua análise?
4. Que perguntas você não consegue responder com os dados disponíveis?
5. Que tipo de especialista humano seria mais útil para validar suas conclusões?
6. Como você avaliaria a confiabilidade de sua própria análise (1-10)?

Esta reflexão me ajudará a entender melhor os limites e forças de sua análise."
```

## 9. Prompts de Simulação de Cenários

### Análise Prospectiva para Jornalismo

```
"Vamos simular diferentes cenários futuros baseados na aprovação (ou rejeição) desta lei no Congresso:

LEI EM QUESTÃO: [descrever a lei]

CENÁRIO 1 - Aprovação Integral:
- Impactos imediatos (3 meses)
- Consequências de médio prazo (1 ano)
- Possíveis efeitos não intencionais
- Grupos mais beneficiados/prejudicados

CENÁRIO 2 - Rejeição Completa:
- Manutenção do status quo
- Pressões para alternativas
- Impacto na agenda política
- Reações dos stakeholders

CENÁRIO 3 - Aprovação com Modificações:
- Que mudanças são mais prováveis?
- Como isso afetaria a eficácia da lei?
- Que grupos pressionariam por quais mudanças?

Para cada cenário:
1. Probabilidade estimada (%)
2. Indicadores para monitorar
3. Fontes para acompanhar desdobramentos
4. Ângulos jornalísticos mais promissores"
```

## 10. Prompts de Estruturação de Dados

### Organização de Informações Complexas

```
"Organizei estas informações sobre um escândalo político complexo. Preciso estruturá-las para melhor compreensão:

INFORMAÇÕES BRUTAS: [dump de informações desorganizadas]

ORGANIZE EM:

CRONOLOGIA:
- [Data]: [Evento] - [Importância: alta/média/baixa]

PERSONAGENS:
- [Nome]: [Papel] - [Relevância] - [Status: investigado/testemunha/suspeito]

FLUXOS FINANCEIROS:
- [Origem] → [Intermediário] → [Destino] - [Valor] - [Data]

EVIDÊNCIAS:
- [Tipo]: [Descrição] - [Força probatória] - [Status de verificação]

PENDÊNCIAS:
- [O que precisa ser investigado]
- [Fontes a contactar]
- [Documentos a obter]

ÂNGULOS NARRATIVOS:
- [Perspectiva 1]: [Resumo do foco]
- [Perspectiva 2]: [Resumo do foco]
- [Perspectiva 3]: [Resumo do foco]"
```

## Implementação Gradual

### Semana 1-2: Técnicas Básicas
- Chain-of-Thought para análises simples
- Few-shot prompting para formatos recorrentes

### Semana 3-4: Técnicas Intermediárias
- Prompt chaining para projetos complexos
- Role-playing para múltiplas perspectivas

### Semana 5-6: Técnicas Avançadas
- Tree-of-Thoughts para investigações
- Prompts metacognitivos para auto-reflexão

### Adaptação Contínua
- Documente o que funciona melhor para seu estilo
- Crie biblioteca pessoal de prompts eficazes
- Ajuste técnicas baseado em resultados

## Medição de Eficácia

### Métricas de Qualidade
- **Precisão**: Informações corretas vs. total de informações
- **Relevância**: Informações úteis vs. total de informações
- **Completude**: Aspectos cobertos vs. aspectos necessários
- **Eficiência**: Qualidade do resultado vs. tempo investido

### Indicadores de Sucesso
- Redução de tempo para pesquisa inicial
- Melhoria na estruturação de matérias
- Aumento na identificação de ângulos alternativos
- Maior consistência na verificação de fatos

---

**Próximo passo:** Compreenda as [Limitações e Considerações Éticas](05-limitacoes-etica.md) para uso responsável dessas técnicas.
