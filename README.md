# Туториал по Нетлифай ЦМС

### Инструкции:
- [как сделать сайт на Джекиле и разместить его на Netlify CDN](site-setup.md)
- [и как добавить к нему админку Netlify CMS](cms-setup.md)

### Результат:
[netlify-primer.netlify.com](https://netlify-primer.netlify.com/)

Можно зарегистрироваться и что-нибудь написать в блог :)

### [Netlify CMS](https://www.netlifycms.org) - это:
- CMS для статических сайтов
- опенсорсный проект
- в лучших традициях JAM-стека
- одностраничное приложение на Реакте
- симпатичный интерфейс
- гибкое взаимодействие с контентом

Обязательное условие: сайт должен быть размещен на гитхабе

### Зачем?
Когда хотим статический сайт, и с админкой будет удобнее:
- цмс для лендинга
- редактирование документации, размещенной на Гитхаб Пейджес
- админка для личного сайта/блога, когда неохота возиться с Вордпрессом
- etc.

### Альтернативы:
Более комплексные сервисы:
- [Forestry](https://forestry.io)
- [CloudCannon](https://forestry.io)

[И много, много еще](https://headlesscms.org)


### Доступ к админке:
- по инвайтам или свободный
- даже для тех, у кого нет гитхаб-аккаунта (т.е. доступа на пуш в репозиторий)


### Установка:
1. Добавляем разметку и стили приложения-админки:
    - используем cdn
    - или устанавливаем npm-пакетом
2. Настраиваем аутентификацию
3. Настраиваем коллекции

### Схема работы:
1. Пользователь заходит в админку и редактирует контент
2. Контент размещается в структурированных файлах
    - форматы: маркдаун, TOML, YAML, JSON
    - структура задается настройкой коллекции
3. Цмс создает в репозитории временную ветку и открывает пул-реквест с новым файлом
4. Цмс мержит реквест в ветку мастер (или другую, по настройкам)
5. Сайт пересобирается, изменения опубликованы.


