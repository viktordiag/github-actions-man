# github-actions-man  
***структура***
- name: Print
- on: workflow_dispatch
- jobs:
  - ***IDjobs***:
    - runs_on: ubuntu_latest
    - steps:
      - \- name: Print to console
        - run: echo Hello GitHub Actions

### `name:` имя рабочего процесса ###
### `on:`  триггер запускающий рабочий процесс ###
* `on: workflow_dispatch` запускает тесты вручную
* `on: push` запускает тесты при внесении изменений в репозиторий 
### `jobs:` далее перечисляем задания ###
рабочий процесс ***workflow*** состоит из одного или нескольких заданий ***jobs*** которые по умолчанию выполняются параллельно <br>
### `IDjobs:` имя задания ###
произвольное имя задания ***jobs*** может использоваться как идентификатор задания при составлении сценариев
### `runs-on:` среда в которой запускается задание ***jobs*** ###
- `runs-on: ubuntu_latest` запускает ubuntu последней версии
### `steps:` далее перечисляем шаги ###
***jobs*** может состоять из нескольких шагов
### `- name:` произвольное имя шага ###
`- name: Print to console`
### `run:` действие которое необходимо выполнить  ###
`run: |` позволяет ввести несколько команд 
```
run: | 
  echo first line
  echo second line
```



