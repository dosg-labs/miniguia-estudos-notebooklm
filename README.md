<div align="center">

# 📊 Treinando uma IA de Aprendizagem: Análise Fundamentalista de FIIs

![DIO](https://img.shields.io/badge/DIO-Bootcamp%20Bradesco-red?style=for-the-badge)
![AI](https://img.shields.io/badge/NotebookLM-Gemini%203.1%20Pro-blue?style=for-the-badge)
![Domain](https://img.shields.io/badge/Finan%C3%A7as-FIIs-green?style=for-the-badge)
![Status](https://img.shields.io/badge/Status-Conclu%C3%ADdo-brightgreen?style=for-the-badge)

*Documentação de engenharia de prompts e caderno temático de estudos no NotebookLM para análise de Fundos Imobiliários.*

[📄 Acessar o Manual Prático em PDF](./Manual_Pratico_FIIs.pdf) • [📚 Ver Curadoria de Fontes](#-curadoria-de-fontes) • [🛠️ Engenharia de Prompts](#%EF%B8%8F-engenharia-de-prompts-e-cicatrizes) • [🎬 Vídeo Complementar](https://youtu.be/NKIsmVbg9I8)

</div>

---

## 📌 Sumário
- [Contexto e Objetivos](#-contexto-e-objetivos)
- [Curadoria de Fontes](#-curadoria-de-fontes)
- [Engenharia de Prompts e "Cicatrizes"](#%EF%B8%8F-engenharia-de-prompts-e-cicatrizes)
- [Entrega Principal: Miniguia de Estudo (Manual Prático)](#-entrega-principal-miniguia-de-estudo-manual-pr%C3%A1tico)
  - [Visão Geral e Arquivo PDF](#-arquivo-do-manual-pr%C3%A1tico)
  - [Resumo Estruturado e Indicadores](#1-resumo-estruturado-dos-fiis)
  - [Estudo de Caso Prático (EXPLO11)](#2-exerc%C3%ADcio-pr%C3%A1tico-fundo-fict%C3%ADcio-explo11)
  - [Glossário de Conceitos](#3-gloss%C3%A1rio-de-conceitos)
  - [Prompts Reutilizáveis para Estudo](#4-prompts-reutiliz%C3%A1veis-para-estudo)
- [Recurso Multimídia Adicional (Vídeo/Podcast)](#-recurso-multim%C3%ADdia-adicional)
- [Autor](#-autor)

---

## 🎯 Contexto e Objetivos

Este projeto foi desenvolvido como parte do desafio prático do **Bootcamp Bradesco - GenAI, Dados & Cyber** promovido pela **DIO**. O intuito é utilizar a IA Generativa (NotebookLM / Gemini) como uma ferramenta ativa de curadoria, síntese e estruturação do conhecimento.

### **Objetivo Principal**
* Capacitar qualquer pessoa leiga a realizar a **análise fundamentalista de Fundos de Investimento Imobiliário (FIIs)** a partir do zero.

### **Objetivos Complementares**
1. Compreender a estrutura, funcionamento e categorias de FIIs (Tijolo, Papel, FoFs e Híbridos).
2. Ler, interpretar e cruzar indicadores financeiros essenciais (P/VP, DY, Vacância Física vs. Financeira, Cap Rate, WALT, LTV).
3. Avaliar a qualidade de um fundo através do estudo de relatórios gerenciais e análise de cenários macroeconômicos.

---

## 📚 Curadoria de Fontes

A seleção das fontes utilizou o recurso **Deep Search** do NotebookLM (Gemini Notebook). A partir de uma busca inicial que retornou 16 resultados, foram selecionados 3 materiais de alta reputação do mercado financeiro:

| Instituição / Portal | Tópico Abordado | Link de Acesso |
| :--- | :--- | :--- |
| **Mais Retorno** | 10 indicadores fundamentais para análise de FIIs | [Acessar Artigo](https://maisretorno.com/portal/10-indicadores-dos-fundos-imobiliarios-que-voce-precisa-conhecer-antes-de-investir) |
| **XP Investimentos** | Metodologia completa de análise de FIIs | [Acessar Relatório](https://conteudos.xpi.com.br/fundos-imobiliarios/relatorios/como-analisar-fundos-imobiliarios/) |
| **Banco Daycoval** | Passo a passo e conceitos introdutórios | [Acessar Artigo](https://blog.daycoval.com.br/como-analisar-um-fii/) |

---

## 🛠️ Engenharia de Prompts e "Cicatrizes"

A construção do caderno temático passou por um processo iterativo de refinamento de prompts (*Troubleshooting*) utilizando o **Gemini 3.1 Pro**.

### 📉 Matriz de Erros e Aprendizados (*Post-Mortem*)

| Tentativa | Prompt Utilizado / Intenção | Resultado Ocorrido | Diagnóstico & Lição Aprendida |
| :---: | :--- | :--- | :--- |
| **1ª** | Busca por *PDFs completos da CVM/B3 cobrindo do básico ao Valuation*. | ❌ **0 resultados** retornados. | **Prompt Hiper-restritivo:** Exigir múltiplos critérios rígidos travou a busca. |
| **2ª** | Busca por *documentos que ensinem tudo sobre FIIs para iniciantes*. | ⚠️ Sugestões de focos genéricos. | **Vício de Formato:** Exigir "para iniciantes" descartou artigos técnicos valiosos. |
| **3ª** | *"Metodologias e princípios de análise fundamentalista de Fundos de Investimento Imobiliário (FIIs)."* | ✅ **16 fontes qualificadas**. | **Matéria-prima Pura:** Buscar conteúdo técnico bruto para que a IA traduza depois. |

> [!IMPORTANT]
> **Lição Aprendida:** Separe a fase de **Coleta de Dados** da fase de **Sintetização Didática**. Na busca inicial, utilize prompts focados na matéria-prima técnica; no chat do caderno, solicite a simplificação para linguagem didática.

---

## 📖 Entrega Principal: Miniguia de Estudo (Manual Prático)

### 📄 Arquivo do Manual Prático
A entrega central e produto final deste desafio é o miniguia em PDF gerado diretamente via NotebookLM a partir do processo de síntese e prompts personalizados em português:

👉 **[Download / Visualizar o Manual Prático (PDF)](./Manual_Pratico_FIIs.pdf)**

---

### 1. Resumo Estruturado dos FIIs

Os **Fundos Imobiliários (FIIs)** democratizaram o mercado imobiliário brasileiro ao permitir que investidores acessem ativos de alto padrão com baixo capital inicial e isenção de Imposto de Renda sobre os rendimentos mensais (para pessoas físicas).

```
[ Investidor ] ──( Compra Cotas )──> [ Fundo Imobiliário ] ──( Adquire )──> [ Imóveis / Títulos ]
       ▲                                                                            │
       └──────────────────( Recebe Aluguéis / Juros )──────────────────────────────┘
```

#### **Categorias e Especificidades Técnicas**
* **Fundos de Tijolo:** Imóveis físicos (Shoppings, Galpões Logísticos, Lajes Corporativas). Renda advinda dos aluguéis.
* **Fundos de Papel (Recebíveis):** Títulos de dívida imobiliária (CRI, LCI). Exigem análise de crédito, tranches (Sênior, Mezanino, Subordinada) e **LTV (Loan-to-Value)**.
* **Fundos de Fundos (FoFs):** Investem em cotas de outros FIIs, garantindo diversificação instantânea.
* **Híbridos:** Combinam ativos imobiliários físicos com títulos de crédito.

---

### 2. Painel de Controle de Indicadores

| Indicador | O que avalia? | Leitura / Critério |
| :--- | :--- | :--- |
| **P/VP** | Preço da Cota vs. Valor Patrimonial | `= 1` (Preço justo), `< 1` (Deságio/Desconto), `> 1` (Ágio/Caro) |
| **Dividend Yield (DY)** | Retorno em proventos | Avaliar histórico de 12m para verificar consistência da renda |
| **Vacância (Física x Financeira)** | Espaço desocupado x Perda de receita | Vacância física baixa com financeira alta indica concessão excessiva de carências |
| **WALT to Break / Expiry** | Média do prazo dos contratos | *WALT to Break* mede a primeira janela de saída sem multa (previsibilidade real) |
| **Absorção Líquida** | Variação de m² ocupados vs. devolvidos | Se positiva, indica expansão da ocupação no fundo/mercado |

---

### 3. Exercício Prático: Fundo Fictício "EXPLO11"

Para consolidar o aprendizado, o manual prático realiza a análise passo a passo de um fundo fictício de Tijolo (Logístico):

* **Dados do EXPLO11:** Cota: R$ 100,00 | VP: R$ 110,00 | DY (12m): 10% a.a. | Vacância Física: 2% | WALT to Break: 6 anos (Contratos Atípicos) | Portfólio: 5 Galpões AAA em SP/MG.
* **Análise:**
  1. *P/VP:* $100 / 110 = 0,90$ (Comprado com 10% de desconto patrimonial).
  2. *Yield:* 10% a.a., retorno real robusto e recorrente.
  3. *Risco/Qualidade:* Imóveis AAA de alta liquidez com contratos atípicos de longo prazo protegidos por multas severas.
* **Conclusão:** O EXPLO11 representa uma oportunidade clara, onde o deságio de 10% (P/VP 0,90) decorre do pessimismo do mercado e não de fundamentos ruins do fundo.

---

### 4. Glossário de Conceitos

* **Cota:** A menor fração do patrimônio do fundo.
* **CapEx (Capital Expenditure):** Investimentos em melhorias e modernização dos imóveis.
* **LTV (Loan-to-Value):** Razão entre a dívida e o valor da garantia (abaixo de 50% indica margem saudável).
* **CRI (Certificado de Recebíveis Imobiliários):** Título de dívida imobiliária que compõe a carteira dos fundos de papel.
* **IFIX:** Índice benchmark do mercado de FIIs na B3.

---

### 5. Prompts Reutilizáveis para Estudo

Utilize estas perguntas orientadoras no chat do seu **NotebookLM** para analisar novos relatórios gerenciais:

1. *"Apresente-me todos os indicadores deste FII, ensinando-me a analisar um a um com definições e exemplos práticos."*
2. *"Explique, de modo didático, os tipos de contratos de locação (típicos vs. atípicos) presentes neste relatório e os pontos de atenção."*
3. *"Ensine, passo a passo, como um investidor leigo deve ler a seção de DRE (Demonstração do Resultado do Exercício) deste fundo."*
4. *"Monte um quadro comparativo elencando os riscos específicos e as oportunidades identificadas na tese deste fundo."*

---

## 🎬 Recurso Multimídia Adicional

Além do miniguia principal em PDF, foi gerado como **produto adicional** um vídeo/podcast em áudio no NotebookLM para primeira aproximação ao tema.

* 🎬 **Assistir ao Vídeo no YouTube:** [Introdução Didática aos FIIs](https://youtu.be/NKIsmVbg9I8)

---

## 👤 Autor

Desenvolvido por **Diego de Oliveira**  
*Estudante do Bootcamp Bradesco - GenAI, Dados & Cyber da DIO.*
