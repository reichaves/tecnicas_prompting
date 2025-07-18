# Ferramentas de IA para Jornalistas

Este capítulo apresenta as principais ferramentas de inteligência artificial úteis para o trabalho jornalístico, com foco em aplicações práticas, custos e melhores práticas de uso.

## 1. Ferramentas de Texto e Análise

### ChatGPT (OpenAI)

#### Características
- **Versões:** GPT-3.5 (gratuito limitado), GPT-4 (pago)
- **Pontos fortes:** Versatilidade, compreensão de contexto, geração de texto
- **Limitações:** Data de corte de conhecimento, pode "alucinar" informações

#### Casos de Uso para Jornalistas
```
ANÁLISE DE DOCUMENTOS
Prompt: "Analise este relatório governamental e extraia:
1. 5 pontos principais
2. Dados estatísticos relevantes
3. Possíveis ângulos de notícia
4. Inconsistências ou lacunas

[Inserir texto do documento]"

GERAÇÃO DE PERGUNTAS
Prompt: "Crie 10 perguntas para entrevistar o ministro da saúde sobre:
- Situação da pandemia
- Orçamento da saúde pública
- Novas políticas preventivas

Estilo: direto mas respeitoso, foco no interesse público."
```

#### Custo e Planos
- **Gratuito:** 20 mensagens/3h com GPT-4o mini
- **Plus ($20/mês):** Acesso ilimitado ao GPT-4, análise de imagens
- **API:** Pago por token, mais econômico para uso intensivo

### Claude (Anthropic)

#### Características
- **Versões:** Claude Sonnet (gratuito limitado), Claude Opus (pago)
- **Pontos fortes:** Análise de documentos longos, ética na resposta, raciocínio
- **Diferencial:** Pode processar textos muito longos (até 200k tokens)

#### Aplicações Específicas
```
ANÁLISE DE DOCUMENTOS EXTENSOS
"Leia este documento de 100 páginas sobre orçamento municipal e:
1. Crie um resumo executivo de 300 palavras
2. Identifique as 5 maiores mudanças em relação ao ano anterior
3. Destaque possíveis irregularidades ou pontos questionáveis
4. Sugira fontes específicas para entrevistar"

VERIFICAÇÃO DE CONSISTÊNCIA
"Compare estas 3 declarações do mesmo político em datas diferentes:
[Declaração 1 - Janeiro]
[Declaração 2 - Março]  
[Declaração 3 - Junho]

Identifique contradições e evolução de posições."
```

#### Custo
- **Gratuito:** Uso limitado do Claude Sonnet
- **Pro ($20/mês):** Acesso prioritário e maior limite de uso

### Gemini (Google)

#### Características
- **Versões:** Gemini (gratuito), Gemini Advanced (pago)
- **Pontos fortes:** Integração com Google Workspace, análise de imagens
- **Diferencial:** Acesso a informações atualizadas via busca do Google

#### Aplicações Jornalísticas
```
PESQUISA CONTEXTUALIZADA
"Pesquise informações recentes sobre:
- Política econômica atual do governo brasileiro
- Principais críticas e apoios
- Dados estatísticos mais recentes
- Posições de especialistas

Foque em fontes oficiais e notícias dos últimos 30 dias."

ANÁLISE DE IMAGENS
"Analise esta foto da manifestação e forneça:
1. Descrição objetiva da cena
2. Estimativa de participantes
3. Elementos visuais relevantes
4. Contexto inferível da imagem"
```

## 2. Ferramentas Especializadas

### Perplexity AI

#### Características
- **Foco:** Pesquisa com fontes citadas
- **Pontos fortes:** Cita fontes automaticamente, informações atualizadas
- **Ideal para:** Verificação inicial de informações

#### Uso Jornalístico
```
VERIFICAÇÃO RÁPIDA
"Verifique esta afirmação: 'O Brasil é o 3º maior produtor mundial de soja'
Forneça:
- Confirmação ou negação da informação
- Fontes oficiais que sustentam a resposta
- Dados atualizados sobre produção de soja
- Posição atual do Brasil no ranking mundial"
```

#### Custo
- **Gratuito:** 5 buscas Pro por dia
- **Pro ($20/mês):** Buscas ilimitadas, upload de arquivos

### Notion AI

#### Características
- **Integração:** Dentro do ecossistema Notion
- **Pontos fortes:** Organização de informações, resumos, templates
- **Ideal para:** Gestão de projetos jornalísticos

#### Aplicações
```
ORGANIZAÇÃO DE PAUTA
"Organize estas informações sobre corrupção municipal:
- Cronologia de eventos
- Personagens envolvidos
- Documentos coletados
- Próximos passos da investigação

Crie uma estrutura clara para acompanhamento."
```

