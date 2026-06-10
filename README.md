# 🏦 Prompt de Análise de Feedbacks Bancários

> Prompt de engenharia para análise inteligente de feedbacks de clientes em canais digitais bancários — focado em CX, segurança da informação e inteligência operacional acionável.

---

## 📌 Sobre o Projeto

Este repositório contém um prompt estruturado para uso com modelos de linguagem (LLMs) como o Claude ou ChatGPT, desenvolvido para atuar como um **analista de dados sênior** especializado em **Experiência do Cliente (CX)** e **Segurança da Informação** no setor bancário.

O objetivo é transformar feedbacks brutos de clientes em **inteligência acionável** para times de produto e operações.

---

## 🎯 Casos de Uso

- Priorização de correções críticas em sistemas de transação
- Identificação de falhas recorrentes no aplicativo
- Detecção de riscos de engenharia social e fraudes
- Redução de insatisfação severa com base em evidências textuais

---

## 🔍 Canais Analisados

| Canal         | Exemplos de Produtos |
|---------------|----------------------|
| Aplicativo    | Login, Notificações  |
| Pix           | Transferências, Chaves |
| Cartão        | Crédito, Débito      |
| Chat          | Atendimento humano e bot |

---

## 📥 Dados de Entrada Esperados

O prompt espera uma base de feedbacks com as seguintes colunas:

| Campo              | Descrição                          |
|--------------------|------------------------------------|
| `data`             | Data do comentário                 |
| `canal`            | Canal de atendimento               |
| `feedback`         | Texto livre do cliente             |
| `produto`          | Produto ou funcionalidade citada   |
| `nota`             | Satisfação de 1 (péssimo) a 5 (ótimo) |

---

## 📤 Formato da Resposta Gerada

O modelo retornará:

1. **Resumo Executivo** — até 5 linhas com o cenário geral
2. **Tabela de Insights** — `Tema | Sentimento | Urgência | Evidência | Ação Sugerida`
3. **Plano de Ação Prioritário** — top 3 correções críticas imediatas

---

## 🔐 Restrições e Segurança

- ✅ Análise baseada **exclusivamente** nos dados fornecidos
- 🚫 Nenhuma métrica ou problema é inventado
- 🔒 **PII mascarado automaticamente** (CPF, cartão, telefone, nome)
- ⚠️ Limitações de dados sinalizadas explicitamente na resposta

---

## 🚀 Como Usar

1. Copie o conteúdo do arquivo [`prompt.md`](./prompt.md) *(ou o bloco abaixo)*
2. Cole em sua LLM preferida (Claude, ChatGPT, Gemini etc.)
3. Adicione os dados de feedbacks no final do prompt
4. Execute e receba a análise estruturada

---

## 🧠 Prompt Completo

<details>
<summary>Clique para expandir o prompt</summary>
