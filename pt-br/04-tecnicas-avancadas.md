# 04 - Técnicas Avançadas de Prompting

Este capítulo explora métodos sofisticados para obter resultados superiores dos modelos de IA, especialmente úteis para investigações complexas e projetos jornalísticos ambiciosos.

## 🌳 Tree-of-Thoughts (Árvore de Pensamentos)

### O que é?
Uma técnica que faz a IA explorar múltiplos ramos de pensamento antes de decidir uma resposta, similar a como um jornalista avalia diferentes ângulos de uma história.

### Estrutura Básica
```
"Explore este tema considerando múltiplas perspectivas:

1. Primeiro, identifique 3-4 abordagens possíveis
2. Para cada abordagem, desenvolva os argumentos principais
3. Avalie prós e contras de cada perspectiva
4. Sintetize uma conclusão balanceada

Tema: [Seu tema aqui]"
```

### Exemplo Jornalístico
```
"Como editor investigativo, analise a proposta de lei sobre privacidade 
digital:

1. Identifique 4 perspectivas-chave:
   - Defensores da privacidade
   - Empresas de tecnologia
   - Governo/segurança
   - Cidadãos comuns

2. Para cada perspectiva, desenvolva:
   - Argumentos principais
   - Interesses em jogo
   - Possíveis consequências

3. Avalie conflitos entre perspectivas

4. Proponha ângulos jornalísticos para cobrir o tema"
```

### Quando Usar Tree-of-Thoughts
- Investigações com múltiplos stakeholders
- Análise de políticas públicas
- Cobertura de temas controversos
- Planejamento de séries investigativas

## 🔄 ReAct (Reasoning and Acting)

### O que é?
Combina raciocínio passo a passo com ações específicas, permitindo que o modelo "pense em voz alta" antes de responder.

### Estrutura ReAct
```
"Passo 1 - Raciocínio: [Analise a situação]
Passo 2 - Ação: [O que fazer baseado na análise]
Passo 3 - Observação: [O que resultou da ação]
Passo 4 - Conclusão: [Síntese final]"
```

### Aplicação em Fact-Checking
```
"Verifique esta afirmação usando o método ReAct:
'O desemprego juvenil aumentou 50% no último ano'

Raciocínio: Primeiro devo identificar qual período específico é 
mencionado e quais fontes oficiais reportam desemprego juvenil.

Ação: Buscar dados do IBGE para o último ano disponível.

Observação: [Incluir dados encontrados]

Raciocínio: Comparar com o ano anterior e calcular a porcentagem 
real de mudança.

Conclusão: A afirmação é [verificada/falsa/parcialmente correta] 
porque..."
```

## 📚 Bibliotecas e Templates

### Criando sua Biblioteca Pessoal

#### Template: Investigação de Antecedentes
```
PROMPT: Perfil de Investigação

Você é um jornalista investigativo preparando um perfil sobre [SUJEITO].

Compile e organize:
1. Informação biográfica básica
2. Trajetória profissional
3. Conexões empresariais/políticas
4. Declarações públicas relevantes
5. Controvérsias ou investigações prévias
6. Patrimônio declarado (se público)

Fontes a considerar:
- Registros públicos
- Declarações de bens
- Notícias anteriores
- Redes sociais profissionais

Formato: Relatório executivo com seções claramente marcadas
Advertências: Sinalize informação não verificada ou rumores
```

#### Template: Análise de Dados
```
PROMPT: Análise Jornalística de Dados

Contexto: Tenho um dataset sobre [TEMA] com as seguintes variáveis:
[LISTA DE VARIÁVEIS]

Tarefas:
1. Identifique as 3 tendências mais significativas
2. Busque correlações relevantes
3. Detecte anomalias ou outliers
4. Sugira visualizações apropriadas
5. Formule perguntas para investigação adicional

Considerações:
- Tamanho da amostra
- Possíveis vieses nos dados
- Limitações do dataset
- Contexto socioeconômico

Entrega: Bullet points com achados-chave + parágrafo narrativo
```

## 🔗 Prompting em Cadeia

### O que é?
Técnica de usar múltiplos prompts sequenciais onde cada um constrói sobre o anterior.

### Exemplo: Investigação em 4 Passos

**Prompt 1 - Exploração**
```
"Liste os 10 principais atores envolvidos no caso de 
corrupção na [empresa/instituição]"
```

