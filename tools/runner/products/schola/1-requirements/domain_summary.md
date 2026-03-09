**Domain Summary**

## Objetivo do produto

O objetivo principal do Schola é permitir que uma pessoa veja turmas abertas, faça matrícula e tenha a matrícula confirmada após confirmação de pagamento.

## Atores

* Aluno
* Admin ProdOps
* Sistema Pagamento

## Entidades principais

* Turmas
* Matrículas
* Pagamentos

## Integrações externas

* Autenticação e cadastro delegados para Certificare
* Recebimento de confirmação de pagamento via webhook

## Eventos externos

* Confirmação de pagamento

## Fluxos principais

1. O aluno se autenticar com o Certificare.
2. O Schola lista turmas abertas do curso de ProdOps.
3. O aluno solicita matrícula em uma turma.
4. O sistema verifica a disponibilidade da turma e confirma a matrícula após recebimento de confirmação de pagamento.

## Restrições

* Não duplicar cadastro local
* Confirmação de pagamento deve ser idempotente
* Toda confirmação deve ser auditável

## Dúvidas abertas

* Como o Schola irá lidar com a integridade dos dados em caso de falha do sistema?
* Quais são as implicações da delegação de autenticação e cadastro para Certificare?

## Regras de qualidade

O resumo deve refletir o domínio correto, capturar o fluxo principal do produto, destacar restrições reais e deixar explícitas as ambiguidades.
