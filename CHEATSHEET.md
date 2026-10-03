# ⚡ Git Cheatsheet — Comandos Salvavidas

## Estado

```bash
git status
git branch --show-current
git log --oneline --graph --decorate -10
```

## Cambios

```bash
git diff
git diff --staged
git restore archivo
git restore --staged archivo
```

## Commits

```bash
git add .
git commit -m "mensaje"
git commit --amend
git revert <hash>
```

## Ramas

```bash
git branch
git switch main
git switch -c nueva-rama
git branch -d rama
```

## Stash

```bash
git stash push -u -m "temporal"
git stash list
git stash pop
```

## Remotos

```bash
git remote -v
git fetch origin
git pull --rebase
git push
git push -u origin rama
```

## Emergencia

```bash
git reflog
git show <hash>
git switch -c rescate <hash>
```

## Muy destructivos

```bash
git reset --hard
git clean -fd
git push --force
```

Antes de usarlos, revisa dos veces qué información vas a perder.