**Prompt 2 - Aprofundamento**
```
"Para os 3 atores mais importantes da lista anterior, detalhe:
- Papel específico
- Conexões entre eles
- Benefícios obtidos"
```

**Prompt 3 - Verificação**
```
"Identifique quais afirmações da análise anterior precisam 
de verificação adicional e sugira fontes para confirmá-las"
```

**Prompt 4 - Narrativa**
```
"Construa um lead de 100 palavras que capture a essência 
desta investigação, começando com o achado mais impactante"
```

## 🎯 Few-Shot Prompting

### O que é?
Fornecer exemplos específicos do tipo de resposta que você busca.

### Estrutura
```
"Quero títulos neste estilo:

Exemplo 1: 'Revelam rede de subornos: 15 funcionários implicados'
Exemplo 2: 'Exclusivo: Documentos mostram desvio milionário'
Exemplo 3: 'Investigam ministro por conflito de interesse'

Agora crie 5 títulos similares para esta notícia: [NOTÍCIA]"
```

### Quando é Mais Efetivo
- Quando precisa de consistência de estilo
- Para formatos específicos do veículo
- Ao treinar novos colaboradores
- Para manter tom editorial

## 🧩 Combinação de Técnicas

### Super-Prompt Investigativo
```
[CONTEXTO - System Instructions]
Você é um jornalista investigativo sênior da Folha de S.Paulo 
especializado em seguir o dinheiro em casos de corrupção.

[TREE-OF-THOUGHTS]
Analise o seguinte caso de 3 perspectivas:
1. Fluxo financeiro
2. Rede de contatos
3. Timeline de eventos

[REACT]
Para cada perspectiva:
- Raciocine o que buscar
- Identifique fontes necessárias
- Antecipe obstáculos

[FEW-SHOT]
Formato de saída como estes exemplos:
- "ACHADO: [descrição] | FONTE: [tipo] | VERIFICAÇÃO: [método]"

[CHAIN]
Finalmente, proponha os próximos 5 passos de investigação em ordem 
de prioridade.
```

## 💡 Técnicas Específicas por Tipo de Cobertura

### Para Investigação Financeira
```
"Modo: Análise forense financeira
1. Rastreie fluxos de dinheiro entre entidades
2. Identifique padrões suspeitos
3. Marque transações que requerem escrutínio
4. Sugira especialistas para consultar"
```

### Para Cobertura Eleitoral
```
"Modo: Análise eleitoral multidimensional
1. Tendências demográficas
2. Comparação histórica
3. Fatores externos influentes
4. Cenários prováveis com porcentagens"
```

### Para Jornalismo de Dados
```
"Modo: Data journalist
1. Limpeza de dados - o que eliminar/corrigir
2. Variáveis-chave para a história
3. Correlações vs causações
4. Visualização mais impactante"
```

## 📈 Otimização de Resultados

### Técnica de Refinamento Iterativo
1. **Prompt inicial**: Amplo e exploratório
2. **Refinamento 1**: Foca em achados interessantes
3. **Refinamento 2**: Aprofunda em detalhes específicos
4. **Polimento final**: Ajusta tom e formato

### Exemplo Prático
```
Iteração 1: "Analise tendências em educação pública"
Iteração 2: "Foque na desigualdade rural-urbana identificada"
Iteração 3: "Detalhe casos específicos de 3 municípios"
Iteração 4: "Reescreva com tom humano, incluindo depoimentos"
```

## 🛠️ Ferramentas Complementares

### Prompts para Diferentes Ferramentas

**Para NotebookLM**
```
"Analise estes 10 documentos e crie:
1. Resumo executivo de achados comuns
2. Contradições entre documentos
3. Linha temporal unificada
4. Pessoas mencionadas com frequência"
```

**Para Google AI Studio com Code Execution**
```
"Analise este CSV de gastos governamentais:
1. Calcule totais por departamento
2. Identifique aumentos superiores a 50%
3. Crie gráfico de tendências
4. Marque anomalias estatísticas"
```

## ✅ Melhores Práticas Avançadas

1. **Documente seus prompts exitosos**: Crie um repositório pessoal
2. **Combine técnicas conforme necessidade**: Nem todas servem para tudo
3. **Ajuste por modelo**: Gemini vs GPT vs Claude respondem diferente
4. **Meça efetividade**: Tempo econom
