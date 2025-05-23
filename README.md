# Устройство детектирования
## Индивидуальное задание 1
### **Краткое описание назначения и применения продукта**

Продукт - устройство детектирования УД) обрабатывает входящие сигналы от датчиков, в случае превышения порога срабатывания принимает решение о выдаче команды в систему управления защиты (СУЗ) реактора (автоматическое срабатывание). <br>
УД передаёт обработанные данные в автоматизированную систему управления технологическим процессом (АСУ ТП) АЭС для дальнейшей обработки, на основе этих данных оператор АСУ ТП может принять решение о выдаче команды в СУЗ (административное срабатывание)

#### Ценности продукта и негативные события в их отношении
| Ценность | Негативное событие | Величина ущерба | Комментарий |
| --- | --- | --- | --- |
| `данные, которые получает, хранит и передает УД` | Нарушение целостности (сигнал изменен), потеряна аутентичность, сигнал не обработан (пришел и пропал) | Высокий | Возможно причинение вреда здоровью клиентов |
| `Команда в СУЗ` | Команды нет, когда нужно; команда есть, когда не нужно | Высокий | Ложное срабатывание защиты реактора, чрезвычайная ситуация |
| `События в журнале` | Событие не зарегистрировано в т.ч. событие из журнала пропало; событие зарегистрировано с искажением; зарегистрировано событие, которого не было | Средний | Сложности при расследовании инцидентов |
| `Обновление` | Применена неатентичная прошивка <br> Аутентичная прошивка привела к любому из: <br> - Устройство превратилось в необновляемый кирпич <br> - Устройство стало допускать любую прошивку <br> - Устройство перестало проходить общесистемные (внешние) положительные тесты. <br> - Устройство перестало реагировать на внешние общесистемные (внешние) негативные тесты | Средний | Может потребоваться внеплановая дорогостоящая замена оборудования |

### **Роли пользователей**

Оператор-фармацевт - вводит задание на производство и получает лекарство для передачи клиенту <br>
Пациент - получает рецепт от врача в клинике и по этому рецепту получает лекарство в аптеке
