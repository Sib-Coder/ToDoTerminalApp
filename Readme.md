# Консольный трекер задач


## Для начала работы 
```bash
> git clone 
> go get "github.com/alexeyco/simpletable"
```
## Режимы работы:
1) add Режим добавления (на вход принимает флаг -add и строку с задачей):
```golang
> go run .\main.go -add Праздник для детей
```
2) done Режим выполнено (на вход принимает флаг -done и индекс задачи):
```golang
> go run .\main.go -done 1
```
3) del Режим удаления (на вход принимает флаг -del и индекс задачи):
```golang
> go run .\main.go -del 1 
```
4) list Режим показа (на вход принимает флаг -list / возвращает таблицу с задачами):
```golang
> go run .\main.go -list  
>
╔═══╤════════════════════╤═══════╤═════════════════════╤═════════════════════╗
║ # │        Task        │ Done? │           CreatedAt │         CompletedAt ║
╟━━━┼━━━━━━━━━━━━━━━━━━━━┼━━━━━━━┼━━━━━━━━━━━━━━━━━━━━━┼━━━━━━━━━━━━━━━━━━━━━╢
║ 1 │ ✔ Мои дела         │ yes   │ 09 Jul 23 12:52 +07 │ 09 Jul 23 13:02 +07 ║
║ 2 │ Праздник для детей │ no    │ 09 Jul 23 12:53 +07 │ 01 Jan 01 00:00 UTC ║
╟━━━┼━━━━━━━━━━━━━━━━━━━━┼━━━━━━━┼━━━━━━━━━━━━━━━━━━━━━┼━━━━━━━━━━━━━━━━━━━━━╢
║                          You have 1 pending todos                          ║
╚═══╧════════════════════╧═══════╧═════════════════════╧═════════════════════╝

```
## Пример работы в Консоли