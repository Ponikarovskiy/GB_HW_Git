# \*\*\* Моя инструкция по работе с git \*\*\*

## 1. Подготовка рабочего пространства:

старт

* [Скачать](https://git-scm.com/book/en/v2/Getting-Started-Installing-Git) и установить GIT;
![логотип_git](https://nsfocusglobal.com/wp-content/uploads/2020/04/git.jpg)
* [Скачать](https://code.visualstudio.com/) и установить VSС
![логотип_VSC](https://media.vlpt.us/images/namtaehyun/post/fe5d86d3-f734-4943-b087-3f3e02b9d5ab/vscode.png?w=768)
* Создать пустую папку (репозиторий) для дальнейшей работы;
* Запустить VSC;
* Запустить терминал;
* Открыть созданную ранее папку (репозиторий);
* Создать файл в репозитории с расширением *md;
* При первом использовании необходимо представиться GITу

    Введя команды:

    git config --global user.email "ВАШ email"

    git config --global user.name "ВАШЕ Имя"

* В поле "Терминал" вводим "git init" для отслеживания всех изминений в нашей папке.

## 2. Основные команды Git

* git init - инициализация локального репозитория
* git status - получить информацию от git о его текущем состоянии
* git add - добавить файл или файлы к следующему коммиту
* git commit -m "message" - создание коммита
* git log - вывод на экран истории всех коммитов с их хеш-кодами
* git branch - посмотреть список веток в репозитории
* git branch <название ветки> - создать новую ветку
* git checkout <название ветки> - переход к другой ветке
* git branch -d <название ветки> - удалить ветку

## 3. Заголовки

Заголовки отмечаются диезом `#` в начале строки, от одного до шести. 

Например:
# Заголовок h1
## Заголовок h2
### Заголовок h3
#### Заголовок h4
##### Заголовок h5
###### Заголовок h6

## 4. Списки

Для разметки неупорядоченных списков можно использовать или `*`, или `-`, или `+`:

- элемент 1
- элемент 2
- элемент ...

Вложенные пункты создаются четырьмя пробелами перед маркером пункта:

* элемент 1
* элемент 2
    * вложенный элемент 2.1
    * вложенный элемент 2.2
* элемент ...

Упорядоченный список:

1. элемент 1
2. элемент 2
    1. вложенный
    2. вложенный
3. элемент 3
4. элемент 4

На самом деле не важно как в коде пронумерованы пункты, главное, чтобы перед элементом списка стояла цифра (любая) с точкой. Можно сделать и так:

0. элемент 1
0. элемент 2
0. элемент 3
0. элемент 4

## 5. Цитаты

Цитаты оформляются как в емейлах, с помощью символа `>`.

> This is a blockquote with two paragraphs. Lorem ipsum dolor sit amet,
> consectetuer adipiscing elit. Aliquam hendrerit mi posuere lectus.
> Vestibulum enim wisi, viverra nec, fringilla in, laoreet vitae, risus.
>
> Donec sit amet nisl. Aliquam semper ipsum sit amet velit. Suspendisse
> id sem consectetuer libero luctus adipiscing.

Или более ленивым способом, когда знак `>` ставится перед каждым элементом цитаты, будь то абзац, заголовок или пустая строка:

> This is a blockquote with two paragraphs. Lorem ipsum dolor sit amet,
consectetuer adipiscing elit. Aliquam hendrerit mi posuere lectus.
Vestibulum enim wisi, viverra nec, fringilla in, laoreet vitae, risus.
>
> Donec sit amet nisl. Aliquam semper ipsum sit amet velit. Suspendisse
id sem consectetuer libero luctus adipiscing.

В цитаты можно помещать всё что угодно, в том числе вложенные цитаты:

> ## This is a header.
>
> 1.   This is the first list item.
> 2.   This is the second list item.
>
> > Вложенная цитата.
>
> Here's some example code:
>
>     return shell_exec("echo $input | $markdown_script");