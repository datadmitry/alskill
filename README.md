# alskill

Навык Яндекс.Алисы ("Купи слона") на Flask.

## Деплой в Replit

1. На https://replit.com → **Create App** → **Import from GitHub** → вставить URL этого репозитория.
2. Replit подхватит `.replit` и `replit.nix` автоматически, зависимости поставятся из `requirements.txt`.
3. Нажать **Run** — сервер поднимется на `python main.py` (Flask dev server, порт 8080).
4. Для продакшена: вкладка **Deployments** → **Autoscale** → **Deploy**. Будет запущен gunicorn командой из секции `[deployment]` в `.replit`.
5. Endpoint навыка: `POST https://<your-repl>.replit.app/post`. Этот URL нужно прописать в настройках навыка в Яндекс.Диалогах.

## Локальный запуск

```bash
pip install -r requirements.txt
python main.py
```
