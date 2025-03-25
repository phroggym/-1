# Устройство детектирования
## Индивидуальное задание 1
### Краткое описание назначения и применения продукта

Продукт - устройство детектирования УД) обрабатывает входящие сигналы от датчиков, в случае превышения порога срабатывания принимает решение о выдаче команды в систему управления защиты (СУЗ) реактора (автоматическое срабатывание). 
УД передаёт обработанные данные в автоматизированную систему управления технологическим процессом (АСУ ТП) АЭС для дальнейшей обработки, на основе этих данных оператор АСУ ТП может принять решение о выдаче команды в СУЗ (административное срабатывание)

| Ценности продукта и негативные события в их отношении |
| --- | --- | --- | --- |
| Ценность | Негативное событие | Величина ущерба | Комментарий |
| `данные, которые получает, хранит и передает УД` | List all *new or modified* files | Высокий | Возможно причинение вреда здоровью клиентов |
| `git diff` | Show file differences that **haven't been** staged |
