**Задача**

1 Создать класс Радио с полями переключение звука и громкость

2 Подключить плагин Surefire так, чтобы сборка падала в случае отсутсвия тестов

3 Подключить плагин JaCoCo в режиме генерации отчётов (обрушать сборку по покрытию не нужно)

4 Написать автотесты на методы, содержащие логику, добиться 100% покрытия по branch'ам

Требования к работе с радиостанциями:

* Номер текущей радиостанции изменяется в пределах от 0 до 9
* Если текущая радиостанция - 9 и клиент нажал на кнопку next (следующая) на пульте, то текущей должна стать 0-ая
* Если текущая радиостанция - 0 и клиент нажал на кнопку prev (предыдущая) на пульте, то текущей должна стать 9-ая
* Клиент должен иметь возможность выставлять номер радиостанции с цифрового пульта (вводя числа 0 - 9)

Требования к работе с уровнем громкости звука:

* Клиент должен иметь возможность увеличивать и уменьшать уровень громкости звука (в пределах от 0 до 10)*
* Если уровень громкости звука достиг максимального значения, то дальнейшее нажатие на + не должно ни к чему приводить
* Если уровень громкости звука достиг минимального значения, то дальнейшее нажатие на - не должно ни к чему приводить

**Решение**

1 Написаны методы, в том числе с использованием Getters и Setters, а также c использованием подхода Early Exit.

2 Написаны автотесты, проверяющие возможность переключения звука и каналов, а также сохранение условий граничных значений или изменения этих значений на минимальное и максимальное.
