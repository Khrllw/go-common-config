# Go_Common_config

Универсальный пакет конфигурации для Go-сервисов в едином формате.

## Что внутри

- загрузка конфигурации из переменных окружения (с поддержкой `.env` для локалки)
- нормализация значений
- fail-fast валидация
- генерация PostgreSQL DSN

## Подключение из другого сервиса

```bash
go get github.com/khrllw/Go_Common_config@latest
```

```go
import config "github.com/khrllw/Go_Common_config"

cfg, err := config.LoadConfig()
if err != nil {
    // обработка ошибки
}
```
