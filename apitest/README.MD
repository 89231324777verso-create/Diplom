# API Autotest

Тест проверяет сценарий:

1. Создание заказа (POST /api/v1/orders)
2. Получение заказа по треку (GET /api/v1/orders/track)
3. Проверка, что код ответа = 200

## Запуск

```bash
pip install pytest requests pytest
### запуск теста

```bash
pytest create_order_test.py