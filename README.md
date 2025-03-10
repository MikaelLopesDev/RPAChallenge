# RPAChallenge - UiPath

## Descrição
Este projeto UiPath foi desenvolvido para resolver o **RPA Challenge**, um desafio onde os seletores dos campos mudam dinamicamente a cada execução. O objetivo é automatizar o preenchimento correto dos campos, garantindo que a automação funcione independentemente das alterações dos seletores.

## Requisitos
Antes de executar o projeto, certifique-se de ter os seguintes requisitos atendidos:
- UiPath Studio **25.0.161.0** ou superior.
- Orchestrator configurado com acesso à Cloud.
- Dependências instaladas:
  - `UiPath.Excel.Activities` (versão: **2.25.1-preview**)
  - `UiPath.System.Activities` (versão: **25.2.1**)
  - `UiPath.Testing.Activities` (versão: **24.10.4**)
  - `UiPath.UIAutomation.Activities` (versão: **25.2.1-preview**)

## Configuração
1. **Criar Fila no Orchestrator**
   - Crie uma fila no **Orchestrator** com o mesmo nome configurado no arquivo de configuração do projeto.

2. **Configurar a Pasta do Orchestrador**
   - No arquivo de configuração do projeto, altere o caminho da pasta do **Orchestrador** para corresponder à sua pasta na UiPath Cloud.

3. **Adicionar Asset no Orchestrator**
   - Nome: `urlChallenge`
   - Value: URL do desafio RPA Challenge
   - Folder: `Shared`

4. **Variáveis Utilizadas**
   - `nameFileToSave`: Define o nome do arquivo onde os dados serão salvos (**valor padrão**: `challenge.xlsx`)

## Como Executar
1. Abra o **UiPath Studio** e carregue o projeto.
2. Certifique-se de que todas as dependências estão instaladas.
3. Verifique e ajuste as configurações no **Orchestrator** conforme descrito acima.
4. Execute o fluxo principal `Main.xaml`.
5. Monitore os logs para verificar a execução e validação dos resultados.

---
**Versão do Projeto:** 1.0.0  
