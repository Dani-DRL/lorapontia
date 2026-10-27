# Finetuning de Stable Diffusion con LoRA (ilustraciones de libros antiguos)

Entrega final del módulo de Modelos de Generación de Imagen.

- Modelo base: `CompVis/stable-diffusion-v1-4`
- Dataset: `gigant/oldbookillustrations` (columnas `1600px` e `info_alt`)
- Modelo finetuneado: https://huggingface.co/DaniDRL/lorapontia

## Contenido

- `finetuning_lora_oldbookillustrations.ipynb`: notebook con el finetuning, la subida a Hugging Face y la carga del modelo desde el Hub.
- `imagenes/`: comparación antes/después con el mismo prompt y semilla (`comparacion_antes_despues.png`) y curva de loss.
- `lora_weights/`: pesos de la LoRA.
- `enlace_modelo_hf.txt`: enlace al modelo en Hugging Face.
- `requirements.txt`: versiones de las librerías usadas.

## Configuración

Entrenado en un MacBook (M2 Pro, 16 GB) en unos 10 minutos: 200 imágenes, 2 épocas, resolución 512 (resize + center crop), LoRA con rango 16 y learning rate 2e-4.
