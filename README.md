# Привет!
Добро пожаловать на страницу описания библиотеки Флореста. Оригинал находиться [тут](https://pypi.org/project/florestdevinstruments/)
----------
# Что я такое?
Я - библиотека Флореста, написанная на Python и имеющая обширный функционал, который с каждым днем только увеличивается.
У меня есть 4 модуля: `florest_utilits`, `working_document`, `ready_games` и `working_api`.
У каждого из данных модулей есть свое предназначение.
Установить модуль можно используя `pip install florestdevinstruments`. Качайте самую последнюю версию!
----------
# Примеры использования
```python
from florestdevinstruments.florest_utilits import ai_image # импорт функции "ai_image" из модуля florest_utilits.
with open('image.png', 'wb') as file: # создаем и открываем файл формата .png
    file.write(ai_image('Draw an old car.')) # записываем в наш файл в изображение
    file.close() # сохраняем изображение.
```

```python
from florestdevinstruments.ready_games import russian_rullet # импортируем русскую рулетку
answear = int(input(f'Введите свое число от 1 до 3:'))
if russian_rullet(answear): # при правильном ответе вернет True
    print(f'Поздравляю!')
else:
    print(f'Ты проиграл!')
```

```python
from florestdevinstruments.working_api import VK # импортируем модуль "VK"
vk = VK('токен приложения сообщества', int('ID сообщества')) # инициализация класса
print(f'Сейчас подписано: {str(vk.get_subs())}) на сообщество.') # выводим количество подписчиков на экран.
```
----------
# Автор
Подписывайтесь на мои ресурсы. [Тык](https://telegra.ph/Socseti-Floresta-06-28)