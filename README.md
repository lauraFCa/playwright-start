[![Playwright Tests](https://github.com/lauraFCa/playwright-start/actions/workflows/playwright.yml/badge.svg)](https://github.com/lauraFCa/playwright-start/actions/workflows/playwright.yml)

**Visão Geral**
- **Projeto:** Playwright start — um repositório de exemplo para testes E2E com Playwright.
- **Objetivo:** Fornecer um ponto de partida rápido para escrever e executar testes usando Playwright em TypeScript.

**Pré-requisitos**
- **Node.js:** Versão LTS instalada (recomenda-se >= 16).
- **NPM/Yarn:** Gerenciador de pacotes disponível.

**Instalação**
- **Dependências:** Instale dependências do projeto.

```powershell
npm install
```

- **Browsers Playwright:** Instale navegadores necessários para os testes.

```powershell
npx playwright install
```

**Executando os testes**
- **Rodar todos os testes:** Executa a suíte completa com Playwright.

```powershell
npx playwright test
```

- **Rodar um arquivo específico:** Execute um teste isolado.

```powershell
npx playwright test tests/example.spec.ts
```

- **Comando via NPM (se existir script):** Use o script definido em `package.json` (ex.: `npm test`).

```powershell
npm test
```

**Relatórios**
- **Relatório HTML:** Após rodar os testes, o relatório é gerado em `playwright-report/index.html`.
- **Visualizar relatório via CLI:** Abra o relatório interativo.

```powershell
npx playwright show-report
```

**Estrutura do projeto**
- **`playwright.config.ts`:** Configurações do Playwright (projetos, timeouts, reporters).
- **`tests/`:** Pasta contendo os arquivos de teste (ex.: `tests/example.spec.ts`).
- **`playwright-report/`:** Relatório HTML estático gerado pelos testes.

**Dicas rápidas**
- **Executar em modo headed (com UI):** Adicione `--headed` ao comando de teste para ver os navegadores.

```powershell
npx playwright test --headed
```

- **Gravar um vídeo por falha:** Configure no `playwright.config.ts` ou use `--timeout`/`--retries` conforme necessário.


**Solução de problemas**
- **Testes não iniciam:** Verifique se os browsers foram instalados (`npx playwright install`) e se as dependências estão atualizadas.
- **Permissões/Antivírus:** Em alguns ambientes Windows, antivírus/Firewall podem bloquear o navegador automático.
