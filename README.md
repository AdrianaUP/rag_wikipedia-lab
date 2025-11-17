## rag_wikipedia-lab
"# RAG Wikipedia Lab

Este repositorio contiene la implementación de un pipeline de Retrieval-Augmented Generation (RAG) usando Wikipedia como fuente de conocimiento. Es parte de la entrega de Task 2 del laboratorio de agentes multiagente.

---

## 📁 Estructura del proyecto

\`\`\`
rag_wikipedia-lab/
├── notebooks/
│   └── rag_wikipedia.ipynb         # Notebook principal con el flujo completo
├── data/
│   └── wiki_corpus.csv             # Corpus chunked extraído de Wikipedia
├── outputs/
│   ├── retrieval_examples.json     # Ejemplos de recuperación con ChromaDB
│   └── rag_summary.md              # Resumen generado en formato Markdown
├── requirements.txt                # Dependencias del proyecto
└── README.md                       # Este archivo
\`\`\`

---

## ⚙️ Descripción del flujo

El notebook realiza los siguientes pasos:

1. Extracción de texto desde una página de Wikipedia (\`Federated_learning\`).
2. Segmentación del texto en chunks utilizando \`RecursiveCharacterTextSplitter\`.
3. Generación de embeddings con el modelo \`all-MiniLM-L6-v2\` de \`sentence-transformers\`.
4. Almacenamiento en ChromaDB para recuperación semántica.
5. Recuperación de documentos relevantes usando LangChain.
6. Generación de resumen en Markdown usando \`google/flan-t5-base\`.

---

## 🚀 Cómo ejecutar (si el entorno lo permite)

1. Crear entorno virtual:
   \`\`\`
   python -m venv .venv
   .venv\Scripts\activate
   \`\`\`

2. Instalar dependencias:
   \`\`\`
   pip install -r requirements.txt
   \`\`\`

3. Ejecutar el notebook:
   \`\`\`
   jupyter notebook notebooks/rag_wikipedia.ipynb
   \`\`\`

---

## 📝 Notas

- Debido a problemas técnicos en el entorno local, los archivos generados fueron creados manualmente para completar la entrega.
- El código está completo y estructurado para reproducibilidad, aunque no se pudo ejecutar en esta máquina.

