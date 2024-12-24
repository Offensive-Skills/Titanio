### **Básico/Miscelánea/tmux.md**

# tmux

## Descripción

`tmux` es un multiplexor de terminal similar a `screen`, con características avanzadas.

## Uso

tmux [comando]

### Comandos comunes

- `new -s nombre`: Crea una nueva sesión con nombre.
- `attach -t nombre`: Adjunta a una sesión existente.
- `ls`: Lista sesiones activas.
- `kill-session -t nombre`: Termina una sesión.

## Ejemplos

- Iniciar una nueva sesión:

  tmux new -s mi_sesion

- Adjuntar a una sesión existente:

  tmux attach -t mi_sesion

- Listar sesiones:

  tmux ls
