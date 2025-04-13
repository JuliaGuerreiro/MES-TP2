# Geração de Mensagens de Commit com LLMs: Uma Análise Quantitativa e Qualitativa

Este repositório contém a proposta e os experimentos relacionados ao Trabalho Prático 2 (TP2) da disciplina *Manutenção e Evolução de Software*. 

---

## 👩‍💻 Aluna

- Júlia Guerreiro – Mestrado em Ciência da Computação

---

## 🔍 Objetivo

Modelos de linguagem de grande porte, como o ChatGPT, vêm sendo explorados para diversas tarefas dentro do ciclo de desenvolvimento de software. Este trabalho propõe avaliar a eficácia desses modelos na geração de mensagens de commit, analisando se os textos gerados são informativos, coerentes e aderentes às mudanças no código. A ideia é entender como as LLMs podem contribuir (ou não) para tarefas de documentação automatizada dentro de um fluxo de versionamento.

---

## ⚙️ Metodologia

### Modelo de Linguagem Utilizado

- **Principal:** ChatGPT-4 (OpenAI)

### Dataset

- Aproximadamente 50 a 100 instâncias de commits
- Coletados de repositórios open-source no GitHub
- Linguagens: Python e JavaScript
- Critérios:
  - Projetos ativos nos últimos 12 meses
  - Commits com mensagens claras
  - Diversidade de alterações (correções, refatorações, novas features)

### Exemplos Preliminares de Prompt

- **Zero-shot:**
  > “A partir do diff a seguir, gere uma mensagem de commit adequada.”
---

## 📊 Avaliação Quantitativa

- **BLEU Score** – Similaridade lexical
- **ROUGE** – Cobertura de termos importantes
- **Cosine Similarity** – Similaridade semântica (com Sentence-BERT)

---

## 🧠 Avaliação Qualitativa

- Clareza e coesão
- Adequação ao conteúdo do diff
- Nível informativo
- Análise manual de casos bons e ruins
