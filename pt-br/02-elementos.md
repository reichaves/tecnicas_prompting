# 02 - Elementos de um Bom Prompt

Um prompt eficaz é composto por quatro elementos fundamentais que trabalham juntos para produzir resultados ótimos.

## 🎯 1. Clareza

### Definição
O prompt deve ser inequívoco e específico. Evitar termos vagos ou perguntas muito gerais que levem a respostas amplas e pouco úteis.

### Exemplos

❌ **Ambíguo:**
```
"Me explica tecnologia"
```

✅ **Claro:**
```
"Como especialista em cibersegurança, explique brevemente três medidas para 
proteger uma rede corporativa contra ataques de ransomware"
```

### Técnicas para melhorar a clareza:
- Use verbos de ação específicos (analise, compare, resuma, liste)
- Defina termos técnicos se necessário
- Evite pronomes sem referente claro
- Estruture as instruções em passos numerados quando apropriado

## 🌍 2. Contexto

### Definição
Fornecer informação de fundo ou situacional para guiar a IA. Isso inclui estabelecer um papel ou audiência e detalhes relevantes do tema.

### Componentes do contexto:
- **Papel**: "Você é um jornalista esportivo..."
- **Audiência**: "...escrevendo para leitores jovens..."
- **Situação**: "...cobrindo a Copa do Mundo de 2026..."
- **Restrições**: "...com limite de 500 palavras"

### Exemplo completo:
```
"Você é um jornalista esportivo escrevendo para um público geral não 
especializado. O contexto é a final da Copa América 2024. 
Preciso que explique as regras básicas do VAR de maneira simples."
```

## 📋 3. Instruções Precisas (Tarefa)

### Definição
Indicar claramente o que se quer que a IA faça. A tarefa é o núcleo da ordem e nunca deve faltar no prompt.

### Frases de ação úteis:
- **Para análise**: "Analise...", "Compare...", "Avalie..."
- **Para síntese**: "Resuma...", "Sintetize...", "Condense..."
- **Para criação**: "Gere...", "Crie...", "Elabore..."
- **Para organização**: "Liste...", "Categorize...", "Priorize..."

### Exemplo estruturado:
```
"Analise os seguintes dados de criminalidade:
1. Identifique as três tendências principais
2. Compare com o ano anterior
3. Sugira possíveis causas para as mudanças observadas"
```

## 📐 4. Formato de Saída

### Definição
Especificar o formato ou estilo esperado na resposta garante que o modelo entregue o conteúdo já estruturado conforme a necessidade.

### Opções de formato:
- **Estrutura**: Parágrafo, lista numerada, bullet points, tabela
- **Comprimento**: Número de palavras, frases ou parágrafos
- **Tom**: Formal, informal, acadêmico, conversacional
- **Estilo**: Jornalístico, técnico, criativo, informativo

### Exemplo detalhado:
```
"Formato de saída:
- Um parágrafo introdutório de 2-3 frases
- Lista de 5 pontos principais com marcadores
- Cada ponto deve ter máximo 50 palavras
- Tom: profissional mas acessível
- Incluir pelo menos duas estatísticas relevantes"
```

## 🔧 Combinando todos os elementos

### Prompt completo exemplar:
```
[CONTEXTO] Você é um editor de política em um jornal nacional.

[TAREFA] Resuma os pontos-chave do relatório anexo sobre transparência 
governamental, focando nos dados de 2023.

[CLAREZA] Identifique especificamente:
- Os três achados mais importantes
- Mudanças em relação ao ano anterior
- Implicações para políticas públicas

[FORMATO] Responda com:
- Um parágrafo inicial de contexto (máximo 3 frases)
- 3-5 pontos-chave em lista numerada
- Tom formal e objetivo
- Extensão total: máximo 300 palavras
```

## 📝 Exercício Prático

Crie um prompt que inclua os quatro elementos para as seguintes situações:

1. **Situação**: Você precisa de uma análise das redes sociais de um político
   **Seu prompt**: _______________

2. **Situação**: Quer gerar perguntas para uma entrevista com um CEO
   **Seu prompt**: _______________

3. **Situação**: Precisa de um resumo de um documento legal complexo
   **Seu prompt**: _______________

## ✅ Lista de Verificação

Antes de enviar seu prompt, verifique:
- [ ] É claro e específico?
- [ ] Inclui contexto relevante?
- [ ] A tarefa está bem definida?
- [ ] Especifica o formato desejado?
- [ ] Evita ambiguidades?

## 🚀 Próximos passos

Uma vez que domine estes elementos, explore como aplicá-los em [casos de uso específicos do jornalismo](03-casos-uso.md).

---

[← Fundamentos](01-fundamentos.md) | [Início](../README.md) | [Casos de Uso →](03-casos-uso.md)
