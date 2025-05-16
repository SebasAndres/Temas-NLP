# Tareas y herramientas de NLP

## Etapas de un proyecto NLP
1. Task formulation
2. Data collection
3. Data processing 
4. Model Training
5. Model Evaluation
6. Deployment

## Arquitectura básica en sistemas de NLP

### Morfologia
Tokenizar: Dado un texto segmentarlo en unidades mas pequeñas.

PoS Tagging: Asignar una etiqueta de clase de palabra para cada palabra de un texto.

Token   | Lema    | POS TAG
atendio | atender | VIMS2312

Lema: Entrada en el diccionario asociada a la raiz.

Los POS TAGGER se pueden armar con:
|-> Reglas lingüísticas
|-> Aprendizaje Automático:SVM, HMM (Modelos Ocultos de Markov), RN profundas

### Análisis de sintaxis

Gramáticas / Árboles de derivación
Es muy costoso armarlo, hay alternativas menos costosas llamadas Shallow Parsing y Chunking

### Análisis semántico
Lexico, Proposicional

El gato: entidad -> ser vivo -> animal -> felino domestico determinado

### Reconocimiento de entidades nombradas (NER)
Identificar instancias de una clase de informacion específica.
Métodos.
-> Reglas
-> Aprendizaje automático

## Preprocesamiento
- Tokenizacion
- Stemming/Lematizers: Reducir las formas inflectivas.
    Sea hace Stemming (obtener la raíz) o lematizacion (obtencion de la forma básica o entrada de diccionario de la palabra). Una o la otra (es mas facil hacer stemmers que lemmatizers).
- Nornalizacion: Transformar el texto para que el procesamiento sea mas sencillo (sacar tildes, expandir acronimos, sacar stop words, convertir numeros a palabras, etc) 

Corpus (~Dataset): conjunto de datos recopilados aveces anotados-etiquetados y/o preprocesados.
La etiquetacion es una tarea no trivial.