<div align="center">

# 📊 Treinando uma IA de Aprendizagem: Análise Fundamentalista de FIIs

*Documentação de engenharia de prompts e caderno temático de estudos no NotebookLM para análise de Fundos Imobiliários.*

**[📄 Acessar o Manual Prático em PDF](https://github.com/dosg-labs/miniguia-estudos-notebooklm/blob/main/Manual%20Pr%C3%A1tico_%20O%20Caminho%20para%20Viver%20de%20Renda%20com%20Fundos%20Imobili%C3%A1rios%20(FIIs).pdf)**
<br>
[📚 Ver Curadoria de Fontes](#curadoria) • [🛠️ Engenharia de Prompts](#engenharia) • [🎬 Vídeo Complementar](https://youtu.be/NKIsmVbg9I8)

---
</div>

## 📌 Sumário
- [Contexto e Objetivos](#contexto)
- [Curadoria de Fontes](#curadoria)
- [Engenharia de Prompts e "Cicatrizes"](#engenharia)
- [Entrega Principal: Miniguia de Estudo (Manual Prático)](#entrega-principal)
  - [Arquivo do Manual Prático](#arquivo-pdf)
  - [1. Resumo Estruturado dos FIIs](#resumo)
  - [2. Painel de Controle de Indicadores](#indicadores)
  - [3. Exercício Prático: Fundo Fictício "EXPLO11"](#exercicio)
  - [4. Glossário de Conceitos](#glossario)
  - [5. Prompts Reutilizáveis para Estudo](#prompts)
- [Recurso Multimídia: Análise Didática em Vídeo](#multimidia)
- [Reflexões Críticas e Roadmap de Evolução (V2)](#reflexoes)
- [Autor](#autor)

---

<a id="contexto"></a>
## 🎯 Contexto e Objetivos

Este projeto foi desenvolvido como parte do desafio prático do **Bootcamp Bradesco - GenAI, Dados & Cyber** promovido pela **DIO**. O intuito é utilizar a IA Generativa (NotebookLM / Gemini) como uma ferramenta ativa de curadoria, síntese e estruturação do conhecimento.

> [!NOTE]
> ### **Objetivo Principal**
> * Capacitar qualquer pessoa leiga a realizar a **análise fundamentalista de Fundos de Investimento Imobiliário (FIIs)** a partir do zero.

### **Objetivos Complementares**
1. Compreender a estrutura, funcionamento e categorias de FIIs (Tijolo, Papel, FoFs e Híbridos).
2. Ler, interpretar e cruzar indicadores financeiros essenciais (P/VP, DY, Vacância Física vs. Financeira, Cap Rate, WALT, LTV).
3. Avaliar a qualidade de um fundo através do estudo de relatórios gerenciais e análise de cenários macroeconômicos.

---

<a id="curadoria"></a>
## 📚 Curadoria de Fontes

A seleção das fontes utilizou o recurso **Deep Search** do NotebookLM (Gemini Notebook). A partir de uma busca inicial que retornou 16 resultados, foram selecionados 3 materiais de alta reputação do mercado financeiro:

| Instituição / Portal | Tópico Abordado | Link de Acesso |
| :--- | :--- | :--- |
| **Mais Retorno** | 10 indicadores fundamentais para análise de FIIs | [Acessar Artigo](https://maisretorno.com/portal/10-indicadores-dos-fundos-imobiliarios-que-voce-precisa-conhecer-antes-de-investir) |
| **XP Investimentos** | Metodologia completa de análise de FIIs | [Acessar Relatório](https://conteudos.xpi.com.br/fundos-imobiliarios/relatorios/como-analisar-fundos-imobiliarios/) |
| **Banco Daycoval** | Passo a passo e conceitos introdutórios | [Acessar Artigo](https://blog.daycoval.com.br/como-analisar-um-fii/) |

---

<a id="engenharia"></a>
## 🛠️ Engenharia de Prompts e "Cicatrizes"

A construção do caderno temático passou por um processo iterativo de refinamento de prompts (*Troubleshooting*) utilizando o **Gemini 3.1 Pro**.

### 📉 Matriz de Erros e Aprendizados (*Post-Mortem*)

| Tentativa | Prompt Utilizado / Intenção | Resultado Ocorrido | Diagnóstico & Lição Aprendida |
| :---: | :--- | :--- | :--- |
| **1ª** | Busca por *PDFs completos da CVM/B3 cobrindo do básico ao Valuation*. | ❌ **0 resultados** retornados. | **Prompt Hiper-restritivo:** Exigir múltiplos critérios rígidos travou a busca. |
| **2ª** | Busca por *documentos que ensinem tudo sobre FIIs para iniciantes*. | ⚠️ Sugestões de focos genéricos. | **Vício de Formato:** Exigir "para iniciantes" descartou artigos técnicos valiosos. |
| **3ª** | *"Metodologias e princípios de análise fundamentalista de Fundos de Investimento Imobiliário (FIIs)."* | ✅ **16 fontes qualificadas**. | **Matéria-prima Pura:** Buscar conteúdo técnico bruto para que a IA traduza depois. |

> [!TIP]
> **Lição Aprendida:** Separe a fase de **Coleta de Dados** da fase de **Sintetização Didática**. Na busca inicial, utilize prompts focados na matéria-prima técnica; no chat do caderno, solicite a simplificação para linguagem didática.

---

<a id="entrega-principal"></a>
## 📖 Entrega Principal: Miniguia de Estudo (Manual Prático)

<a id="arquivo-pdf"></a>
### 📄 Arquivo do Manual Prático
A entrega central e produto final deste desafio é o miniguia em PDF gerado diretamente via NotebookLM a partir do processo de síntese e prompts personalizados em português:

> [!IMPORTANT]
> 👉 **[Download / Visualizar o Manual Prático em PDF](https://github.com/dosg-labs/miniguia-estudos-notebooklm/blob/main/Manual%20Pr%C3%A1tico_%20O%20Caminho%20para%20Viver%20de%20Renda%20com%20Fundos%20Imobili%C3%A1rios%20(FIIs).pdf)**

---

<a id="resumo"></a>
### 1. Resumo Estruturado dos FIIs

Os **Fundos Imobiliários (FIIs)** democratizaram o mercado imobiliário brasileiro ao permitir que investidores acessem ativos de alto padrão com baixo capital inicial e isenção de Imposto de Renda sobre os rendimentos mensais (para pessoas físicas).

**Fluxo de Funcionamento do FII:**
1. **Investidor** ➔ *(Compra Cotas)* ➔ **Fundo Imobiliário**
2. **Fundo Imobiliário** ➔ *(Adquire)* ➔ **Imóveis / Títulos**
3. **Imóveis / Títulos** ➔ *(Gera Rendimentos)* ➔ **Investidor** (Recebe Aluguéis / Juros)

#### **Categorias e Especificidades Técnicas**
* **Fundos de Tijolo:** Imóveis físicos (Shoppings, Galpões Logísticos, Lajes Corporativas). Renda advinda dos aluguéis.
* **Fundos de Papel (Recebíveis):** Títulos de dívida imobiliária (CRI, LCI). Exigem análise de crédito, tranches (Sênior, Mezanino, Subordinada) e **LTV (Loan-to-Value)**.
* **Fundos de Fundos (FoFs):** Investem em cotas de outros FIIs, garantindo diversificação instantânea.
* **Híbridos:** Combinam ativos imobiliários físicos com títulos de crédito.

---

<a id="indicadores"></a>
### 2. Painel de Controle de Indicadores

| Indicador | O que avalia? | Leitura / Critério |
| :--- | :--- | :--- |
| **P/VP** | Preço da Cota vs. Valor Patrimonial | `= 1` (Preço justo), `< 1` (Desconto), `> 1` (Ágio) |
| **Dividend Yield (DY)** | Retorno em proventos | Avaliar histórico de 12m para verificar consistência |
| **Vacância (Física x Financeira)** | Espaço desocupado x Perda de receita | Física baixa com financeira alta indica carências excessivas |
| **WALT to Break / Expiry** | Média do prazo dos contratos | O *To Break* mede a 1ª janela de saída sem multa |
| **Absorção Líquida** | Variação de m² ocupados vs. devolvidos | Se positiva, indica expansão da ocupação no fundo |

---

<a id="exercicio"></a>
### 3. Exercício Prático: Fundo Fictício "EXPLO11"

Para consolidar o aprendizado, o manual prático realiza a análise passo a passo de um fundo fictício de Tijolo (Logístico):

* **Dados do EXPLO11:** Cota: R$ 100,00 | VP: R$ 110,00 | DY (12m): 10% a.a. | Vacância Física: 2% | WALT to Break: 6 anos | Portfólio: 5 Galpões AAA em SP/MG.
* **Análise:**
  1. *P/VP:* R$ 100 / R$ 110 = 0,90 (Comprado com 10% de desconto patrimonial).
  2. *Yield:* 10% a.a., retorno real robusto e recorrente.
  3. *Risco/Qualidade:* Imóveis AAA de alta liquidez com contratos atípicos de longo prazo.
* **Conclusão:** O EXPLO11 representa uma oportunidade clara, onde o deságio de 10% (P/VP 0,90) decorre do pessimismo do mercado e não de fundamentos ruins do fundo.

---

<a id="glossario"></a>
### 4. Glossário de Conceitos

* **Cota:** A menor fração do patrimônio do fundo.
* **CapEx (Capital Expenditure):** Investimentos em melhorias e modernização dos imóveis.
* **LTV (Loan-to-Value):** Razão entre a dívida e o valor da garantia (abaixo de 50% indica margem saudável).
* **CRI (Certificado de Recebíveis Imobiliários):** Título de dívida imobiliária que compõe a carteira dos fundos de papel.
* **IFIX:** Índice benchmark do mercado de FIIs na B3.

---

<a id="prompts"></a>
### 5. Prompts Reutilizáveis para Estudo

Utilize estas perguntas orientadoras no chat do seu **NotebookLM** para analisar novos relatórios gerenciais:

1. *"Apresente-me todos os indicadores deste FII, ensinando-me a analisar um a um com definições e exemplos práticos."*
2. *"Explique, de modo didático, os tipos de contratos de locação (típicos vs. atípicos) presentes neste relatório e os pontos de atenção."*
3. *"Ensine, passo a passo, como um investidor leigo deve ler a seção de DRE (Demonstração do Resultado do Exercício) deste fundo."*
4. *"Monte um quadro comparativo elencando os riscos específicos e as oportunidades identificadas na tese deste fundo."*

---

<a id="multimidia"></a>
## 🎬 Recurso Multimídia: Análise Didática em Vídeo

Adicionalmente ao relatório escrito em PDF, foi gerada uma **síntese multimídia em áudio/vídeo** através do NotebookLM. 

Um achado relevante durante o projeto foi a comparação entre os formatos: enquanto o relatório textual acabou apresentando limitações e ficando excessivamente técnico em suas seções finais, **no vídeo a IA não demonstrou essas travas de clareza**. O modelo conseguiu expor os conceitos financeiros com uma linguagem fluida, natural e extremamente didática para o público iniciante.

🎬 **[Clique aqui para assistir ao vídeo explicativo no YouTube](https://youtu.be/NKIsmVbg9I8)**

---

<a id="reflexoes"></a>
## 💡 Reflexões Críticas e Roadmap de Evolução (V2)

A avaliação contínua das saídas geradas pela IA faz parte de uma postura responsável de Engenharia de Prompts. A partir do resultado final deste projeto, foram registradas as seguintes observações e oportunidades de melhoria:

### **1. Análise Crítica dos Resultados (Texto vs. Áudio)**
* **Densidade Técnica no Relatório:** O manual em PDF começou com boa cadência e didática, porém tornou-se técnico demais no decorrer das seções.
* **Efetividade Multimodal:** A versão em áudio/vídeo gerada pelo NotebookLM superou as limitações do texto, demonstrando maior eficiência cognitiva e clareza para a introdução ao tema.

> [!WARNING]
> ### **2. Hipóteses de Melhoria e Ajustes de Prompt (Roadmap V2)**
> Para contornar a curva de complexidade e elevar a precisão do estudo em próximas iterações, foram traçadas três frentes de atuação:
> 
> 1. **Ampliação da Curadoria de Fontes:** Integrar portais de dados financeiros em tempo real (como *Investidor10* ou *StatusInvest*) para indicadores dinâmicos, combinados a artigos acadêmicos para rigor metodológico.
> 2. **Prompts de Tradução Didática Compulsória:** Implementar travas nos prompts que forcem a IA a **sempre emparelhar qualquer conceito financeiro complexo com um exemplo prático do dia a dia** (ex: *"Sempre que mencionar LTV, explique utilizando a analogia de um empréstimo com garantia pessoal"*).
> 3. **Framework de Análise Escalável:** Aprimorar o caderno temático para transformar a estrutura de prompts em um modelo reutilizável, capaz de processar relatórios gerenciais e executar a análise fundamentalista automatizada de **qualquer fundo imobiliário listado na B3**.

---

<a id="autor"></a>
## 👤 Autor

Desenvolvido por **Diego de Oliveira**  
*Estudante do Bootcamp Bradesco - GenAI, Dados & Cyber da DIO.*