### Otter.ai

#### Características
- **Especialidade:** Transcrição de áudio em tempo real
- **Pontos fortes:** Precisão, identificação de falantes, integração
- **Ideal para:** Entrevistas e conferências de imprensa

#### Workflow para Jornalistas
1. **Gravação:** Gravar entrevista com app
2. **Transcrição:** Automática em tempo real
3. **Edição:** Revisar e corrigir erros
4. **Análise:** Usar IA para extrair quotes principais

## 3. Ferramentas de Análise de Dados

### Jupyter AI / Google Colab

#### Características
- **Ambiente:** Notebooks para análise de dados
- **Pontos fortes:** Análise estatística, visualizações, código Python
- **Ideal para:** Jornalismo de dados

#### Exemplo de Uso
```python
# Análise de gastos públicos com IA
import pandas as pd
import matplotlib.pyplot as plt

# Carregar dados
dados = pd.read_csv('gastos_municipais.csv')

# Prompt para IA assistente
"""
Analise estes dados de gastos municipais e:
1. Identifique padrões suspeitos
2. Crie visualizações relevantes
3. Calcule estatísticas descritivas
4. Sugira hipóteses para investigação
"""
```

### Tableau com IA

#### Características
- **Especialidade:** Visualização de dados com assistente IA
- **Pontos fortes:** Gráficos automáticos, insights sugeridos
- **Ideal para:** Criação rápida de infográficos

### Power BI (Microsoft)

#### Características
- **Integração:** Office 365, fontes de dados diversas
- **IA Features:** Q&A em linguagem natural, insights automáticos
- **Ideal para:** Redações que usam ecossistema Microsoft

## 4. Ferramentas de Verificação

### SIFT (Stanford Internet Observatory)

#### Características
- **Foco:** Verificação de informações online
- **Métodos:** Stop, Investigate, Find, Trace
- **Gratuito:** Recursos educacionais

### InVID (WeVerify)

#### Características
- **Especialidade:** Verificação de vídeos e imagens
- **Recursos:** Análise de metadados, busca reversa
- **Gratuito:** Plugin para navegador

### TruthNest

#### Características
- **Foco:** Verificação automatizada de claims
- **Integração:** APIs para redações
- **Status:** Em desenvolvimento

## 5. Fluxo de Trabalho Integrado

### Setup Básico para Redação

#### Ferramentas Essenciais (Custo-benefício)
```
NÍVEL GRATUITO/BÁSICO:
- ChatGPT (gratuito) para análise inicial
- Gemini para pesquisa atualizada
- Otter.ai (gratuito limitado) para transcrições
- SIFT/InVID para verificação

INVESTIMENTO TOTAL: $0-40/mês
```

#### Setup Profissional
```
NÍVEL PROFISSIONAL:
- ChatGPT Plus ($20/mês)
- Claude Pro ($20/mês)  
- Perplexity Pro ($20/mês)
- Otter.ai Pro ($17/mês)
- Tableau Creator ($75/mês)

INVESTIMENTO TOTAL: ~$150/mês
```

### Workflow Típico de Reportagem

#### 1. Pesquisa Inicial (Gemini + Perplexity)
```
"Pesquise informações sobre [TÓPICO]:
- Contexto histórico
- Desenvolvimentos recentes
- Principais stakeholders
- Controvérsias atuais
- Fontes primárias para contato"
```

#### 2. Análise de Documentos (Claude)
```
"Analise estes documentos oficiais:
- Extraia informações-chave
- Identifique inconsistências
- Sugira perguntas para autoridades
- Destaque dados verificáveis"
```

#### 3. Preparação de Entrevistas (ChatGPT)
```
"Crie roteiro de entrevista para:
- [Perfil do entrevistado]
- [Objetivos da entrevista]
- [Contexto da matéria]
- [Tempo disponível]"
```

#### 4. Transcrição e Análise (Otter.ai + IA de texto)
```
"Da transcrição desta entrevista, extraia:
- 5 quotes mais impactantes
- Pontos que contradizem versão oficial
- Informações que precisam verificação
- Follow-ups necessários"
```

#### 5. Verificação (Ferramentas especializadas)
- Checar claims específicos
- Verificar dados estatísticos
- Confirmar informações com fontes primárias

#### 6. Estruturação Final (IA de texto)
```
"Organize esta matéria seguindo:
- Lead com informação principal
- Desenvolvimento com contexto
- Quotes relevantes distribuídos
- Dados verificados integrados
- Conclusão com próximos passos"
```

