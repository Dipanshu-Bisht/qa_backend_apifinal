# QA Backend API

## Setup

```bash
pip install -r requirements.txt
uvicorn app.main:app --reload
```

## Endpoints

### 1. Upload a Document

**POST** `/upload`  
**Form field:** `file` (upload `.pdf`, `.txt`, or `.docx`)

### 2. Ask a Question

**POST** `/question`  
**Body (JSON):**
```json
{
  "question": "What is the document about?"
}
```

## Notes

- Ensure the document is uploaded first.
- You can use Postman to test both endpoints.