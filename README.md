# Домашнее задание по теме "Доработка бота"
____
## Цель: 
подготовить Telegram-бота для взаимодействия с базой данных.
## Задача "Витамины для всех!":
**Подготовка:**

Подготовьте Telegram-бота из последнего домашнего задания 13 модуля сохранив код с ним в файл ***module_14_3.py***.

*Если вы не решали новые задания из предыдущего модуля рекомендуется выполнить их.*

**Дополните ранее написанный код для Telegram-бота:**

**Создайте и дополните клавиатуры:**
>1. В главную (обычную) клавиатуру меню добавьте кнопку **`"Купить"`**.
> 
>2. Создайте ***Inline*** меню из 4 кнопок с надписями **`Product1`**, **`Product2`**, **`Product3`**, **`Product4`**.
У всех кнопок назначьте ***`callback_data="product_buying"`***

**Создайте хэндлеры и функции к ним:**
>1. Message хэндлер, который реагирует на текст ***`Купить`*** и оборачивает функцию **`get_buying_list(message)`**.
>   
>3. Функция **`get_buying_list`** должна выводить надписи
>
>**`Название: Product<number> `**| **`Описание: описание <number>`** |**` Цена: <number * 100>`**
>
>**4 раза**.
> После каждой надписи выводите картинки к продуктам.
>В конце выведите ранее созданное **Inline** меню с надписью **`Выберите продукт для покупки:`**.
>4. **Callback** хэндлер, который реагирует на текст ***`product_buying`*** и оборачивает функцию **`send_confirm_message(call)`**.
>
>5. Функция **`send_confirm_message`** присылает сообщение ***`Вы успешно приобрели продукт!`***

## Пример результата выполнения программы:

**Обновлённое главное меню:**

![image](https://github.com/user-attachments/assets/f41dc58d-6163-43ab-837e-4b91d8651e31)

**Список товаров и меню покупки:**

![image](https://github.com/user-attachments/assets/9ff3106e-27a7-4d76-bebc-e92811a7bafb)



**Примечания:**
>1. Название продуктов и картинок к ним можете выбрать самостоятельно. (Минимум 4)
**Файл module_14_3.py с кодом загрузите на ваш GitHub репозиторий. В решении пришлите ссылку на него.**
