Путешествия по России

Описание:
Одностраничный сайт с информацией об уголках нашей страны, с фотографиями, описанием и ссылками на источники. Благодаря пройденному курсу по адаптивности сайта под разные устройства, добились эффекта "резинового сайта". Теперь он одинаково хорошо открывается на экранах шириной от 320px и выше.

В процессе создания проекта были использованы разнообразные технологии:

1. Скачивание и установка определенных шрифтов
@font-face {
    font-family: 'Inter';
    src: url(../../russian-travel/Inter/Inter-Regular.woff2);
    font-weight: normal;
}

2. Медиазапросы
@media screen and (min-width: 1024px) and (max-width: 1279px) {
    .cover__title {
        max-width: 500px;
        white-space: normal;
    }
}

3. Работа с затеменением одного элемента
.cover__image {
    position: absolute;
    top: 0;
    left: 0;
    max-width: 100%;
    height: 100%;
    opacity: 0.5;
}

.cover__image:hover {
    opacity: 0.7;
}

4. Разкладка по правилам БЭМ

5. Grid
.place {
    display: grid;
    grid-template-columns: repeat(2, 1fr);
    grid-template-rows: repeat(1, 1fr)1, 2fr;
    column-gap: 40px;
    row-gap: 60px;
    color: #ffffff;
    margin: 0;
    margin-bottom: 72px;
}


Планы по доработке.
В скором времени планирую:
-заменить абсолютное позиционирование на наложение с помощью Grid;
-прописать кроссбраузность;
-Добавить карту России

Автор:
Артур Нуртдинов

Обратная связь:
nal.kzn@yandex.ru