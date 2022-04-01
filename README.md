# xmlSync_schtasks
scripting create tasks for xmlSync (wmn)



# Installation with command line

```shell
schtasks /create /tn xmlSyncTasks /tr "C:\wayssoft\Environment\services\xmlSync.exe" /sc daily /st 10:00:00
```

# Installation with xml File

```shell
schtasks /create /tn xmlSyncTasks /XML "C:\wayssoft\Environment\services\xmlSyncTasks.xml"

```

# List tasks for csv

```shell
schtasks /query /fo csv >> "C:\wayssoft\Environment\logs\schtasks.csv"

```

## ATENÇÃO 

<br />
Lembre-se de trocar o nome da tarefa na tag /tn, caso queira criar mais de uma tarefa.
<br />
Ex: xmlSyncTasks_01


<br /><br />
## TESTADO EM:
windows 7
