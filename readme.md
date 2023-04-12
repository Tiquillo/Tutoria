## Diagrama de clases

```mermaid
classDiagram

    iPhone13 <|-- Celular
    Pantalla *-- Celular
    Camara <.. Celular
    Persona -- Celular

    class Persona {
        +string nombre
        +dateFormat nacimiento
        +Edad()
        +Presentarse()
    }

    class Celular {
        +string imei
        +string procesador
        +Llamar()
        +EnviarMensaje()
    }

    class iPhone13 {
        +string MAC
        +Rastrear()
    }

    class Camara {
        +string MP
        +string marca
        +Capturar()
    }

    class Pantalla {
        +string resolucion
        +string marca
        +Mostrar()
    }
