# CREACIÓN DE UMBRALES ESTADÍSTICOS DE LA PRODUCCIÓN

# **Predicción de Producción Agrícola y Pecuaria a Nivel de Cuenca**

## **Descripción del Proyecto**
Este proyecto tiene como objetivo la estimación y predicción de la producción agrícola y pecuaria en distintas cuencas hidrográficas utilizando modelos de regresión lineal. Se emplean datos históricos municipales para calcular la distribución espacial a nivel de cuenca, generar modelos de regresión para cada tipo de producción y proyectar los valores hasta el año 2040.

## **Estructura del Código**
El código está organizado en las siguientes secciones:

1. **Importación de Librerías**: Se importan las librerías necesarias para la manipulación de datos, visualización y modelado estadístico.
2. **Carga de Datos**: Se leen los archivos Excel que contienen datos históricos de producción agrícola y pecuaria, así como las proporciones de distribución por cuenca.
3. **Procesamiento de Datos**:
   - Transformación de datos municipales a nivel de cuenca mediante proporciones asignadas.
   - Agregación y almacenamiento de datos procesados.
4. **Modelado de Regresión Lineal**:
   - Creación de modelos de regresión lineal simple para cada cultivo o tipo de producción en cada cuenca.
   - Cálculo de coeficientes de regresión y coeficiente de determinación (R²).
5. **Predicción hasta 2040**:
   - Estimación de valores futuros basados en modelos de regresión lineal.
   - Generación de intervalos de confianza y predicción.
6. **Visualización**:
   - Gráficos de tendencias y predicciones para producción agrícola y pecuaria.
   - Comparación de valores observados y proyectados.
7. **Población**:
   - Incorporación de datos de proyección de población urbana y rural basada en información del DANE.
   - Estimaciones de población a nivel de cuenca mediante regresión lineal para el período 2023-2040.

## **Requisitos**
Para ejecutar este proyecto se necesita:
- Python 3.7+
- Librerías:
  - `pandas`
  - `numpy`
  - `matplotlib`
  - `statsmodels`
  - `sklearn`
- Google Colab (opcional, si se usa almacenamiento en Google Drive)

## **Ejecución del Proyecto**
1. Montar Google Drive si se ejecuta en Google Colab.
2. Asegurarse de que los archivos de entrada están correctamente almacenados en las rutas especificadas.
3. Ejecutar las celdas en orden para procesar los datos, entrenar modelos y generar predicciones.
4. Analizar los resultados generados en los archivos de salida y gráficos.

## **Archivos de Entrada**
- `historico-palma.xlsx`
- `historico-arroz.xlsx`
- `historico-cacao.xlsx`
- `historico-porcino.xlsx`
- `historico-ave.xlsx`
- `proporcion.xlsx`
- `historico-bovino-animal.xlsx`
- `proporcion-urbano.xlsx`
- `proporcion-rural.xlsx`
- `proyeccion-dane-urbano.xlsx`
- `proyeccion-dane-rural.xlsx`

## **Archivos de Salida**
- `historico-cuenca.xlsx` → Datos históricos transformados a nivel de cuenca.
- `modelos-regresion-cultivo.xlsx` → Resultados de regresión lineal.
- `prediccion-2007-2040.xlsx` → Predicción completa hasta 2040.
- `prediccion-2023-2040-agricola.xlsx` → Predicción para producción agrícola.
- `prediccion-2023-2040-pecuario.xlsx` → Predicción para producción pecuaria.
- `prediccion-2023-2040-poblacion.xlsx` → Proyección poblacional a nivel de cuenca.

## **Contacto**
Para cualquier consulta o colaboración, por favor contacta a través de este repositorio o a [oscarvargas@trabajocientif.com].

