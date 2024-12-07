# Entrega final IIC3633 - Sistemas Recomendadores

# Contenido del repositorio :rocket:

El repositorio cotiene tres carpetas principales 
1. **Generar embeddings**
2. **Embeddings**
3. **Métricas**

Es importante ejecutar los archivos en el **orden correspondiente** para el correcto funcionamiento.

## Contenido por carpeta :hammer:

### Generar embeddings :envelope:
En esta carpeta se encuentran los archivos .ipynb correspondientes para generar los embeddings de **texto**, **imagen** y **multimodal** de Siglip, Clip y Blip:

1. Siglip.ipynb
2. Clip.ipynb
3. Blip.ipynb
   
El output de cada archivo serán tres archivos conteniendo el embedding respectivo. El nombre con el cual se guarda es suficientemente descriptivo para saber cuál es el embedding y a qué modelo pertenece:

1. NombreModelo_text_embeddings.pt
2. NombreModelo_image_embeddings.pt
3. NombreModelo_multimodal_embeddings.pt

#### Ejecución :warning:
Estos archivos se deben importar a una sesión en google collab y ejecutar todas las celdas para obtener los archivos de embeddings como output. 

### Embeddings :floppy_disk:

En esta carpeta se encuentran tres carpetas:
1. Siglip
2. Clip
3. Blip
   
Cada carpeta contiene los tres archivos de embeddings que generamos al hacer el proyecto. 

### Métricas :bar_chart:

En esta carpeta se encuentran cuatro archivos:
1. Métricas_Siglip_LightFM.ipynb
2. Métricas_Clip_LightFM.ipynb
3. Métricas_Blip_LightFM.ipynb
4. Referencia GPT para consultas.pdf

Los primeros tres archivos se encargan de calcular las métricas por cada modelo y para cada archivo de embedding. El cuarto, contiene la conversación usada para apoyar la construcción de métricas.

#### Ejecución :warning:

Los archivos de **métricas** deben importarse a una sesión de google collab, y en el entorno se deben cargar los archivos de embeddings para el modelo correspondiente. Es decir, si estamos trabajando con Métricas_Siglip_LightFM.ipynb, se deben cargar los archivos:
1. SIGLIP_text_embeddings.pt
2. SIGLIP_image_embeddings.pt
3. SIGLIP_multimodal_embeddings.pt

Luego, ejecutar todas las celdas, y se obtendrán las métricas por cada archivo de embedding.


