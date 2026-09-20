# Автотесты API сервиса «Яндекс Самокат»

Автоматизированные тесты API для сервиса аренды самокатов: проверка эндпоинтов, статус-кодов и структуры ответов.

## Технологии
- Python 3.10+
- Pytest 8.4.1
- requests 2.32.4
- Allure (allure-pytest 2.15.0) — отчётность

## Структура проекта
```
Sprint_7/
├── data/        — тестовые данные
├── helpers/     — генераторы тестовых данных
├── methods/     — методы работы с API (обёртки над запросами requests)
├── tests/       — тест-кейсы
└── requirements.txt
```

## Как запустить
```bash
git clone https://github.com/Ximikkirito/Sprint_7.git
cd Sprint_7
python -m venv venv && source venv/bin/activate   # Windows: venv\Scripts\activate
pip install -r requirements.txt
pytest -v
```

Генерация отчёта:
```bash
pytest --alluredir=allure-results
allure serve allure-results
```

## Автор
Игорь Федотов — [ссылка на резюме/GitHub-профиль]