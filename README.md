# github-actions-man  
***структура***
- name:
- on:
- jobs:
  - ***IDjobs***:
    - runs_on:

### `name:` имя рабочего процесса ###
### `on:`  триггер запускающий рабочий процесс ###
* `on: workflow_dispatch` запускает тесты вручную
* `on: push` запускает тесты при внесении изменений в репозиторий 
### `jobs:` задания ###
рабочий процесс ***workflow*** состоит из одного или нескольких заданий ***jobs*** которые по умолчанию выполняются параллельно <br>
### `IDjobs:` имя задания ###
произвольное имя задания ***jobs*** может использоваться как идентификатор задания при составлении сценариев
### `runs-on:` среда в которой запускается задание ***jobs*** ###
- `runs-on: ubuntu_latest` запускает ubuntu последней версии
