# MedHelp Architecture

## High-Level Flow

```text
User
  │
  ▼
Flask Web Interface
  │
  ▼
Application / Query Processing
  │
  ▼
LangChain Retrieval Workflow
  │
  ▼
Pinecone Vector Database
  │
  ▼
Relevant Context
  │
  ▼
Llama 2
  │
  ▼
Generated Response
  │
  ▼
User
```

## Main Components

### `app.py`
Application entry point for the Flask web application.

### `store_index.py`
Responsible for the vector-index preparation workflow.

### `helper.py`
Contains supporting project utilities.

### `prompt.py`
Contains prompt-related configuration.

### `template.py`
Contains application/template configuration.

### `data/`
Stores the knowledge/data resources required by the project.

### `model/`
Stores the local model resources required to run the application.

### `chat.html` and `style.css`
Provide the browser-based chat interface.

> Keep this architecture document synchronized with the implementation whenever the system changes.
