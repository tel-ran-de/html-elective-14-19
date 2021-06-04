# Шестой урок

## Повторение

```plaintext
*             {}  /* a=0 b=0 c=0 d=0 -> specificity = 0,0,0,0 */
li            {}  /* a=0 b=0 c=0 d=1 -> specificity = 0,0,0,1 */
li:first-line {}  /* a=0 b=0 c=0 d=2 -> specificity = 0,0,0,2 */
ul li         {}  /* a=0 b=0 c=0 d=2 -> specificity = 0,0,0,2 */
ul ol+li      {}  /* a=0 b=0 c=0 d=3 -> specificity = 0,0,0,3 */
h1 + *[rel=up]{}  /* a=0 b=0 c=1 d=1 -> specificity = 0,0,1,1 */
ul ol li.red  {}  /* a=0 b=0 c=1 d=3 -> specificity = 0,0,1,3 */
li.red.level  {}  /* a=0 b=0 c=2 d=1 -> specificity = 0,0,2,1 */
#x34y         {}  /* a=0 b=1 c=0 d=0 -> specificity = 0,1,0,0 */
style=""          /* a=1 b=0 c=0 d=0 -> specificity = 1,0,0,0 */
```

Пример:
```plaintext
/* 1 attribute, 2 types -> specificity = 0-1-2 */
html div[id^="blue"] {
background-color: blue
}

/* 1 ID                 -> specificity = 1-0-0 */
#blue4 {
    background-color: red
}
```
##  Дополнительные ссылки

1. Безбарьерный интернет
2. Verordnung zur Schaffung barrierefreier Informationstechnik nach dem Behindertengleichstellungsgesetz (Barrierefreie-Informationstechnik-Verordnung - BITV 2.0
3. Float - повторить
4. Переменные в CSS https://developer.mozilla.org/ru/docs/Web/CSS/Using_CSS_custom_properties
5. Что такое модульные сетки https://setka.io/rublog/why-you-should-use-grids/
6. Медиа запросы https://developer.mozilla.org/ru/docs/Web/CSS/Media_Queries/Using_media_queries
7. Закладка о странице печати - https://andron13.de/school/frontend/css/11-css-media-queries-print-version/

## Домашнее задание № 1

1. Для чего используются теги dt, dd, dl?
2. Используя dt, dd, dl создай html файл с описанием тегов:
   abbr, address, aside, code, caption, cite, fieldset, figcaption, legend, mark, output, optgroup, option, picture, progress, section, samp, summary, tfoot, th, thead, time, track, meter, nav, menu, menuitem, keygen, main, embed.
3. Можно ли дважды на странице использовать __h1__?
4. Можно ли дважды на странице использовать __main__?
5. Можно ли дважды на странице использовать __article__?
6. Чем отличается __b__ от __strong__?

## Домашнее задание №2

1. Сделать трёхколоночный сайт: шапка, футер, контент и две боковые колонки. Использовать флоат. 
2. В контентой части должна быть минимум одна "обтекаемая" фотография
3. Сайт должен быть "настоящим". Тематика - ваш сайт, резюме, сайт для друга. В случае если настоящий сайт невозможен -> выбрать тематику из следующих: 
    - Гостиница для животных города Москвы
    - Приют для бездомных животных города Гомеля
    - Продажа породистых кошек в городе Киеве
    - йога курсы в городе Берлине
    - репетитор русского языка в Берлине
    - репетитор немецкого языка в Минске
    - школа программирования в Потсдаме
    - кулинарный сайт с рецептом драников, борща или наполеона
4. Важно. Тематика одна на ученика. Просьба не повторяться и "забить тему" в комментариях и после этого приступать к работе. 
5. Сайт должен отображаться и содержать медиазапросы для мобилы, десктопа(резина) и планшета
6. Обязательно настроить принтверсию страницы. 
7. Использовать собственные переменные для цветов
8. Домашнее задание в идеале закинуть пуллреквестом.
   
   