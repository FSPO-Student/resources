## input

Чтобы добавить в форму текстовое поля, мы можем воспользоваться тегом `input`.

```html
<form action="/example" method="GET">
   <h6>Наша первая форма</h6> 
   <input type="text" name="username" placeholder="Введите свое имя"/>
   <input type="number" name="phone" placeholder="Введите свой номер телефона"/>
   <input type="text" name="race" value="Человек"/>
</form>
```

Результат:

<div class="html">
    <form action="/example" method="GET">
       <h6>Наша первая форма</h6> 
       <input class="form-control" type="text" name="username" placeholder="Введите свое имя"/>
       <input class="form-control" type="number" name="phone" placeholder="Введите свой номер телефона"/>
       <input class="form-control" type="text" name="race" value="Человек"/>
    </form>
</div>

Атрибут `type` используется для указания типа вводимых данных. В нашем примере - это текст (text) и число (number).

> Кроме `text` и `number` существуют следующие типы:
> * password - используется для ввода пароля,
> * url - для ввода url,
> * email - для ввода email,
> * file - для отправки файла,
> * checkbox - для добавления флажка,
> * radio - для добавления переключателя.
>
> Список остальных типов вы можете найти [тут](https://html5book.ru/html5-forms/).

Атрибут `name` указывает имя параметра, который будет передавать обработчику на backend при нажатии на кнопку "Отправить".

`placeholder` - задает текст, отображаемый до заполнения. Обычно оно используется для подсказки.

Ну и `value`, с помощью которого мы можем задать начальное значение введенное в поле. В нашем примере мы предустановили значение **Человек**.

Больше информации о атрибутах вы можете найти [вотут](https://html5book.ru/html5-forms/).

### Задание

Добавьте в форму четыре поля:
- текстовое ФИО,
- email,
- номер телефона,
- ссылку на портфолио.

Не забудьте про соответствующий `type` для каждого поля.