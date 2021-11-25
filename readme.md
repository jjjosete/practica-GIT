1. -git reset --hard HEAD~1

Porque la otra opción de deshacer un commit, es decir, simplemente <git reset HEAD~1>
mantiene intacto nuestra working copy.

2. -git reset --hard <sha1 del commit anterior>

Con el comando y el código del commit que quería recuperar podía volver a ese punto sin 
tener que repetir lo hecho anteriormente.

3. - No hubo ningún conflicto porque la línea style sólo contiene el archivo git-nuestro.md actualizado. 
Si antes del merge hubiéramos modificado el archivo en la rama master sí que habría ocurrido un conflicto.

4.Sí, hubo conflicto porque los archivos git-nuestro.md habían sido modificados de maneras distintas y desde 
distintas ramas, es decir, las modificaciones del archivo no habían sufrido una progresión lineal, sino que
las modificaciones habían ido por caminos distintos. Por eso al intentar mergearlos hubo conflicto.

5. No hubo ningún conflicto, porque ya habían mergeado antes.

6.git log --graph --decorate --pretty=oneline

7. sí, porque el archivo de git-nuestro.md de title era el de master modificado. Si antes de mergear title y
 master hubiéramos modificado el archivo de master sólo podría haber sido  no fast forward.

8.  git reset HEAD~1

9. git restore git-nuestro.md

10.  git branch -D title

11. git branch title 
    git checkout master
    git merge title

12. git checkout c424c13

13. git checkout 2ac3ae4
