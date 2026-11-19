# Instrucciones para agentes — ASSIO-ESA

Se aplica a todo el repositorio. Codex debe leer este archivo; con Claude u otra herramienta, incluirlo explícitamente si no lo carga automáticamente.

## Antes de cambiar archivos

Lee `README.md` y la memoria antes de describir objetivos o resultados. `main` contiene entregables; el README enlaza otras ramas, incluido el TXT manual de comandos de P2. Verifica la rama antes de asumir qué material está disponible. No es una aplicación ni infraestructura automatizada.

Comprueba `git status --short` y la rama. Conserva cambios ajenos y lee las instrucciones de cualquier subdirectorio afectado. Contrasta los documentos con el código: un plan o resultado antiguo no demuestra una función actual. Limita cada cambio al encargo recibido.

## Reglas del proyecto

- Conserva PDF/PPTX originales; no los regeneres o sobrescribas durante una tarea documental.
- No inventes código, dependencias, VM, servicios o comandos de prueba ausentes. El TXT de P2 tiene encabezados y sesiones interactivas: no lo pases entero a Bash ni lo presentes como script idempotente. Las capturas son evidencia histórica del laboratorio, no del sistema actual.
- No ejecutes `sudo`, cambios de propietarios, usuarios, grupos o ACL de la memoria en el host. Cualquier reproducción debe tener una VM de laboratorio explícita y alcance definido.
- No copies datos personales o credenciales desde capturas a la documentación nueva.

## Validación y entrega

Para documentos comprueba inventario, enlaces y coherencia con los entregables. Si se solicita editar un PDF o PPTX, conserva una copia y verifica su renderizado. No hay CI ni tests que lanzar. Si se desarrolla automatización futura, registra SO, precondiciones y comprobaciones por rol sin presentar la extracción de texto como ejecución del laboratorio.

En cambios solo de documentación, comprueba rutas, enlaces relativos y comandos contra los archivos reales; no hace falta repetir toda la suite si no cambia el comportamiento. No inventes pruebas ausentes ni marques como aprobado un comando que no ejecutaste. Informa comando, resultado y alcance pendiente.

Revisa el diff antes de hacer commit. No incluyas dependencias instaladas, archivos generados, datos personales, credenciales, cookies, tokens ni archivos de entorno privados. Mantén los documentos útiles existentes y actualiza el estado si cambia una decisión o una limitación. Los commits deben explicar el resultado y su validación; separa documentación y cambios funcionales.
