# Guia Completo do Google AI Studio para Jornalistas

O Google AI Studio é uma plataforma poderosa para prototipar e testar prompts com os modelos Gemini. Este guia detalha as configurações essenciais para jornalistas.

## 🚀 Configurações Essenciais

### 1. System Instructions (Instruções do Sistema)
**O que é**: Define a personalidade, papel e estilo das respostas da IA.

**Como usar para jornalismo**:
```
"Você é um jornalista investigativo cético, sempre verificando fatos e 
questionando fontes. Suas respostas devem ser objetivas, baseadas em 
evidências e seguir o padrão de pirâmide invertida."
```

### 2. Temperature (Temperatura)
**O que é**: Controla a aleatoriedade e criatividade das respostas (0 a 1).

**Configurações recomendadas**:
- `0.0 - 0.3`: Fact-checking, resumos, análise de dados
- `0.4 - 0.7`: Redação de notícias, perguntas para entrevistas
- `0.8 - 1.0`: Brainstorming, títulos criativos, pautas

### 3. Token Count (Contagem de Tokens)
**O que é**: Quantidade de texto que o modelo pode processar.

**Limites importantes**:
- Gemini 1.5 Pro: até 2 milhões de tokens de entrada
- Gemini 1.5 Flash: até 1 milhão de tokens
- 1 token ≈ 0,75 palavras em português

### 4. Thinking Mode (Modo Pensamento)
**O que é**: Mostra o raciocínio do modelo antes da resposta final.

**Quando ativar**:
- Investigações complexas
- Análises que requerem múltiplas perspectivas
- Verificação de lógica em argumentos

### 5. Grounding with Google Search
**O que é**: Conecta o modelo a informações atualizadas da web.

**Essencial para**:
- Verificação de fatos recentes
- Cobertura de eventos atuais
- Confirmação de dados e estatísticas

## 📊 Configuração Recomendada para Jornalismo

### Para Reportagem Factual:
```
Temperature: 0.1
Thinking Mode: Ativado
Grounding: Ativado
Safety Settings: Máximo
System Instructions: "Você é um jornalista factual. Sempre cite fontes 
e indique quando a informação não pode ser verificada."
```

### Para Conteúdo Criativo:
```
Temperature: 0.7
Thinking Mode: Desativado
Top P: 0.9
System Instructions: "Você é um redator criativo mas responsável. 
Mantenha precisão factual enquanto explora ângulos interessantes."
```

## 🔧 Outras Configurações Úteis

### Top P
- Controla diversidade vocabular
- Use valores baixos (0.1-0.5) para textos técnicos
- Use valores altos (0.8-0.95) para textos criativos

### Safety Settings
Configure filtros para:
- Discurso de ódio
- Conteúdo prejudicial
- Desinformação
- Importante: Mantenha no máximo para jornalismo

### Code Execution
Permite análise de dados com Python:
- Útil para jornalismo de dados
- Processamento de planilhas
- Criação de visualizações

## 💰 Limites da Conta Gratuita

### Requisições por Minuto (RPM):
- Gemini 1.5 Pro: 2 RPM
- Gemini 1.5 Flash: 15 RPM

### Requisições por Dia (RPD):
- Gemini 1.5 Pro: 50 RPD
- Gemini 1.5 Flash: 1.500 RPD
- Grounding with Search: 1.000-1.500 RPD

## 🎯 Fluxo de Trabalho Otimizado

### 1. Pesquisa Inicial
```
1. Use Gemini Flash com Temperature 0.5
2. Ative Grounding para dados atuais
3. Faça perguntas exploratórias
```

### 2. Aprofundamento
```
1. Mude para Gemini Pro
2. Reduza Temperature para 0.1
3. Ative Thinking Mode
4. Faça análises detalhadas
```

### 3. Redação Final
```
1. Use configuração equilibrada (Temperature 0.3)
2. Defina System Instructions para tom desejado
3. Revise e verifique todos os fatos
```

## ⚡ Atalhos de Produtividade

### Templates Salvos
Crie e salve prompts para:
- Resumos de coletivas
- Análise de documentos
- Geração de pautas
- Fact-checking

### Uso de Contexto
- Anexe múltiplos documentos
- Use até 10 arquivos por vez
- Formatos suportados: PDF, TXT, DOC, imagens

### Exportação
- Copie código para API
- Exporte para Vertex AI
- Salve histórico de conversas

## 🚨 Avisos Importantes

1. **Sempre verifique**: Informações podem estar incorretas
2. **Cite o uso de IA**: Mantenha transparência
3. **Proteja fontes**: Não inclua informações sensíveis
4. **Respeite limites**: Monitore uso de tokens e requisições

## 📚 Recursos Adicionais

- [Documentação Oficial](https://ai.google.dev/docs)
- [Melhores Práticas](https://ai.google.dev/docs/prompting_guide)
- [Fórum da Comunidade](https://discuss.ai.google.dev/)

---

[← Voltar ao início](README.md)
