Los errores que hemos encontrado en el backend son:

- El archivo MetricResponseDTO.java estaba duplicado en la carpeta repository.
- En los endpoints de metrics/ se devolvía valores aunque el valor dado al endpoint no esté enlistado en el código, mostrando una mala validación de entrada.
- En SecurityConfig acepta todas las peticiones que recibe sin restricción, sirviendo más de adorno que como real seguridad.
- En DeveloperMetricRepository.java se encuentran los datos que deberían estar ocultos y guardados en una base de datos.
- MetricResquestDTO.java tiene un seteo muy pobre, hacen falta getters, setters, etc.
