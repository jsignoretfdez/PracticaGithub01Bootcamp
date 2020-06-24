# Preguntas Ejercicio 1 Bootcamp Full Stack Web Git & Github

#### - ¿Qué comando utilizaste en el paso 11? ¿Por qué?

**<span style = "color: #910e04; font-size:14px">git reset --hard HEAD~1</span>** en este caso utilizamos el modificador **--hard** ya que se nos pide que debemos realizarlo perdiendo los cambios del Working Copy.

#### - ¿Qué comando o comandos utilizaste en el paso 12? ¿Por qué?

Primero vamos a realizar un **<span style = "color: #910e04; font-size:14px">git reflog</span>**. Esto nos va a permitir ver hacia que id debemos ir para llegar hasta el commit que debemos rehacer de nuevo.

**<span style = "color: #910e04; font-size:14px">git reset --hard 06f9835 </span>**. Debemos realizarlo con **--hard** ya que tenemos que modificar el working copy para que estén los cambios que habiamos realizado en el archivo *git-nuestro.md*

#### - El merge del paso 13, ¿Causó algún conflicto? ¿Por qué?

No, al realizar el merge con el comando **<span style = "color: #910e04; font-size:14px">git merge master </span>**, me salta el siguiente mensaje **Already up-to-date**. Según he leido esto pasa debido a que por decirlo de alguna manera la rama que estamos intentando fusionar, es una matriz de la rama actual por lo que el contenido ya esta fusionado. Por eso nos salta el mensaje de ya actualizado. Además con esto lo que pasa es que estamos intenando mover el puntero styled a master cuando en el grafo master es el padre de styled y a nivel de grafo sería desplazar hacia abajo el puntero styled.  

#### - El merge del paso 19, ¿Causó algún conflicto? ¿Por qué?

Si, en esta ocasión al realizar el merge con el comando **<span style = "color: #910e04; font-size:14px">git merge htmlify </span>**, nos sale el mensaje como que tenemos un conflicto. Esto pasa porque en el archivo hemos modificado la misma línea en htmlify que teniamos en el archivo de la rama styled. Por lo que vamos a proceder a modificar el archivo para quedarnos con la parte de styled tal como nos dice el punto 20. Una vez modificado y guardado vamos a comitearlo para que se queden correctamente realizado el merge.

#### - El merge del paso 21, ¿Causó algún conflicto? ¿Por qué?

No, esta vez se ha realizado el merge correctamente con el comando **<span style = "color: #910e04; font-size:14px">git merge styled </span>**. Esto se debe a que se ha realizado un merge fast forward tal como nos indica el mensaje en la consola de comandos y lo que hacemos a nivel de grafo es pasar el puntero master al commit de la rama styled.

#### - ¿Qué comando o comandos utilizaste en el paso 25?

Primeramente me he creado un alias para futuros usos y no tener que poner todo el rato el comando ya que he metido varios modificadores para mejorar la forma de mostrar el grafico de los logs. El alias que configure es el siguiente **<span style = "color: #910e04; font-size:14px">git config --global alias.lg "log --graph --date-order --date=short \
--pretty=format:'%C(auto)%h%d %C(reset)%s %C(bold blue)%ce %C(reset)%C(green)%cr (%cd)'"</span>**. El comando lo saque de una web donde ponian ejemplos de como se ve una grafo con ciertos modificadores, seguiré investigando para ver cual se puede gustarme más para futuras consultas del grafo. El comando para que nos muestre el grafo que he utilizado es **<span style = "color: #910e04; font-size:14px"> git lg </span>**

#### - El merge del paso 26, ¿Podría ser fast forward? ¿Por qué?

Si, podría ser fast forward porque el padre de title es master.

#### - ¿Qué comando o comandos utilizaste en el paso 27?

En este caso he utilizado el comando **<span style = "color: #910e04; font-size:14px">git reset HEAD~1 </span>** ya que nos indican que no debemos perder los cambios del working copy.

#### - ¿Qué comando o comandos utilizaste en el paso 28?

Utilizo el comando **<span style = "color: #910e04; font-size:14px">git restore git-nuestro.md </span>**. También podríamos haber utilizado el comando **git checkout git-nuestro.md** ya que esta es la forma antigua en la que se hacía.

#### - ¿Qué comando o comandos utilizaste en el paso 29?

He tenido que utilizar **<span style = "color: #910e04; font-size:14px">git branch -D title </span>**, ya que al intentar hacerlo con -d git nos manda un mensaje donde nos indica que la rama title no esta mergeada y que si estamos seguros debemos utilizar el modificador -D.

#### - ¿Qué comando o comandos utilizaste en el paso 30?

Primero utilice el comando **git reflog** para saber el id del commit al que debia ir y a continuación.

Utilice el comando **<span style = "color: #910e04; font-size:14px">git reset --hard 5e36990</span>**

#### - ¿Qué comando o comandos usaste en el paso 32?

Primero utilice el comando **git reflog** para saber el id del commit al que debia ir y a continuación.

Utilice el comando **<span style = "color: #910e04; font-size:14px">git checkout 4e5a828</span>**


#### - ¿Qué comando o comandos usaste en el punto 33?

Primero utilice el comando **git reflog** para saber el id del commit al que debia ir y a continuación.

Utilice el comando **<span style = "color: #910e04; font-size:14px">git checkout 14f586c</span>**
