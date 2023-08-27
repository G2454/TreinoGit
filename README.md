# Tarefas

Lista de comandos que vamos utilizar

1. Baixar repositórios
```bash
git clone <https://link-com-o-nome-do-repositório>
```
2. Verificar se os arquivos foram modificados ou necessitam ser comitados 
```bash
git status
```
3. Incluir as alterações no próximo commit
```bash
git add <nome-do-arquivo>
```
4. Comandos relacionados a branch
- Lista todas as branch
```bash
git branch ou git branch --list
```
- Cria uma nova branch
```bash
git branch <nome-da-branch>
```
- Excluir uma branch
```bash
git branch -d <nome-da-branch>
```
- Upar a branch local para um servidor remoto
```bash
git push -u <local-remoto> <nome-da-branch>
```
- Trocar de Branch
```bash
git checkout <nome-da-branch>
```


5. Commit de alterações
```bash
git commit -m "mensagem do commit"
```
6. Empurrar alterações para o servidor
```bash
git push origin <nome-da-branch>
```
- Para Branch recém criadas

```bash
git push --set-upstream <repositório-remoto> <nome-da-branch>
```
7. Obter alterações do servidor

```bash
git pull <repositório-remoto>
```
8. Voltar para um commit anterior
- Utilize um comando para ver o seu histórico de commits
```bash
git log -- oneline
```
- Então utilize o git revert
```bash
git revert hash
```

9. Merge de 2 Branch
- Digamos que eu quero fazer Merge das Branch Felipe e main
1. Vou para a branch main
```bash
git checkout main
```
2. Atualizo a Branch main
```bash
git fetch
```
3. Rodo o comando de merge
```bash
git merge <nome-da-branch-com-o-recurso>
```
## Ordem da utilização

- Para upar as modificações locais
```bash
git status
git add <nome-do-arquivo-modificado> ou git add . //adiciona todos os arquivos
git commit -m 'Meu primeiro commit'
git push
```
- Para atualizar o repositório local com as novas informações do servidor
```bash
git status //não devem existir modificações que precisem de git add
git pull
```

## Fonte
https://www.freecodecamp.org/portuguese/news/10-comandos-do-git-que-todo-desenvolvedor-deveria-conhecer/

## Extra
https://www.freecodecamp.org/portuguese/news/ficha-informativa-do-git-50-comandos-do-git-que-voce-deveria-conhecer/
