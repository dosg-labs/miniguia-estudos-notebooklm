<div align="center">

# 📊 Treinando uma IA de Aprendizagem: Análise Fundamentalista de FIIs

![DIO](https://img.shields.io/badge/DIO-Bootcamp%20Bradesco-red?style=for-the-badge)
![AI](https://img.shields.io/badge/NotebookLM-Gemini%203.1%20Pro-blue?style=for-the-badge)
![Domain](https://img.shields.io/badge/Finan%C3%A7as-FIIs-green?style=for-the-badge)
![Status](https://img.shields.io/badge/Status-Conclu%C3%ADdo-brightgreen?style=for-the-badge)

*Um guia prático e documentação de engenharia de prompts criando um caderno temático de estudos no NotebookLM.*

[📺 Assistir Vídeo Explicativo no YouTube](https://youtu.be/NKIsmVbg9I8) • [📚 Ver Fontes](#-curadoria-de-fontes) • [🛠️ Engenharia de Prompts](#%EF%B8%8F-engenharia-de-prompts-e-cicatrizes)

</div>

---

## 📌 Sumário
- [Contexto e Objetivos](#-contexto-e-objetivos)
- [Curadoria de Fontes](#-curadoria-de-fontes)
- [Engenharia de Prompts e "Cicatrizes"](#%EF%B8%8F-engenharia-de-prompts-e-cicatrizes)
- [Miniguia de Estudo (Entrega Final)](#-miniguia-de-estudo-entrega-final)
  - [Resumo Estruturado dos FIIs](#1-resumo-estruturado)
  - [Principais Indicadores](#2-indicadores-essenciais)
  - [Glossário do Investidor](#3-gloss%C3%A1rio-de-conceitos)
  - [Prompts Reutilizáveis](#4-prompts-reutiliz%C3%A1veis-para-estudo)
- [Resultados Multimídia](#-resultados-multim%C3%ADdia)
- [Autor](#-autor)

---

## 🎯 Contexto e Objetivos

Este projeto foi desenvolvido como parte do desafio prático do **Bootcamp Bradesco - GenAI, Dados & Cyber** promovido pela **DIO**. O intuito é utilizar a IA Generativa (NotebookLM / Gemini) não apenas como gerador de texto, mas como uma ferramenta ativa de curadoria, síntese e aprendizado contínuo.

### **Objetivo Principal**
* Capacitar qualquer pessoa leiga a realizar a **análise fundamentalista de Fundos de Investimento Imobiliário (FIIs)** a partir do zero.

### **Objetivos Complementares**
1. Compreender a estrutura, funcionamento e categorias de FIIs.
2. Ler, interpretar e cruzar indicadores financeiros essenciais.
3. Avaliar criticamente a saúde de um fundo antes de tomar decisões de investimento.

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

A construção da base de conhecimento passou por um processo iterativo de *Troubleshooting* de prompts com o auxílio do **Gemini 3.1 Pro**.

### 📉 Matriz de Erros e Aprendizados (*Post-Mortem*)

| Tentativa | Prompt Utilizado / Intenção | Resultado Ocorrido | Diagnóstico & Lição Aprendida |
| :---: | :--- | :--- | :--- |
| **1ª** | Busca por *PDFs completos da CVM/B3 cobrindo do básico ao Valuation*. | ❌ **0 resultados** retornados. | **Prompt Hiper-restritivo:** Tentar achar o "documento perfeito" travou o motor de busca. |
| **2ª** | Busca por *documentos que ensinem tudo sobre análise de FIIs para iniciantes*. | ⚠️ Sugestão de focos muito genéricos. | **Vício de Formato:** Exigir termos como "iniciante" descartava artigos técnicos valiosos. |
| **3ª** | *"Metodologias e princípios de análise fundamentalista de Fundos de Investimento Imobiliário (FIIs)."* | ✅ **16 fontes qualificadas**. | **Matéria-prima Pura:** Buscar conteúdo técnico bruto para que a IA traduza depois. |

> [!IMPORTANT]
> **Lição de Engenharia de Prompts:** Separe a fase de **Coleta de Dados** da fase de **Sintetização Didática**. Na busca, foque na densidade técnica do assunto; no chat interno do caderno, peça para a IA adaptar o tom para iniciantes.

---

## 📖 Miniguia de Estudo (Entrega Final)

### 1. Resumo Estruturado

Os **Fundos Imobiliários (FIIs)** representam uma forma acessível de investir no mercado imobiliário sem a necessidade de comprar um imóvel físico diretamente.

```
[ Investidor ] ──( Compra Cotas )──> [ Fundo Imobiliário ] ──( Adquire )──> [ Imóveis / Títulos ]
       ▲                                                                            │
       └──────────────────( Recebe Aluguéis / Juros )──────────────────────────────┘
```

#### **Categorias de FIIs**
* **Fundos de Tijolo:** Investem em imóveis físicos (Shopping Centers, Galpões Logísticos, Prédios Corporativos, Hospitais).
* **Fundos de Papel:** Investem em títulos de dívida do setor imobiliário (CRI, LCI). Recebem juros e correção monetária.
* **Fundos de Fundos (FoFs):** Investem em cotas de outros FIIs, oferecendo diversificação imediata.

---

### 2. Indicadores Essenciais

| Indicador | O que mede? | Sinal de Tranquilidade | Sinal de Alerta |
| :--- | :--- | :--- | :--- |
| **P/VP** | Preço da Cota / Valor Patrimonial | Próximo de **1,00** | Muito acima de **1,10** (caro) ou abaixo de **0,70** (risco oculto) |
| **DY (Dividend Yield)** | Retorno em proventos | Consistente e alinhado aos pares | DY desproporcionalmente alto (ganho não recorrente) |
| **Vacância Física** | Imóveis desocupados | Abaixo de **10%** | Crescimento contínuo acima de **20%** |
| **Liquidez Diária** | Facilidade de comprar/vender | Alto volume diário de negociação | Baixo volume (dificuldade de resgate) |

---

### 3. Glossário de Conceitos

* **Cota:** A menor fração do patrimônio do fundo.
* **Cotista:** O investidor que possui cotas e tem direito ao recebimento dos rendimentos distribuídos.
* **IFIX:** O principal índice da B3 que mede o desempenho médio dos FIIs no mercado.
* **Relatório Gerencial:** Documento publicado mensalmente pelo gestor apresentando resultados financeiros, taxa de ocupação e estratégias do fundo.

---

### 4. Prompts Reutilizáveis para Estudo

Copie e cole estas perguntas no chat do seu **NotebookLM** para destrinchar relatórios gerenciais e analisar fundos específicos:

1. *"Apresente-me todos os indicadores deste FII, ensinando-me a analisar um a um com definições e exemplos práticos."*
2. *"Explique, de modo didático, os tipos de contratos de locação (típicos vs. atípicos) presentes neste relatório e os pontos de atenção."*
3. *"Ensine, passo a passo, como um investidor leigo deve ler a seção de DRE (Demonstração do Resultado do Exercício) deste fundo."*
4. *"Monte um quadro comparativo elencando os riscos específicos e as oportunidades identificadas na tese deste fundo."*

---

## 🎬 Resultados Multimídia

Além dos resumos estruturados no caderno, a experiência gerou entregáveis práticos de aplicação:

1. **Relatório Customizado:** Manual Prático de Metodologia Fundamentalista gerado com instruções de linguagem didática em PT-BR e simulação de análise de um fundo fictício.
2. **Podcast / Vídeo Explicativo:** Material em vídeo gerado para introdução dinâmica ao universo dos FIIs.
   * 🎬 **Assista aqui:** [Vídeo Completo no YouTube](https://youtu.be/NKIsmVbg9I8)

> [!TIP]
> **Oportunidade de Melhoria:** Em um cenário ideal, a integração do agente com fontes de dados em tempo real (como *Investidor 10* ou *Status Invest*) enriqueceria as simulações com cotações e proventos atualizados no dia.

---

## 👤 Autor

Desenvolvido por **Diego de Oliveira**  
*Estudante do Bootcamp Bradesco - GenAI, Dados & Cyber da DIO.*# miniguia-estudos-notebooklm
