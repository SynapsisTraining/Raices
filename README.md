# Raíces

Aplicación Streamlit para explorar posibles creencias y patrones aprendidos en cinco
ámbitos: amor y relaciones, dinero, salud, deporte y trabajo.

## Qué hace

El usuario introduce una frase, pensamiento o situación. La aplicación distingue entre:

- lo que aparece explícitamente en sus palabras;
- las posibles creencias y patrones;
- el posible aprendizaje familiar;
- la influencia cultural o colectiva;
- otras explicaciones que deben considerarse;
- preguntas para comprobar o descartar la hipótesis;
- una alternativa más flexible y una pequeña acción observable.

La herramienta es educativa y exploratoria. No realiza diagnósticos psicológicos o
médicos ni atribuye enfermedades o problemas a conflictos emocionales.

## Ejecutar en local

1. Instala las dependencias:

   ```bash
   pip install -r requirements.txt
   ```

2. Copia `.streamlit/secrets.toml.example` como `.streamlit/secrets.toml` y añade tu
   clave de Gemini.

3. Ejecuta:

   ```bash
   streamlit run app.py
   ```

## Publicar en Streamlit Community Cloud

1. Crea un repositorio de GitHub y sube estos archivos conservando sus carpetas.
2. En Streamlit Community Cloud, crea una aplicación indicando `app.py` como archivo
   principal.
3. En **App settings > Secrets**, configura:

   ```toml
   GEMINI_API_KEY = "tu_clave"
   GEMINI_MODEL = "gemini-2.5-flash"
   ```

No subas nunca el archivo real `secrets.toml` al repositorio.

