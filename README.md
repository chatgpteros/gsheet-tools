Descripción general
Este repositorio contiene un script de Google Sheets en JavaScript que permite interactuar con los modelos de lenguaje OpenAI GPT, incluidos ChatGPT (GPT-3.5-turbo) y GPT-4. Este script permite enviar consultas a los modelos y recibir respuestas, proporcionando una integración fácil y rápida con Google Sheets.

Cómo usar
Crea una nueva hoja de cálculo de Google Sheets.
Ve a Herramientas > Editor de secuencias de comandos para abrir el editor de secuencias de comandos de Google.
Copia y pega el contenido del archivo JS proporcionado en el editor de secuencias de comandos.
Reemplaza TUAPI en la línea const apiKey = "TUAPI" con tu clave de API de OpenAI.
Guarda el script y cierra el editor de secuencias de comandos.
Vuelve a tu hoja de cálculo de Google Sheets y escribe una función en una celda, por ejemplo, =CHATGPT("Hola, ¿cómo estás?", "¿Cuál es tu nombre?"). La función enviará una consulta al modelo ChatGPT y mostrará la respuesta en la celda.
Funciones disponibles
CHATGPT(text, prompt, systemPrompt='', maxTokens=200, temperature=0.0, model='gpt-3.5-turbo'): Envía una consulta a ChatGPT y devuelve la respuesta.
GPT4(text, prompt, systemPrompt='', maxTokens=200, temperature=0.0, model='gpt-4'): Envía una consulta a GPT-4 y devuelve la respuesta.
OpenAIGPT(text, prompt, systemPrompt='', maxTokens=200, temperature=0.0, model='gpt-3.5-turbo'): Función base para enviar consultas a los modelos de lenguaje GPT de OpenAI.
GPTCOST(model='', maxOutputTokens=100, text='', prompt='', systemPrompt=''): Estima el costo en USD de una solicitud basándose en la cantidad de tokens de entrada y salida.
Advertencia
El uso de la API de OpenAI y los modelos de lenguaje GPT puede generar costos. Consulta la página de precios de OpenAI para obtener más información sobre los costos asociados. Utiliza este script bajo tu propia responsabilidad y ten en cuenta los costos y límites de API asociados con tu cuenta de OpenAI.
