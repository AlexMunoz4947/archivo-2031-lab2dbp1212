| Hallazgo | Dónde estaba | Técnica de Git | Comando exacto | Referencia |
|---|---|---|---|---|
| FRAG-01 | Historial de la rama principal de la cinta | Inspección de commit | `git show 086ff0f:bitacora/frag-01.txt` | `086ff0f` |
| FRAG-02 | Tag anotado de respaldo previo al incidente | Inspección de objeto Git | `git cat-file -p respaldo/pre-incidente` | `respaldo/pre-incidente` |
| Glifo | Árbol asociado al respaldo previo al incidente | Restauración desde referencia | `git restore --source=respaldo/pre-incidente -- assets/sello.svg` | `respaldo/pre-incidente` |