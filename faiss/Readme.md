# Create Docker

From folder `faiss/` run:
```bash
docker build . -t faiss
docker run -v $(pwd):/home/jovyan/src/ -p 8888:8888 faiss
```

# Content:
- Как для одного вектора найти его ближайшего соседа в "базе данных" (индексе)?
- Как для нескольких векторов найти их ближайший соседей в "базе данных" (индексе)?
- Как построить индекс если вектора не помещаются в память?