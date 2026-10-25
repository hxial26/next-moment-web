# NextMoment · prototipo interactivo

Prototipo mobile-first de la propuesta NextMoment para el reto de Imaxel en TecnoChallenge. Conserva la interfaz trabajada anteriormente, el logo y el wordmark originales y la paleta del proyecto.

## Ejecutar

Abre `app/index.html` o inicia Live Server desde la carpeta del proyecto. No requiere dependencias ni compilación. La portada principal incluye un acceso directo a esta demo.

## Recorrido

- Bienvenida y acceso de demostración.
- Revisión de fotografías de muestra con X para marcar y ✓ para conservar, gestos laterales, animación y estado guardado en `localStorage`.
- Álbumes con filtros, búsqueda, creación de colecciones y un álbum colaborativo de ejemplo.
- Invitaciones de álbum y referidos simulados. Copiar o enviar un enlace no suma puntos; un registro simulado añade los 50 puntos propuestos. Los 250 puntos por primera compra para cada persona se describen, pero no se simulan. Los estados e historial quedan en `localStorage`.
- Catálogo conceptual con álbum, idea NFC, copias instantáneas, calendarios, pósteres, lienzos y regalos. La selección de productos es una demo sin precios ni pagos.
- Perfil de demostración con favoritos, métricas de sesión, ajustes y reinicio de datos.
- Resumen de una sesión de revisión.

Las ilustraciones de muestra y los productos se sirven desde `app/assets/images`, sin servicios externos. El análisis por IA, la limpieza, la integración NFC, los puntos, los referidos, el acceso y las compras son simulaciones: no se borran las fotos originales ni se procesan pagos. El sistema de referidos no funciona entre dispositivos; requeriría backend y autenticación. Los precios están por definir y el prototipo no lee etiquetas NFC. Las fotos añadidas desde el equipo se usan localmente durante la sesión.
