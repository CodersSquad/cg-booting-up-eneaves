[![Review Assignment Due Date](https://classroom.github.com/assets/deadline-readme-button-22041afd0340ce965d47ae6ef1cefeee28c7c493a6346c4f15d667ab976d596c.svg)](https://classroom.github.com/a/swKMSSMl)
[![Open in Visual Studio Code](https://classroom.github.com/assets/open-in-vscode-2e0aaae1b6195c2367325f4f02e2d04e9abb55f0b24a779b69b11b9e10269abc.svg)](https://classroom.github.com/online_ide?assignment_repo_id=16850903&assignment_repo_type=AssignmentRepo)
# Computer Graphics Booting Up

## Let's start with ModernGL

This lab stands to prepare the moderngl development environment. Below the steps and requirements for initial coding tasks. Please make sure to edit the python provided files; for dependencies, you can add the files you need.

1. Install moderngl and its dependencies
2. Make sure that the following programs run
    - [`01_hello_world.py`](./01_hello_world.py)
    - [`06_multiple_objects.py`](./06_multiple_objects.py)
    - [`09_models_and_images.py`](./09_models_and_images.py)
        - _Modify this program to change the box's texture to a correctly aligned TEC logo_
3. Document how to execute the 3 programs in the section below.

* For documentation and missing dependencies, follow these links:
    - https://github.com/moderngl/moderngl
    - https://moderngl.readthedocs.io/

## How to run your program

```
Proyecto de Visualización 3D con moderngl, pygame y PyGLM
Este proyecto consta de tres programas de visualización en 3D utilizando moderngl, pygame, y PyGLM para gráficos en OpenGL. Estos programas muestran el uso de colores animados, geometrías simples (como triángulos) y modelos 3D más complejos con texturas.

Requisitos
Dependencias de Python
Instala las dependencias de Python con pip:

pip install moderngl pygame PyGLM numpy pillow
Nota: PyGLM se usa en lugar de glm, que puede tener problemas de compatibilidad. Si tenías glm instalado previamente, desinstálalo antes de instalar PyGLM:

pip uninstall glm
pip install PyGLM
Modelos 3D
Para el tercer programa, necesitas descargar dos archivos OBJ que representen los modelos 3D de una caja y un carro de juguete. Puedes utilizar los nombres de archivo crate.obj y lowpoly_toy_car.obj, y colocar estos archivos en el mismo directorio que el script de Python.

Configuración en macOS
Si estás en macOS, es posible que necesites ajustar algunos atributos de contexto de OpenGL en pygame para evitar problemas de compatibilidad. Agrega las siguientes líneas después de la inicialización de pygame:

pygame.display.gl_set_attribute(pygame.GL_CONTEXT_MAJOR_VERSION, 3)
pygame.display.gl_set_attribute(pygame.GL_CONTEXT_MINOR_VERSION, 3)
pygame.display.gl_set_attribute(pygame.GL_CONTEXT_PROFILE_MASK, pygame.GL_CONTEXT_PROFILE_CORE)
Esto configura la versión del contexto de OpenGL a 3.3 en pygame.

Ejecución de los Programas
Primer Programa: Muestra un cambio de color dinámico en el fondo de la pantalla.
Segundo Programa: Renderiza un triángulo con diferentes posiciones y colores.
Tercer Programa: Renderiza modelos 3D de un carro y una caja con texturas.
Para ejecutar cualquiera de los programas, simplemente ejecuta el script correspondiente con:

python nombre_del_script.py
Notas
Este proyecto requiere una tarjeta gráfica que soporte OpenGL 3.3 o superior.
Los archivos OBJ y las texturas deben estar en el mismo directorio que el script de Python.
En caso de problemas, verifica que tu entorno esté correctamente configurado para soportar gráficos en OpenGL con pygame y moderngl.
```

## Grading Policy

- 25% - `01_hello_world.py` is running with no errors
- 25% - `06_multiple_objects.py` is running with no errors
- 25% - `09_models_and_images.py` is running with the requested change (TEC logo texture)
- 25% - Documentation on how to run your programs