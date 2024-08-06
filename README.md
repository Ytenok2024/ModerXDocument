# Документация:
**Документация по языку программирования ModerX**

**Общие конструкции**

**Переменные**
**Создание переменной типа number**
number.new название-переменной значение
**Редактирование переменной**
number.edit.название-переменной = значение

// Операторы: - уменьшает, + прибавляет, / делит, * умножает
**Создание переменной типа string**

string.new название-строки "текст-строки"


**Списки**

**Создание списка**

List.new название-листа = тип-листа [количество-элементов]

**Редактирование элемента списка**

List.edit.название-листа[номер-элемента] = значение

**Присвоение индексов элементам списка**

List.edit.название-листа[#all] = #index


**Строковые функции**

**Возврат строк**

return(строки-через-запятую ; сколько-раз)

**Вывод текста в консоль**

print("текст")

**Вывод текста на экран игрока**

printscreen("текст")


**Генерация случайных чисел**

**Генерация случайного числа**

random(значение1, значение2 ; название-переменной)


**Задержка**

**Создание задержки**

delay in временной_тип(значение)

// Временные типы: sec(секунда), min(минута)


**Условные конструкции**

**Условные операторы**

if название_переменной == значение {

  // код
  
} else if название_переменной == значение {

  // код
  
} else {

  // код
  
}

**Циклы**

**Цикл for**

for (number.new переменная значение ; переменная < значение ; команда на увеличение) {

  // код
  
}

**Цикл while**

while (переменная < значение) {

  // код
  
}

**Функции и кнопки**

**Создание функции**

from [название] {команды-через-точку-с-запятой}

**Вызов функции**

usefrom [название]

**Создание кнопки**

create.new Button название-кнопки {функция кнопки}

**Создание текста (можно использовать только переменные)**

create.new Text название-текста


**Импорт плагинов**

**Импорт плагина**

import plugin название-плагина


**Команды для плагинов**

**Обозначение плагина**

#plugin

**Создание команды**

addnewcommand (комманда) {

  // функция
  
}
**Использование текста в команде**

<текст>


**Пример плагина**

_Код плагина test_

#plugin


addnewcommand (test <test>) {

  print(<test>)
  
}
**Пример использования**
import plugin test
test "текст"
