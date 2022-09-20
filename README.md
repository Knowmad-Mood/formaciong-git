# Formaciong Git

Repositorio para formación a cerca de git y github actions

## Buenas prácticas

A continuación tenemos algunas buenas prácticas a tener en cuenta para llevar un flujo de trabajo limpio y adecuado.

### Squash

A la hora de realizar un merge, siembre es conveniente dejar bien limpio y claro el historial de commit. Para ello, podemos agregar el parámetro o flag --squash en nuestro merge

TODO: Definir los pasos para realizar squash cuando mergeamos.

#### Trick

```bash
git config --global alias.squash-all '!f(){ git reset $(git commit-tree HEAD^{tree} -m "${1:-A new start}");};f'
```
