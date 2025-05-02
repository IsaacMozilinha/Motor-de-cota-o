# Motor-de-cota-o
Motor de cotação para testes antes de subir para o repositório da FECAP

**Para rodar:**

Baixe o PyCharm;

Abra o código no PyCharm;

Rode o comando no terminal:

```python
pip install -r requirements.txt
```

Após isso crie a pasta modelos dentro da pasta "app" e coloque os arquivos pkl nessa pasta

Para rodar a FastAPI rode no terminal:
```
uvicorn app.main:app --reload
```

E para acessar o Swagger cole no navegador:

http://127.0.0.1:8000/docs


Em POST passe o seguinte Payload:

````
{
  "lat_origem": -23.5505,
  "lng_origem": -46.6333,
  "lat_destino": -23.5568,
  "lng_destino": -46.6395,
  "ano": 2025,
  "mes": 4,
  "hora": 18,
  "tipo_dia": "dia_util",
  "trafego_estimado": "livre"
}
````