## 6. Segurança e Boas Práticas

### Proteção de Dados Sensíveis

#### O que NÃO colocar em ferramentas IA:
- 🚫 Nomes reais de fontes confidenciais
- 🚫 Dados pessoais identificáveis  
- 🚫 Documentos vazados não autorizados
- 🚫 Informações que comprometem investigações

#### Técnicas de Anonimização:
```
❌ Evitar:
"João Silva, morador da Rua X, 123, relatou que..."

✅ Usar:
"Fonte local relatou que..."

❌ Evitar:
"Documento interno da empresa ABC mostra..."

✅ Usar:
"Documento empresarial indica..."
```

### Backup e Documentação

#### Sistema de Backup:
- Salvar prompts eficazes em biblioteca pessoal
- Documentar configurações que funcionam
- Manter logs de verificações realizadas
- Backup de conversas importantes

#### Controle de Versão:
```
Estrutura de arquivo sugerida:
/projetos
  /investigacao-corrupcao-municipal
    /prompts-utilizados.md
    /fontes-verificadas.md
    /conversas-ia/
      /2024-01-15-analise-documentos.txt
      /2024-01-16-perguntas-entrevista.txt
    /documentos-originais/
    /verificacoes/
```

## 7. Considerações de Custo-Benefício

### Análise de ROI para Redações

#### Métricas de Economia:
- **Tempo economizado** em pesquisa inicial
- **Redução de custos** em transcrição manual
- **Aumento de produtividade** na análise de dados
- **Melhoria na qualidade** de verificação

#### Cálculo Simplificado:
```
EXEMPLO DE REDAÇÃO PEQUENA (3 jornalistas):

CUSTOS MENSAIS:
- Ferramentas IA: $120/mês
- Treinamento inicial: $500 (uma vez)

ECONOMIA ESTIMADA:
- 20h/mês economizadas em pesquisa: $800
- 10h/mês economizadas em transcrição: $300
- Melhoria em qualidade: Inestimável

ROI: 900% no primeiro ano
```

### Estratégia de Implementação Gradual

#### Fase 1 (Mês 1-2): Ferramentas Gratuitas
- Testar ChatGPT gratuito
- Experimentar Gemini
- Avaliar resultados e necessidades

#### Fase 2 (Mês 3-4): Investimento Básico
- Subscrever 1-2 ferramentas pagas
- Treinar equipe em uso eficaz
- Documentar melhores práticas

#### Fase 3 (Mês 5-6): Otimização
- Adicionar ferramentas especializadas
- Automatizar workflows
- Medir resultados e ajustar

## 8. Troubleshooting Comum

### Problemas Frequentes e Soluções

#### "A IA não entende meu prompt"
**Solução:** Ser mais específico e dar contexto
```
❌ Vago: "Analise este documento"
✅ Específico: "Analise este relatório financeiro de 20 páginas da prefeitura e extraia: 1) maiores gastos por categoria, 2) comparação com ano anterior, 3) possíveis irregularidades"
```

#### "Respostas são muito genéricas"
**Solução:** Fornecer exemplos e especificar formato
```
"Crie perguntas de entrevista no estilo jornalístico investigativo:
EXEMPLO: 'O senhor pode explicar por que sua empresa ganhou 80% das licitações municipais nos últimos dois anos?'
CONTEXTO: Entrevista com empresário sobre contratos públicos
FORMATO: 10 perguntas diretas e específicas"
```

#### "Informações parecem incorretas"
**Solução:** Sempre verificar e pedir fontes
```
"Forneça informações sobre [TÓPICO] e para cada afirmação:
1. Indique fonte ou tipo de fonte necessária
2. Marque nível de confiança (alto/médio/baixo)  
3. Sinalize se informação pode estar desatualizada"
```

## 9. Recursos para Aprofundamento

### Cursos e Certificações
- **Knight Center (UT Austin):** Cursos gratuitos sobre IA no jornalismo
- **Coursera:** Especialização em prompt engineering
- **Abraji:** Workshops sobre tecnologia investigativa

### Comunidades Profissionais
- **AI for Journalism** (grupo no LinkedIn)
- **Computational Journalism** (grupo no Facebook)
- **NICAR** (Computer-Assisted Reporting)

### Ferramentas de Teste
- **OpenAI Playground:** Para experimentar modelos
- **Hugging Face:** Modelos open source
- **Anthropic Console:** Para testar Claude
- **Google AI Studio:** Interface experimental do Gemini

---

**Próximo passo:** Consulte [Prompts Utilizados](prompts-utilizados.md) para exemplos práticos testados e [Referências](referencias.md) para aprofundamento teórico.
