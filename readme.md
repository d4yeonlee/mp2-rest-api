
# MP2 Data Processing REST API

This project is a REST API built with FastAPI that allows users to upload, retrieve, validate, and process CSV datasets. It integrates reusable data processing modules from MP1 to handle missing values, remove duplicate rows, and optionally detect outliers. The API uses Pydantic models for request validation, in-memory storage for datasets, and middleware for logging requests and tracking response times.

## API Endpoints

- GET /health - Check the API status.
- POST /upload - Upload a CSV dataset.
- GET /datasets/{dataset_id} - Retrieve a stored dataset.
- POST /datasets/{dataset_id}/process - Validate and clean a dataset.

## Testing

Run the required tests using:

```bash
python -m pytest tests -v
```

All three required API tests passed.
