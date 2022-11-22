# Туториал по языку разметки MarkDown

## как добавить исходный код 
В чистом Маркдауне блоки кода отбиваются 4 пробелами в
начале каждой строки.
Но в GitHub-Flavored Markdown (сокращенно GFM) есть
более удобный способ: ставим по три апострофа (на букве
Ё) до и после кода. Также можно указать язык исходного
кода.

```html
<nav class="nav nav-primary">
 <ul>
 <li class="tab-conversation active">
 <a href="#" data-role="post-count"
class="publisher-nav-color" data-nav="conversation">
 <span class="comment-count">0
комментариев</span>
 <span class="comment-countplaceholder">Комментарии</span>
 </a>
 </li>
 <li class="dropdown user-menu" data-role="logout">
 <a href="#" class="dropdown-toggle" datatoggle="dropdown">
    <span class="dropdown-toggle-wrapper">
 <span>
 Войти
 </span>
 </span>
 <span class="caret"></span>
 </a>
 </li>
 </ul>
</nav>
```
Самое приятное, что в коде не нужно заменять угловые
скобки `< >` и амперсанд `&` на их html-сущности.

## как добавить инлайн код
Для вставки кода внутри предложений нужно заключать этот
код в апострофы (на букве Ё). Пример: `<html class="ie
no-js">`.
Если внутри кода есть апостроф, то код надо обрамить
двойными апострофами: ``There is a literal backtick (`)
here.``

## Как использовать HTML в нутри Markdown

Mожно смешивать Markdown и HTML. Если на какие-то
элементы нужно поставить классы или атрибуты, смело
используем HTML:
> Выделять слова можно при помощи * и _ . Например, это
<em class="a1">italic</em> и это тоже <i
class="a1">italic</i>. А вот так уже <b>strong</b>, и
так тоже <strong>strong</strong>.
Можно и наоборот, внутри HTML-тегов использовать
Маркдаун.
<section class="someclass">
### Пример Маркдауна внутри HTML
Выделять слова можно при помощи `*` и `_` . Например,
это _italic_ и это тоже *italic*. А вот так уже
__strong__, и так тоже **strong**.
</section>


## как применить Маркдауна внутри HTML

### Пример Маркдауна внутри HTML
Выделять слова можно при помощи `*` и `_` . Например,
это _italic_ и это тоже *italic*. А вот так уже
__strong__, и так тоже **strong**.

## как добавить таблице
В чистом Маркдауне нет синтаксиса для таблиц, а в GFM
есть.
First Header | Second Header
------------- | -------------
Content Cell | Content Cell
Content Cell | Content Cell
Для красоты можно и по бокам линии нарисовать:
| First Header | Second Header |
| ------------- | ------------- |
| Content Cell | Content Cell |
| Content Cell | Content Cell |
Можно управлять выравниванием столбцов при помощи
двоеточия.
| Left-Aligned | Center Aligned | Right Aligned |
|:------------- |:---------------:| -------------:|
| col 3 is | some wordy text | **$1600** |
| col 2 is | centered | $12 |
| zebra stripes | are neat | ~~$1~~ |
Внутри таблиц можно использовать ссылки, наклонный,
жирный или зачеркнутый текст.
Для всего остального есть обычный HTML.

## Как сделать горизонтальную черту
 `hr` создается тремя звездочками или тремя дефисами.
***