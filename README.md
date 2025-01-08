# CHRONOLOG 
### [Versión actual: 0.1.0](#versiones)

> ### Visite [chronolog](https://tutosrivegamerlq.github.io/chronolog/) para más documentación

"**Chronolog**" es un módulo diseñado para facilitar la creación de registros (_logs_) en aplicaciones desarrolladas con **Python**. Proporciona una manera sencilla y estructurada de documentar eventos, errores y actividades en los programas, mejorando la capacidad de monitoreo y depuración del código.

> Ejemplo de registro: En una línea
```md
>  
2025-01-06 19:52:08.636560 - Exception - FileNotFoundError - File - c:\Users\srm\Desktop\msqlite\msqlite\__logger.py - ErrorLine: 35 - Messsage: [Errno 2] - No such file or directory: './data/log'
```

Para empezar a usar, iniciaría con una instancia de la _clase_ **Logger**, la cual toma como argumentos el siguiente parámetro:

- `name:str`: Nombre del archivo en el cual se guardarán los registros (Ej: `'log.log'`).
> NOTA: Es necesario que el directorio donde se guardará el archivo esté creado, ÚNICAMENTE el **directorio**, el archivo se creará dentro de automáticamente...

## Métodos públicos disponibles:

- **log**: Permite guardar mensajes **generales** en el registro, es decir, **NO ERRORES**, mensajes de información _ordinaria_ (general).
- **log_e**: Permite registrar errores, es un registro más específico.

### Métodos privados 🔏

- **__write**: Escribe los mensages en el archivo cargado
- **__date**: Obtiene la fecha actual
- **__log**: Toma registro de errores internos, guarda los registros en el archivo "./log.log" (En el directorio raíz del módulo)

## Versiones:
 - v0.1.0: Inicial

Si desea conocer más acerca de, visite:
- [Web de soporte](https://tutosrivegamerlq.github.io/chronolog/)
- [Web pypi.org](https://pypi.org/project/chronolog/)
- [Github project](https://github.com/tutosrivegamerLQ/chronolog/)