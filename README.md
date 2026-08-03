<div align="center">

# 📊 Treinando uma IA de Aprendizagem: Análise Fundamentalista de FIIs

![DIO](https://img.shields.io/badge/DIO-Bootcamp%20Bradesco-red?style=for-the-badge)
![AI](https://img.shields.io/badge/NotebookLM-Gemini%203.1%20Pro-blue?style=for-the-badge)
![Domain](https://img.shields.io/badge/Finan%C3%A7as-FIIs-green?style=for-the-badge)
![Status](https://img.shields.io/badge/Status-Conclu%C3%ADdo-brightgreen?style=for-the-badge)

*Documentação de engenharia de prompts e caderno temático de estudos no NotebookLM para análise de Fundos Imobiliários.*

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
- [💡 Reflexões Críticas e Roadmap de Evolução (V2)](#-reflex%C3%B5es-cr%C3%ADticas-e-roadmap-de-evolu%C3%A7%C3%A3o-v2)
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

👉 **[Download / Visualizar o Manual Prático em PDF](https://github.com/dosg-labs/miniguia-estudos-notebooklm/blob/main/Manual%20Pr%C3%A1tico_%20O%20Caminho%20para%20Viver%20de%20Renda%20com%20Fundos%20Imobili%C3%A1rios%20(FIIs).pdf)**

---

### 1. Resumo Estruturado dos FIIs

Os **Fundos Imobiliários (FIIs)** democratizaram o mercado imobiliário brasileiro ao permitir que investidores acessem ativos de alto padrão com baixo capital inicial e isenção de Imposto de Renda sobre os rendimentos mensais (para pessoas físicas).
