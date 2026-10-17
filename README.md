# Timer Flotante
Cronómetro pequeño, siempre visible, para medir cuánto tiempo llevas en espera durante una llamada. Al silenciar el micrófono, la ventana se pone roja y el cronómetro arranca; al activarlo, vuelve a negro y se pausa.

## Controles

| Acción | Qué hace |
|---|---|
| Clic izquierdo | Iniciar / pausar el cronómetro |
| Clic derecho | Reiniciar a cero |
| Barra espaciadora | Silenciar / activar el micrófono de Windows y cambiar el color de la ventana (la ventana debe estar enfocada) |
| Arrastrar el interior | Mover la ventana |
| Arrastrar los bordes | Cambiar el tamaño de la ventana |
| Ctrl + rueda del ratón | Cambiar el tamaño del texto |
| Esc | Cerrar |

La posición, el tamaño y el tamaño del texto se guardan en `timer_config.json`, junto al script.

## Requisitos

- Windows y Python 3. Tkinter ya viene incluido.
- [pycaw](https://pypi.org/project/pycaw/), para controlar el micrófono. Instálalo con:

```powershell
winget install --exact --id Python.Python.3.12
```

```powershell
pip install pycaw
```

Si pycaw no está instalado, el timer funciona igual (cronómetro y cambio de color), pero no silencia el micrófono real.

## Uso

Haz doble clic en `timer_flotante.pyw`, o ejecútalo sin consola con:

```powershell
pythonw timer_flotante.pyw
```

Solo se permite una ventana a la vez.
