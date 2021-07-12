# Create Docker

From folder `feature_extraction/` run:
```bash
docker build . -t feature_extraction
docker run -v $(pwd):/home/jovyan/src/ -p 8888:8888 feature_extraction
```


# Content
- `feature_extraction.ipynb`:  - Содержит примеры запуска моделей из [lightning-bolts](https://lightning-bolts.readthedocs.io/en/latest/):
- AE;
- VAE;
- SimCLR;
- SwAV.


