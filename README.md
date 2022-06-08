# pipebank
a simple program to store and retrieve named binary streams

```bash
Usage: [|] pipebank <command> [key] [|]
Commands:
  set/put/send/save [key]
  get <key>
  fetch <key> - get and delete
  delete/rm <key>
  list/ls
  clear
```

```bash
$ cat recipe.txt | pipebank save fluffy-pizza
$ pipebank fetch fluffy-pizza | grep -i secret
```

```bash
$ ls | pipebank send
#Saved as Y7E2
$ pipebank fetch Y7E2 | sort
```