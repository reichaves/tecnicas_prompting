# 03 - Casos de Uso no Jornalismo

Esta seção explora aplicações práticas de prompting em tarefas jornalísticas cotidianas, com exemplos e templates prontos para usar.

## 📰 1. Geração de Títulos

### Por que usar IA para títulos?
- Gerar múltiplas opções rapidamente
- Explorar diferentes ângulos
- Otimizar para diferentes plataformas
- Superar bloqueios criativos

### Template Básico
```
"Você é um editor de [tipo de publicação]. Crie [número] títulos para 
a seguinte notícia: [resumo ou lead da notícia]. 

Requisitos:
- Máximo [X] caracteres
- Tom: [informativo/chamativo/neutro]
- Evite: [clickbait/sensacionalismo/jargões]
- Inclua: [palavra-chave se necessário]"
```

### Exemplo Prático
```
"Você é um editor de portal de notícias online. Crie 5 títulos para a 
seguinte notícia: 'Pesquisa revela que 67% dos brasileiros mudaram 
hábitos de consumo após a pandemia, priorizando compras online e 
produtos locais.'

Requisitos:
- Máximo 60 caracteres
- Tom informativo mas envolvente
- Inclua o dado percentual
- Foque no impacto pós-pandemia"
```

### Variações por Plataforma
- **Web**: Títulos SEO-friendly com palavras-chave
- **Redes Sociais**: Mais conversacionais e diretos
- **Impressp**: Podem ser mais longos e descritivos

## 📋 2. Resumos Automáticos

### Aplicações
- Condensar relatórios extensos
- Criar briefs de notícias
- Preparar newsletters
- Resumir transcrições de entrevistas

### Template para Resumo
```
"Como jornalista, resuma o seguinte [tipo de documento] em [número] 
[frases/parágrafos], destacando:
- [Aspecto 1]
- [Aspecto 2]
- [Aspecto 3]

Mantenha: [dados específicos/citações/números]
Tom: [objetivo/analítico/informativo]
Público: [especializado/geral]"
```

### Exemplo Real
```
"Como jornalista econômico, resuma este relatório do Banco Central em 
3 parágrafos, destacando:
- Taxa de juros atual e projeção
- Principais riscos inflacionários
- Mudanças em relação ao relatório anterior

Mantenha todos os percentuais exatos
Tom: objetivo e técnico
Público: leitores com conhecimento básico de economia"
```

## 🗂️ 3. Organização de Pautas

### Usos Práticos
- Priorizar coberturas
- Organizar reuniões de pauta
- Distribuir tarefas na redação
- Planejar coberturas especiais

### Template de Organização
```
"Você é um editor-chefe. Organize as seguintes pautas:
[Lista de pautas]

Critérios:
1. Agrupe por editoria (política, economia, cultura, etc.)
2. Classifique por urgência (urgente, hoje, esta semana)
3. Indique recursos necessários (repórter, fotógrafo, tempo)
4. Sugira ordem de prioridade baseada em [critério]"
```

### Exemplo Aplicado
```
"Você é um editor-chefe de um jornal regional. Organize estas pautas:
- Aumento de casos de dengue na cidade
- Novo shopping será inaugurado
- Prefeito anuncia mudanças no trânsito
- Festival de música no fim de semana
- Escândalo de corrupção na câmara

Critérios:
1. Agrupe por relevância jornalística
2. Considere impacto na comunidade
3. Sugira deadline para cada pauta
4. Indique se precisa de acompanhamento"
```

## 🔍 4. Análise de Documentos

### Cenários de Uso
- Investigações com muitos documentos
- Análise de dados públicos
- Revisão de processos judiciais
- Fact-checking de declarações

### Template para Análise
```
"Você é um jornalista investigativo. Analise o documento anexo e:

1. Identifique os principais atores mencionados
2. Extraia todas as datas e crie uma linha do tempo
3. Destaque valores monetários e suas contextos
4. Aponte inconsistências ou informações contraditórias
5. Liste perguntas para investigação adicional

Formato: relatório estruturado com subtítulos
Foco: [aspecto específico da investigação]"
```

### Dicas para Documentos Longos
- Divida em seções se exceder limite de tokens
- Peça primeiro um sumário geral
- Depois aprofunde em seções específicas
- Use prompts encadeados para análise completa

## 🎨 5. Criação de Imagens

### Quando Usar
- Ilustrar matérias sem fotos
- Criar infográficos conceituais
- Visualizar dados ou estatísticas
- Produzir conteúdo para redes sociais

### Template para Imagens
```
"Crie uma [tipo de imagem] mostrando [descrição da cena].

Estilo: [fotorrealista/ilustração/infográfico]
Composição: [descrição de elementos e posicionamento]
Cores: [paleta ou mood]
Iluminação: [tipo e direção]
Detalhes importantes: [elementos que não podem faltar]
Evitar: [elementos indesejados]
Formato: [proporção e resolução]"
```

### Exemplo Prático
```
"Crie uma ilustração fotorrealista mostrando o impacto da seca em 
uma cidade do interior.

Estilo: fotojornalístico, realista
Composição: rua principal com comércio local, pessoas caminhando
Cores: tons terrosos, céu sem nuvens, sensação árida
Iluminação: sol forte do meio-dia criando sombras duras
Detalhes importantes: 
- Vegetação seca
- Solo rachado visível
- Pessoas com expressões de cansaço
- Comércio com aspecto de pouco movimento
Evitar: dramatização excessiva
Formato: 16:9, alta resolução"
```

## 💡 Melhores Práticas por Caso

### Para Todos os Casos:
1. **Sempre revise**: IA é ferramenta, não substituto
2. **Verifique fatos**: Especialmente datas e números
3. **Mantenha ética**: Transparência sobre uso de IA
4. **Personalize**: Adapte templates ao seu contexto
5. **Itere**: Refine prompts baseado nos resultados

### Erros Comuns a Evitar:
- Aceitar primeira resposta sem revisão
- Não verificar informações geradas
- Usar tom inadequado para o veículo
- Esquecer contexto local/cultural
- Não creditar uso de IA quando apropriado

## 📚 Próximos Passos

Explore [técnicas avançadas](04-tecnicas-avancadas.md) para maximizar resultados ou revise [limitações éticas](05-limitacoes-etica.md) do uso de IA no jornalismo.

---

[← Elementos](02-elementos.md) | [Início](../README.md) | [Técnicas Avançadas →](04-tecnicas-avancadas.md)
