FROM lukasblecher/pix2tex:api

WORKDIR /backend
ADD backend/* /backend/
RUN pip install -e latexorc

ENTRYPOINT ["uvicorn", "latexorc.app:app", "--host", "0.0.0.0", "--port", "7860"]
