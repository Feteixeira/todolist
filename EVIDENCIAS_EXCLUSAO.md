# Evidências — Fluxo de Confirmação de Exclusão

Este documento reúne as evidências do fluxo de exclusão segura de tarefas, implementado com
`AlertDialog` (Jetpack Compose Material 3) na tela `ListaTarefasScreen`.

## 1. Lista antes da exclusão

Tela inicial exibindo a tarefa que será excluída, ainda presente na lista.

![Lista antes da exclusão](docs/images/exclusao/01-lista-antes.png)

## 2. Diálogo aberto com a tarefa selecionada

Ao tocar no ícone de lixeira, o `AlertDialog` é exibido sobre a própria tela da lista,
informando claramente qual tarefa (pelo título) será excluída.

![Diálogo de confirmação aberto](docs/images/exclusao/02-dialogo-aberto.png)

## 3. Resultado ao cancelar

Ao tocar em **Cancelar**, o diálogo é fechado e a tarefa permanece na lista, sem nenhuma alteração.

![Resultado após cancelar](docs/images/exclusao/03-resultado-cancelar.png)

## 4. Nova abertura do diálogo

O ícone de lixeira é tocado novamente na mesma tarefa, reabrindo o diálogo de confirmação.

![Diálogo aberto novamente](docs/images/exclusao/04-dialogo-reaberto.png)

## 5. Resultado após confirmar a exclusão

Ao tocar em **Excluir**, o diálogo é fechado e a tarefa é removida definitivamente da lista —
apenas a tarefa selecionada é excluída, as demais permanecem intactas.

![Resultado após confirmar exclusão](docs/images/exclusao/05-resultado-excluir.png)