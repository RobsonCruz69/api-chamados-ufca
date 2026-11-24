# API de Chamados de Suporte — Atividade #1 (ADS0021)

## Identificação do Estudante
- **Nome completo:** Francisco Robson Paulino Cruz
- **Matrícula:** 2025014458
- **Curso:** Análise e Desenvolvimento de Sistemas / CEAD - Icó - Tecnológico - EAD - MTN

## Objetivo do Projeto
Criar a estrutura inicial de uma API REST de chamados de suporte em Python com Flask, utilizando o gerenciador `uv` para controle de ambiente virtual e dependências, expondo uma rota inicial de verificação de funcionamento (`GET /`).

## Instalação das Dependências
Certifique-se de ter o `uv` instalado e execute na raiz do projeto:

```bash
uv sync --locked
```

## Execução da Aplicação

Para executar localmente:

```bash
uv run flask --app app run
```

Para executar no GitHub Codespaces (ou expondo na rede):

```bash
uv run flask --app app run --host=0.0.0.0 --port=5000
```

## Acesso à Rota Inicial e Resposta Esperada
Com a aplicação em execução, faça uma requisição `GET` para `http://localhost:5000/` pelo navegador ou via terminal:

```bash
curl -i http://localhost:5000/
```

**Resposta esperada:**
- **Status HTTP:** `200 OK`
- **Cabeçalho:** `Content-Type: application/json`
- **Corpo (JSON):**

```json
{
  "mensagem": "API de chamados em funcionamento"
}
```