Você está executando correção estrutural dos artefatos gerados.

A saída anterior violou contratos obrigatórios.

Sua tarefa é corrigir apenas a estrutura necessária.

---

# Contexto

{{CONTEXT_JSON}}

---

# Artefatos atuais

{{CURRENT_OUTPUT_JSON}}

---

# Erros detectados

{{CONTRACT_ERRORS_JSON}}

---

# Regras obrigatórias

Preserve o conteúdo existente sempre que possível.

Corrija apenas o necessário.

Não invente novo domínio.

Mantenha aderência a:

- Schola
- ProdOps
- turmas
- matrícula
- pagamento
- Certificare

---

# Regras estruturais

## requirements_md

Deve conter **no mínimo 10 requisitos**.

Cada requisito deve começar com:

## RF-001
## RF-002
...
## RF-010

Cada requisito deve conter pelo menos:

- Objetivo
- Descrição
- Regras de negócio
- Critérios de aceitação
- Rastreabilidade

---

## non_functional_md

Deve conter:

- Segurança
- Performance
- Confiabilidade
- Observabilidade

---

## glossary_md

Deve conter tabela markdown válida com **pelo menos 5 termos**.

---

## assumptions_md

Deve conter **pelo menos 3 suposições**:

AS-001 ...
Justificativa: ...

AS-002 ...
Justificativa: ...

AS-003 ...
Justificativa: ...

---

## handoff_md

Deve conter:

- Entradas
- Próximo passo
- Pontos críticos

---

# Regra crítica de saída

Responda **SOMENTE em JSON válido**.

Não escreva texto fora do JSON.

---

# Estrutura obrigatória da resposta

{
  "requirements_md": "markdown completo",
  "non_functional_md": "markdown completo",
  "glossary_md": "markdown completo",
  "assumptions_md": "markdown completo",
  "handoff_md": "markdown completo"
}