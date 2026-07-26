# carapicu-model
Descrever....
# carapicu-prompt
## Prompt Used to Generate the Carapicu-textbook Dataset

The **Carapicu-textbook** dataset was generated using the GPT-4o-mini API. Each section of the **BPLN NLP textbook** was independently submitted to the model together with the following prompt to generate question–answer pairs.

### Context

Você é um(a) pesquisador(a) e professor(a) especialista em Processamento de Linguagem Natural (PLN). Sua tarefa é gerar **20 pares de perguntas e respostas** sobre o conteúdo do texto fornecido, extraído de um livro-texto técnico de PLN em português.

As perguntas e respostas devem refletir conceitos centrais, fundamentos, técnicas e aplicações da área, de forma didática, coerente e cientificamente correta.

### Generation Instructions

1. Leia atentamente o texto fornecido.
2. Gere **20 pares de perguntas e respostas** em português formal e técnico.
3. Organize as perguntas em três grupos temáticos:
   - **Fundamentos e Conceitos**
   - **Técnicas e Modelos**
   - **Aplicações e Desafios**
4. Cada resposta deve ser objetiva e baseada exclusivamente no conteúdo do texto.
5. Não gere respostas que dependam da localização no livro.
6. Evite perguntas que sejam simples paráfrases do texto.
7. Gere perguntas envolvendo definições, comparações, relações de causalidade, descrições, motivações e justificativas.
8. Utilize linguagem acadêmica clara.
9. Apresente o resultado em formato **JSON**.
10. Mesmo que o texto esteja em inglês, gere todas as perguntas e respostas em português.

---

## Expected Output Format (JSON)

```json
{
  "Fundamentos e Conceitos": [
    {
      "pergunta": "...",
      "resposta": "..."
    }
  ],
  "Tecnicas e Modelos": [
    {
      "pergunta": "...",
      "resposta": "..."
    }
  ],
  "Aplicacoes e Desafios": [
    {
      "pergunta": "...",
      "resposta": "..."
    }
  ]
}
```
# Citation / Reference Context

## Citation

If you use this repository in your research, please cite:

```bibtex
@inproceedings{gomes-claro-att-multidomain-bracis2026,
  title        = {Grammatical Representations in Transformer Attention: A Multidomain Study of Portuguese via UD},
  author       = {Ricardo Gomes de Oliveira and Daniela Barreiro Claro and Rerisson Cavalcante de Araújo},
  year         = 2026,
  month        = {October},
  booktitle    = {Proceedings of the 36th Brazilian Conference on Intelligent Systems},
  publisher    = {Springer},
  address      = {New York, NY},
  pages        = {},
  organization = {SBC}
}
