# Programación Orientada a Objetos (POOB)

Repositorio general del curso Programación Orientada a Objetos (ISIS POOB-201), que agrupa —mediante submódulos de git— los laboratorios individuales del curso y los proyectos desarrollados en equipo.

Cada submódulo es un repositorio independiente con su propio historial de commits y README. Para clonar este repositorio junto con todo su contenido, ver [Cómo clonar](#cómo-clonar).

## Estructura del proyecto

```
Programacion-Orientada-a-Objetos/
├── Laboratorios/
│   ├── Formas-Geometricas-y-Torre-de-Hanoi-POOB/
│   ├── Calculadora-Relacional-Diseno-y-Pruebas-POOB/
│   ├── Automata-Celular-Herencia-e-Interfaces-POOB/
│   ├── Excepciones-Tienda-de-Disfraces-POOB/
│   ├── Interfaz-Grafica-Clustering-POOB/
│   └── Persistencia-Replicate-POOB/
└── Proyectos/
    ├── TILTING-TILES-POOB/
    └── POOBvsZOMBIES-POOB/
```

## Temas del curso

El curso recorre el ciclo completo de diseño y construcción de software orientado a objetos, desde los fundamentos hasta la construcción de aplicaciones completas con interfaz gráfica y persistencia:

- **Fundamentos**: metodologías ágiles (Manifiesto Ágil, XP), principios SOLID, y los conceptos base de clases y objetos en Java (tipos primitivos, modificadores de acceso, `==` vs. `equals`).
- **Encapsulamiento, ocultación de información y sobrecarga**: los tres pilares iniciales del diseño orientado a objetos.
- **Relaciones entre objetos**: asociación, enlaces, multiplicidad, agregación y composición.
- **Herencia y polimorfismo**: sobreescritura de métodos, uso de `super`, jerarquías de clases y clases abstractas.
- **Interfaces**: contratos de comportamiento y su diferencia con las clases abstractas.
- **Excepciones**: jerarquía `Throwable`/`Error`/`Exception`, excepciones chequeadas vs. no chequeadas, `try`/`catch`/`finally`, propagación y excepciones personalizadas.
- **Interfaces gráficas**: componentes AWT/Swing, patrón Modelo-Vista-Controlador (MVC), contenedores, layouts y manejo de eventos.
- **Colecciones**: listas, mapas, conjuntos y genéricos, con su rol de encapsulamiento y delegación.
- **Persistencia**: serialización de objetos y entrada/salida a archivos de texto plano.
- **De diseño a código**: cómo traducir un plano de objetos (diagrama de clases) a una implementación completa en Java, incluyendo pruebas de aceptación.

## Cosas a tener en cuenta

- Los laboratorios se desarrollan sobre proyectos BlueJ, con arquitectura por capas (`domain`/`presentation`) y pruebas unitarias en JUnit.
- Cada laboratorio retoma y extiende el proyecto del laboratorio anterior del mismo tercio (por ejemplo, `Automata-Celular-Herencia-e-Interfaces-POOB` y `Persistencia-Replicate-POOB` parten ambos del proyecto `replicate`).
- `Calculadora-Relacional-Diseno-y-Pruebas-POOB` (laboratorio 2, primer tercio) documenta el enunciado real del laboratorio, pero el código nunca llegó a subirse a GitHub en su momento — el repositorio conserva ese estado real en vez de fabricar una implementación.
- `TILTING-TILES-POOB` y `POOBvsZOMBIES-POOB` son proyectos desarrollados en equipo (2-3 integrantes) como entregas finales del curso.

## Herramientas

- Java (BlueJ, compilación/documentación/pruebas también desde consola: javac, javadoc, jar)
- JUnit
- Swing / AWT

## Cómo clonar

```bash
git clone --recurse-submodules https://github.com/JuanGuayazanC/Programacion-Orientada-a-Objetos.git
```

Si ya clonaste el repositorio sin submódulos:

```bash
git submodule update --init --recursive
```
