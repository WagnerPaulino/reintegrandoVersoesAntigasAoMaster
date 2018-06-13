**1.** Para fazer um branch de um commit especifico

```bash
git checkout -b test-branch 859bba32efc812a1a69cd66b1fe3d5e9321fa493
```

**2.** Apos fazer as alterações fazer a adições de suas alterações e o commit

```bash
git add . 
git commit -m ""
```

**3.** Troque para o branch master 

```bash
git checkout master
```

**4.** Execute o seguinte comando para começar a fazer a reintegração com master

```bash
git rebase test-branch
```

**5.** Resolva os conflitos adicione a resolução ao git

```bash
git add . 
```

**6.** Execute o seguinte comando para que o git vá para o proximo commit 

```bash
git rebase --continue
```

**7.** Faça a adição das alterações

```bash
git add . 
```

**8.** Execute o camando caso haja algo que queira manter 

```bash
git rebase --continue
```

**9.** Caso queira pular as alterações que apareceram como conflite digite o seguinte comando

```bash
git rebase --skip
```

**10.** Execute esse processo até que acabe os commits e você chegue no ultimo commit feito no master
