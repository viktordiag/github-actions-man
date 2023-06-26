# github-actions-man  
***структура*** \
name: \
on: \
jobs:
+ \<ID jobs\>:

## `name:` имя рабочего процесса ##
## `on:`  триггер запускающий рабочий процесс ##
* `on: workflow_dispatch` запускает тесты вручную
* `on: push` запускает тесты при внесении изменений в репозиторий 
## `jobs:` задания ##
рабочий процесс ***workflow*** состоит из одного или нескольких заданий ***jobs*** которые по умолчанию выполняются параллельно <br>
