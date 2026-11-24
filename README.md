# 📊 API Metrics

API simples em **Flask** que expõe métricas gerais em JSON, pronta para deploy (Gunicorn + Procfile).

## 🚀 Rodando localmente

```bash
pip install -r requirements.txt
python metrics.py
```

A API sobe em `http://localhost:10000`.

## 🔌 Endpoints

| Rota | Descrição |
|:--|:--|
| `GET /` | Health check (`{"status": "ok"}`) |
| `GET /api/metrics` | Métricas gerais (empresas, clientes, serviços, usuários, agendamentos, comandas) |

`/api/metrics.php` também é aceito, para compatibilidade com front-ends antigos. CORS liberado.

## ☁️ Deploy

O `Procfile` usa Gunicorn — funciona direto em Render, Railway ou Heroku.
