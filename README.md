# BlockChainBlackProject

Этот проект предоставляет клиент для взаимодействия с блокчейнами, такими как Ethereum, Polygon, Binance Smart Chain (BSC), NEAR, Avalanche и Solana. Он включает функции для работы с смарт-контрактами, такие как получение баланса, отправка транзакций, подписка на события и взаимодействие с несколькими контрактами.

![BlockChainBlackProject](https://img.freepik.com/premium-vector/blockchain-line-icon-logo-concept-dark-background_516670-196.jpg)

## Функционал

### Основные возможности:

- **Получение баланса**: Приложение позволяет получить баланс Ethereum-адреса из блокчейн-сети.
- **Отправка транзакций**: Отправка транзакций для изменения данных в смарт-контрактах (например, инкрементирование значения).
- **Подписка на события**: Подписка на события смарт-контрактов с отображением в реальном времени.
- **Работа с несколькими блокчейнами**: Поддержка различных блокчейн-сетей, таких как Ethereum, Polygon, Binance Smart Chain (BSC), NEAR, Avalanche, Solana.
- **Работа с несколькими контрактами**: Получение данных из нескольких контрактов параллельно.

### Новые функции:

- **Переключение блокчейнов**: В проект добавлена возможность переключения между различными блокчейн-сетями через интерфейс.
- **Интерактивное меню**: Пользователь может выбрать необходимые операции (получение баланса, отправка транзакций, подписка на события и т.д.) через консоль.
- **Система уведомлений**: Базовая система уведомлений для отображения успешных транзакций и важной информации в процессе работы.
- **Поддержка нескольких контрактов**: Приложение теперь позволяет работать с несколькими смарт-контрактами одновременно, параллельно получая и обрабатывая данные.
- **Валидация данных**: Приложение включает механизмы для валидации входных данных (адресов и приватных ключей) перед выполнением операций на блокчейне, что повышает безопасность работы.
- **Логирование и обработка ошибок**: В проекте предусмотрено логирование ошибок и успешных операций, а также грамотная обработка исключений для предотвращения сбоев приложения.

## Структура проекта

- **BlockchainClient**: Основная структура для взаимодействия с блокчейном. Содержит методы для получения данных с контрактов и отправки транзакций.
- **BlockchainType**: Перечисление для работы с различными блокчейн-сетями (Ethereum, Polygon, BSC, NEAR, Avalanche, Solana).
- **ContractFactory**: Структура для создания контрактов и работы с ними.

## Установка и настройка

1. **Клонируйте репозиторий:**
   ```bash
   git clone https://github.com/alexmorettihhhh/blockchain_event_project.git
   cd blockchain_event_project


1.**Установите зависимости для Rust:**
```bash
cargo build
```

Настройте переменные окружения для приватных ключей и других конфигурационных данных: ``` " export PRIVATE_KEY="your_private_key" " ```


**Получение баланса**
```
Выберите операцию:
1. Получить баланс
2. Отправить транзакцию
3. Подписаться на события
4. Переключить блокчейн
5. Работать с несколькими контрактами
6. Выход
1
Введите адрес кошелька:
0xYourAddress
Баланс: 1000000000000000000
```
**Пример 2: Отправка транзакции**
```
Выберите операцию:
1. Получить баланс
2. Отправить транзакцию
3. Подписаться на события
4. Переключить блокчейн
5. Работать с несколькими контрактами
6. Выход
2
Введите приватный ключ:
0xYourPrivateKey
[ALERT] Транзакция успешна, хэш: 0xTransactionHash
```
**Пример 3: Подписка на события**
```
Выберите операцию:
1. Получить баланс
2. Отправить транзакцию
3. Подписаться на события
4. Переключить блокчейн
5. Работать с несколькими контрактами
6. Выход
3
Получено событие: CounterIncremented с новым значением: 5
```
**Пример 4: Переключение блокчейна**

```
Выберите операцию:
1. Получить баланс
2. Отправить транзакцию
3. Подписаться на события
4. Переключить блокчейн
5. Работать с несколькими контрактами
6. Выход
4
Выберите блокчейн (Ethereum, Polygon, BSC, Solana):
Polygon
Переключение блокчейна на Polygon
```
**Пример 5: Работа с несколькими контрактами**
```
Выберите операцию:
1. Получить баланс
2. Отправить транзакцию
3. Подписаться на события
4. Переключить блокчейн
5. Работать с несколькими контрактами
6. Выход
5
Введите адреса контрактов через запятую (например, 0xAddress1,0xAddress2):
0xAddress1,0xAddress2
Data from contract: 10
Data from contract: 20

```

# Что нового в версии 1.3.0
## Добавлено:
- Поддержка мультичейн-операций (Ethereum, Polygon, BSC, Solana).
- Новые методы API: get_blockchain_info(), list_contracts().
- Cистема валидации адресов и приватных ключей.
- Уведомления о статусе транзакций.
## Изменено:
- Обновлены зависимости ethers-rs до v2.0.0.
- Улучшена обработка ошибок.
- Оптимизирована работа с асинхронными запросами.

## Исправлено:
- Исправлены ошибки компиляции.
- Исправлена работа с Solana RPC.
- Исправлена сериализация событий.

## Как внести вклад
- Форкните репозиторий.
- Создайте ветку для вашей функции (`git checkout -b feature/AmazingFeature`).
-  Зафиксируйте изменения (`git commit -m 'Add some AmazingFeature'`).
-  Запушьте ветку (`git push origin feature/AmazingFeature`).
- Откройте Pull Request.






