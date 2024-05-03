## Efficient Document Retrival using Ollama and PrivateGPT

This project aims to enhance document search and retrieval processes, ensuring privacy and accuracy in data handling.

### Getting Started

##### Step 1: Setup a Virtual Env

##### Step 2: Install Dependencies using Pip

```bash
pip install -r requirements.txt
```

##### Step 3: Ensure Ollama and Mistral is installed

```bash
ollama pull mistral
```

##### Step 4: Create `source_documents` Folder and Add your Documents

```bash
mkdir source_documents
```

Supported file types:

- `.csv`: CSV,
- `.docx`: Word Document,
- `.doc`: Word Document,
- `.enex`: EverNote,
- `.eml`: Email,
- `.epub`: EPub,
- `.html`: HTML File,
- `.md`: Markdown,
- `.msg`: Outlook Message,
- `.odt`: Open Document Text,
- `.pdf`: Portable Document Format (PDF),
- `.pptx` : PowerPoint Document,
- `.ppt` : PowerPoint Document,
- `.txt`: Text file (UTF-8),

##### Step 5: Ingest Documents to Store in Vector Database for Query

```bash
python ingest.py
```

##### Step 6: Chat using PrivateGPT

```bash
python privateGPT.py
```

To use a different model try


```bash
ollama pull llama2:13b
MODEL=llama2:13b python privateGPT.py
```
