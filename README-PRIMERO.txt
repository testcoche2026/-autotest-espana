AUTOTEST ESPAÑA — PROYECTO ANDROID

Este paquete es el proyecto fuente Android; no es todavía un archivo .AAB firmado.
En este entorno no están instalados el Android SDK y las herramientas de compilación/firma necesarias para producir un AAB verificable. Puedes generarlo con Android Studio siguiendo estos pasos.

REQUISITOS
- Ordenador Windows, macOS o Linux.
- Android Studio reciente.
- Cuenta de Google Play Console para publicar (la cuenta de desarrollador de Google Play normalmente requiere una cuota única de registro; por eso no se puede garantizar una publicación completamente gratuita).

GENERAR EL AAB
1. Descomprime AutoTestEspaniaAndroid.zip.
2. Abre Android Studio.
3. Selecciona Open y elige la carpeta AutoTestEspaniaAndroid (la que contiene settings.gradle).
4. Acepta la sincronización de Gradle e instala el Android SDK 36 si Android Studio lo solicita.
5. En el menú, selecciona Build > Generate Signed Bundle / APK.
6. Selecciona Android App Bundle y pulsa Next.
7. Crea un nuevo keystore (guárdalo con cuidado; no lo pierdas y no lo compartas). Rellena los campos solicitados y pulsa Next.
8. Selecciona la variante release y pulsa Create/Finish.
9. Android Studio generará el archivo .aab dentro de app/release/ o la ruta que indique al terminar.
10. Sube ese .aab a una versión de prueba interna en Google Play Console y completa los formularios de la ficha, privacidad y clasificación de contenido.

IMPORTANTE
- applicationId: es.autotest.espana. Debe ser único para tu app. Si ya lo usa otra app tuya, cámbialo antes de publicar.
- No cambies el applicationId después de publicar la primera versión.
- Las preguntas son ejemplos originales de práctica y las señales usan emojis ilustrativos. No son material oficial de la DGT.
- Antes de publicar, revisa las políticas actuales de Google Play, el requisito vigente de API objetivo y los requisitos de privacidad. Esta plantilla no recopila datos ni crea cuentas.
- La publicación en Google Play no es necesariamente gratuita: Google Play Console suele cobrar una tarifa de registro de desarrollador.
