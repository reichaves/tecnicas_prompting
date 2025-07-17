# 01 - Fundamentos do Prompting

## O que é um Prompt?

Um **prompt** é a instrução ou entrada que fornecemos a um modelo de IA para que gere uma resposta ou resultado. O modelo responde em linguagem natural baseando-se nessa indicação.

> 💡 **Conceito-chave**: Os modelos generativos não "entendem" intenções ocultas, apenas seguem as instruções fornecidas. Por isso, é responsabilidade do usuário formular bem o pedido.

## A Importância de um Bom Prompt

A qualidade do prompt influencia diretamente a qualidade da resposta do modelo. Pense no prompting como uma habilidade similar a fazer as perguntas certas em uma entrevista jornalística.

## Prompt Genérico vs. Específico

### Exemplo de Comparação

**Prompt Genérico:**
```
"O que você pode me dizer sobre mudanças climáticas?"
```

**Prompt Específico:**
```
"Você é um jornalista científico. Resuma em 3 frases claras os efeitos das 
mudanças climáticas na América Latina, citando um dado recente."
```

### Por que a diferença importa?

- O prompt genérico pode gerar respostas muito amplas e pouco úteis
- O prompt específico:
  - Define um papel (jornalista científico)
  - Estabelece uma tarefa clara (resumir)
  - Limita o escopo (3 frases)
  - Especifica o contexto geográfico (América Latina)
  - Requer evidência (dado recente)

## Princípios Básicos do Prompting Eficaz

### 1. Seja Específico
Em vez de perguntas abertas, forneça instruções claras sobre o que você precisa.

### 2. Forneça Contexto
Ajude o modelo a entender o quadro de referência da sua solicitação.

### 3. Defina o Formato
Especifique como você quer que a resposta seja estruturada.

### 4. Estabeleça Limitações
Indique restrições como comprimento, tom ou estilo.

## Exercício Prático

Transforme estes prompts genéricos em específicos:

1. **Genérico**: "Escreva sobre economia"
   **Específico**: Sua versão aqui

2. **Genérico**: "Me dê informações sobre eleições"
   **Específico**: Sua versão aqui

3. **Genérico**: "Fale sobre tecnologia"
   **Específico**: Sua versão aqui

## Erros Comuns a Evitar

1. **Ser vago demais**: "Me diga algo interessante"
2. **Não especificar o formato**: Esquecer de indicar se quer lista, parágrafo, tabela, etc.
3. **Assumir conhecimento implícito**: O modelo não conhece seu contexto específico
4. **Prompts muito longos sem estrutura**: Dificultam a compreensão

## Melhores Práticas

- **Itere e refine**: Se a primeira resposta não for ideal, ajuste seu prompt
- **Salve prompts bem-sucedidos**: Crie sua biblioteca pessoal
- **Experimente variações**: Pequenas mudanças podem melhorar muito os resultados
- **Inclua exemplos**: Se possível, mostre o tipo de resposta que espera

## Próximos Passos

Uma vez que você compreenda estes fundamentos, estará pronto para explorar os [elementos específicos de um bom prompt](02-elementos.md).

---

[← Voltar ao início](../README.md) | [Próximo: Elementos de um Bom Prompt →](02-elementos.md)
