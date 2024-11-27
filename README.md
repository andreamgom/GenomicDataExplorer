# Análisis de Secuencias Genómicas y Proteicas

## 📖 Introducción
Este proyecto tiene como objetivo procesar y analizar secuencias biológicas almacenadas en archivos FASTA, con un enfoque en:
- Conteo y visualización de bases nucleotídicas en ADN.
- Análisis de residuos de aminoácidos en proteínas.
- Descarga de secuencias desde la API de NCBI en formatos **FASTA** y **GenBank**.

---

## 🔍 Descarga de Secuencias mediante la API de NCBI

Se pueden obtener secuencias desde NCBI utilizando la URL: https://eutils.ncbi.nlm.nih.gov/entrez/eutils/efetch.fcgi?db={db}&id={sequence_id}&rettype={rettype}&retmode=text


**Parámetros**:
- `db`: Base de datos (`nucleotide` para ADN, `protein` para proteínas).
- `sequence_id`: Identificador único de la secuencia.
- `rettype`: Formato del archivo (`FASTA` o `GenBank`).

### Ejemplo:
Descargar la secuencia de un gen introduciendo el identificador, y guardar los archivos descargados en tu dispositivo. Primero en formato **FASTA** y luego en **GenBank**.

---

## 🧬 Caso 1: Análisis del Gen APP

### 1. ¿Qué tipo de información contienen los archivos?

#### Archivo FASTA
- Contiene una **secuencia de nucleótidos** (ARN mensajero del gen APP).
- El encabezado incluye el identificador `NM_000484.4` y una breve descripción del gen.
- La secuencia contiene nucleótidos (A, T, C, G).

#### Archivo GenBank
- Incluye información adicional:
  - **Identificador único**: NM_000484.4.
  - **Descripción**: mRNA del gen APP, variante de transcripción 1.
  - **Clasificación taxonómica**: *Homo sapiens*.
  - **Anotaciones funcionales**: Genes, exones, CDS, y regiones regulatorias.

### 2. ¿Son secuencias de genes específicos, genomas completos u otras entidades biológicas?
Corresponden a un **gen específico**. En este caso, el gen **APP** humano.

### 3. Proporción de nucleótidos:
La secuencia de 3,583 bp muestra un equilibrio entre bases nucleotídicas, con una ligera predominancia de A y G.

---

## 🧬 Caso 2: Análisis de la Green Fluorescent Protein (GFP)

### 1. ¿Qué tipo de información contienen los archivos?

#### Archivo FASTA
- Contiene la **secuencia de aminoácidos** de la proteína GFP.
- Encabezado: `>Chain A, GREEN FLUORESCENT PROTEIN`.
- Secuencia de 236 aminoácidos representada con letras estándar.

#### Archivo GenPept
- Contiene la misma secuencia, pero con anotaciones detalladas:
  - **Fuente biológica**: *Aequorea victoria*.
  - **Información estructural**: Hojas beta y residuos no estándar como MSE.
  - **Clasificación funcional**: Referencias a bases de datos como Pfam.

### 2. ¿Son secuencias de genes específicos, genomas completos u otras entidades biológicas?
Corresponden a una **proteína específica**, GFP, traducida de su gen original.

### 3. Proporción de aminoácidos:
La proteína tiene 236 aminoácidos. Cada uno está representado por su frecuencia relativa en la secuencia.

---

## 🌱 Reto: Fragmento del Cromosoma 4 de *Arabidopsis thaliana*

### 1. ¿Qué tipo de información contienen los archivos?

#### Archivo FASTA
- Contiene la secuencia de ADN del cromosoma 4, fragmento de contig Nº 17.
- Encabezado: `>AL161505.2 Arabidopsis thaliana DNA chromosome 4, contig fragment No. 17`.
- Secuencia en nucleótidos (A, T, G, C).

#### Vista gráfica
Proporciona un mapa estructural y funcional del fragmento:
- **Genes y exones**: Marcados en el eje genómico.
- **Regiones repetidas**: Elementos móviles y regulatorios.

### 2. Anotaciones funcionales:
- Genes como AT4g97320 y AT4g97410.
- Elementos regulatorios como promotores.




