# API usage

GET `/health`, GET `/resources`, and GET/POST `/api/RESOURCE`. PUT `/api/RESOURCE/ID` requires `{ "record": {...}, "version": 1 }`. Unknown resources return 404 and invalid records return 400. Only local synthetic-data usage is supported.
