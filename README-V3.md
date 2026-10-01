# Inventario Almacén v3 — compilación automática

Esta versión está preparada para compilar el APK automáticamente en GitHub Actions, sin instalar Android Studio en el teléfono.

## Qué incluye
- Productos y códigos de barras.
- Entradas y salidas con actualización de stock.
- Historial de movimientos.
- Escáner real mediante cámara + CameraX + ML Kit.
- Exportación de inventario e historial a CSV compatible con Excel.
- Base de datos local Room.
- APK Debug generado automáticamente por GitHub Actions.

## Cómo obtener el APK desde un teléfono
1. Crea una cuenta gratuita en GitHub.
2. Crea un repositorio nuevo, por ejemplo `inventario-almacen`.
3. Sube **todo el contenido de esta carpeta** al repositorio (incluido `.github`).
4. Abre la pestaña **Actions**.
5. Entra en **Compilar APK Inventario Almacen**.
6. Pulsa **Run workflow**.
7. Espera a que termine el proceso.
8. En la ejecución terminada, baja hasta **Artifacts**.
9. Descarga `InventarioAlmacen-debug-apk` y extrae `app-debug.apk`.
10. Instala el APK en tu Xiaomi.

## Requisitos del proyecto
- Android Gradle Plugin 8.7.3
- Kotlin 2.0.21
- Gradle 8.9
- Java 17
- Android compileSdk 35
- minSdk 26

## Nota
No se incluye `gradle-wrapper.jar` porque este paquete está diseñado para que GitHub Actions configure Gradle automáticamente. No necesitas Android Studio para la compilación mediante Actions.
