# Análisis de Secuencias Genómicas y Proteicas

## 📖 Introducción
El análisis de secuencias genómicas y proteicas es un componente esencial en la bioinformática. Permite comprender la composición, estructura y funcionalidad de genes y proteínas. Este proyecto tiene como objetivo principal procesar y analizar secuencias biológicas almacenadas en archivos FASTA, con un enfoque específico en el conteo y visualización de bases nucleotídicas y residuos de aminoácidos.

---

## 🔍 Descarga de Secuencias mediante la API de NCBI

Se pueden obtener secuencias de ADN y proteínas desde la base de datos de NCBI utilizando la URL:



### Parámetros:
- **`db`**: Base de datos a consultar (`nucleotide` para ADN, `protein` para proteínas).
- **`sequence_id`**: Identificador único de la secuencia.
- **`rettype`**: Formato del archivo (`FASTA` o `GenBank`).

Ejemplo: Descargar una secuencia específica y guardarla en ambos formatos (FASTA y GenBank) en tu dispositivo.

---

## 🖥️ Interfaz de Usuario

### Vista previa:
La interfaz permite buscar secuencias introduciendo el identificador y descargarlas directamente desde la API. A continuación, el archivo puede ser guardado con un nombre y ubicación personalizada.

---

## 🧬 Análisis del Gen APP

### Contexto:
La enfermedad de Alzheimer es una condición neurodegenerativa asociada con mutaciones en genes como **APP**, **PSEN1**, y **PSEN2**, que llevan a la acumulación tóxica de β-amiloide en el cerebro. 

El gen **APP** está localizado en el brazo largo del cromosoma 21 (21q21.3) y codifica la **proteína precursora de amiloide**. Mutaciones en este gen han sido asociadas con casos de Alzheimer de inicio precoz.

### Contenido de los Archivos:
#### **Formato FASTA**
- **Encabezado**: `>NM_000484.4 Homo sapiens APP variant 1`.
- **Secuencia**: Contiene nucleótidos (A, T, C, G).

#### **Formato GenBank**
Incluye información adicional como:
- **General Info**: Identificador, longitud, descripción, organismo, y taxonomía.
- **Gene Info**: Localización, nombre del gen y anotaciones.
- **Exons**: Rango de nucleótidos de cada exón.
- **CDS (Coding Sequences)**: Secuencia codificante para proteínas.
- **Péptidos señal y maduros**: Regiones funcionales derivadas.
- **Regulatory Features**: Promotores, potenciadores y otros elementos regulatorios.

### Proporción Nucleotídica:
La secuencia tiene una longitud de **3,583 bp**, con una distribución equilibrada de bases, predominando A y G.

---

## 🌟 Análisis de Green Fluorescent Protein (GFP)

### Contenido de los Archivos:
#### **Formato FASTA**
- Secuencia de 236 aminoácidos.
- Encabezado: `>Chain A, GREEN FLUORESCENT PROTEIN`.

#### **Formato GenPept**
- Anotaciones detalladas como:
  - Fuente biológica: *Aequorea victoria*.
  - Estructura y funcionalidad.
  - Clasificación en bases de datos como Pfam.

---

## 🧩 Ejemplo: Fragmento de Cromosoma en Arabidopsis thaliana

### Archivo FASTA:
- **Encabezado**: `>AL161505.2 Arabidopsis thaliana DNA chromosome 4, contig fragment No. 17`.
- **Secuencia**: Representación de nucleótidos.

### Representación Gráfica:
- **Genes y exones**: Anotados en el eje genómico.
- **Regiones repetidas**: Visualización de elementos móviles o regulatorios.

---

## 📊 Conclusión

Este proyecto ofrece una herramienta integral para el análisis de secuencias genómicas y proteicas, combinando acceso directo a bases de datos (NCBI), procesamiento de secuencias en diversos formatos y análisis estructural. Es aplicable en investigaciones sobre enfermedades genéticas y estudios funcionales de proteínas.

