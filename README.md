# MedAgenda · Plano de Testes e Validação

Testes e validação do MedAgenda, sistema web de uma clínica médica: agendamento de consultas,
atendimento com prontuário, documentos em PDF, notificações, assistente virtual e relatórios.

Projeto da disciplina **Teste de Software (2026.2)**, Sistemas de Informação, UNIFACISA.
Prof. Bruno Rafael Araújo Vasconcelos.

## Equipe

- Felipe Renan dos Santos Ferreira
- Mateus Patrício Vasconcelos
- Renata Cardoso Mantovani

## Como executar o MedAgenda (Docker)

Na pasta do pacote `medagenda.zip`, disponibilizado pelo professor:

```bash
docker compose up --build
```

| Serviço | Endereço |
|---|---|
| Sistema | http://localhost:8080 |
| API | http://localhost:3000/api |
| MongoDB | mongodb://localhost:27017 |

Para voltar os dados ao estado inicial:

```bash
docker compose exec api npm run seed
```

## Estrutura

O código do MedAgenda não é alterado. Os testes do grupo ficarão na pasta `tests/`,
que será adicionada nas próximas entregas:

```
tests/api     testes de API e permissões
tests/e2e     testes de interface
tests/bdd     cenários Gherkin
tests/carga   teste de desempenho
tests/a11y    acessibilidade
```
