# Primeros pasos

- entremos a tmux usando el comando `tmux` en nuestra terminal
- con tmux puedes crear sesiones, que basicamente son tus ventanas de trabajo para tu terminal.
- el comando anterior automaticamente creara una sesion nueva con un panel de terminal.
- estas sesiones no se pierden si no las eliminas, lo que es una ventaja si tienes algun problema o se cierra tu terminal por error.
- para crear una sesion, tienes el comando `tmux new`
- a una sesion le puedes definir un nombre completando el comando asi: `tmux new -s <NOMBRE>`
- puedes crear tantas sesiones como quieras, ocupan muy poca memoria
- Para interactuar con tmux dentro de una sesion, podemos hacerlo via comandos.
- estos comandos seran ejecutados siempre y cuando los invoques despues de presionar el "prefijo".
- por defecto el prefijo de tmux es `crtl + b`. Yo he cambiado la tecla `Mayus` de mi mac a que sea `ctrl` y he cambiado mi prefijo a `ctrl + a`, asi es mucho mas facil presionar ambas teclas.
- en los atajos siguientes me referiré a `ctrl + (a|b)` como `PREFIX`.

## Paneles

- en una sesion de tmux puedes "dividir" la pantalla en varias terminales, a cada division le llama "panel".
- para crear un panel, el comando depende de donde lo quieras crear:

  ```bash
  `PREFIX %`      # Dividir panel horizontalmente
  `PREFIX \"`     # Dividir panel verticalmente
  ```

- Para moverte entre los paneles (cambiar el foco), lo puedes hacer con `PREFIX + FLECHA` y te moveras al panel que esté en la dirección de la flecha.

- Para cambiar el tamaño de un panel:

  ```bash
  `PREFIX Ctrl + FLECHA`      # Cambias el tamaño en la direccion de la flecha
  ```

- Si mantienes presionado `Ctrl` y la flecha, el panel se ira moviendo hasta que tu sueltes las teclas.
