# Генератор списков доп. полей

**Документация**: [На сайте автора](https://devcraft.club/articles/xf-list-generator.14/)

**Пользовательское соглашение**: [На сайте автора](https://devcraft.club/pages/licence-agreement/)

**Автор**: Maxim Harder

**Версия**: 1.1.0

Модуль подключается в любом шаблоне при помощи инклуда:
```
{include file="engine/modules/xf_list_gen.php?xffield=X&template=X&&limit=X&skip=X&sort=X&cat=X&news_id=X"}
```


Обязательные теги:
- **xffield** - Название доп. поля
- **template** - Название шаблона с окончанием


Дополнительные теги:
- **limit** - Ограничивает вывод записей в списке, принимает только числа. По умолчанию: пусто
- **skip** - Пропускает заданное число записей, принимает только числа. По умолчанию: пусто
- **sort** - Сортировка списка, по умолчанию или по убыванию. Принимает только ASC и DESC. По умолчанию: ASC
- **cat** - Перечень категорий через запятую (,) из которых должны формироваться списки **# начиная с версии 1.1.0**
- **news_id** - Перечень новостей через запятую (,) из которых должны формироваться списки **# начиная с версии 1.1.0**


Возможные теги в вашем шаблоне:
- **{link}** - Выводит ссылку на доп. поле, если имеется (хотя да...)
- **{name}** - Название доп. поля
- **{value}** - Значение доп. поля
- **{max_value}** - Максимально возможное значение, сделано для вывода чисел
- **{min_value}** - Минимально возможное значение, сделано для вывода чисел
- **{count}** - Выводит общее количество использования доп. поля **# начиная с версии 1.1.0**


# Установка

Либо закинуть файл **xf_list_gen.php** в папку **engine/modules**, либо установить **плагин через менеджер плагинов**