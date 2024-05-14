# SGH
El objetivo es diseñar un diagrama de clases para un sistema de gestión de hospital que incorpore diversos elementos de la programación orientada a objetos, tales como asociaciones, herencias, realizaciones, agregaciones, composiciones, dependencias, clases abstractas, interfaces, enumeradores, atributos de solo lectura y atributos de clase.

Requisitos del Sistema:
1.	Personas:
o	Existen tres tipos de personas: Paciente, Doctor y Enfermero.
o	Todas las personas tienen atributos como nombre, identificación y dirección.
o	Los Pacientes pueden tener múltiples citas médicas.
o	Los Doctores pueden atender múltiples pacientes y tienen una especialidad.
o	Los Enfermeros asisten a los doctores y también pueden tener múltiples pacientes asignados.
2.	Citas Médicas:
o	Las citas médicas tienen atributos como fecha, hora, motivo de la cita y estado (programada, realizada, cancelada).
o	Cada cita médica está asociada a un Paciente y a un Doctor.
3.	Expedientes Médicos:
o	Los expedientes médicos contienen el historial médico del paciente, incluyendo diagnósticos, tratamientos y prescripciones.
o	Cada Paciente tiene un expediente médico.
4.	Especialidades Médicas:
o	Definir un enumerador para las especialidades médicas (ej. Cardiología, Dermatología, Pediatría).
5.	Relaciones:
o	Los Pacientes pueden tener múltiples citas médicas.
o	Los Doctores pueden atender múltiples pacientes y citas médicas.
o	Los Enfermeros pueden asistir a múltiples doctores y pacientes.
6.	Clases Abstractas e Interfaces:
o	Crear una clase abstracta Persona que será la superclase de Paciente, Doctor y Enfermero.
o	Definir una interfaz GestiónCitas con métodos para programar, cancelar y realizar citas médicas.
7.	Agregaciones y Composiciones:
o	Los Expedientes Médicos tienen una relación de composición con los Pacientes.
o	Las Citas Médicas tienen una relación de agregación con los Doctores y Pacientes.
8.	Dependencias:
o	La clase Doctor depende de la interfaz GestiónCitas para realizar sus funciones.
o	La clase Cita Médica depende de las clases Paciente y Doctor para gestionar las citas.
9.	Atributos de solo lectura y de clase:
o	Los atributos como el número de identificación y la especialidad de los doctores deben ser de solo lectura.
o	Los contadores de citas médicas pueden ser atributos de clase para llevar el registro a nivel del sistema.
<p><img src="https://raw.githubusercontent.com/Jxel117/SGH/main/imagen_2024-05-14_100918906.png"
