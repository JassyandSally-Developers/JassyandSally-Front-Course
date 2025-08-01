div{background-color:blue;}
Селектор CSS это конструкция которая позволяет выбрать отдельные или однотипные элементы на странице чтобы их стилизовать.
Селектор (div) он выбирает кокретный элемент на странице потом после фигурных скобок указывается свойства со значениями (background-color) и между ними ставится двоеточие (:) сами свойства обязательно отделяются друг от друга  точкой запятой (;) .
Несколько свойств можно писать все одну строку :
div{
    background:blue;
    width:100%;
}
Фреймворке bootstrap вы можете встретить второй или как его назвают минимизированы вариант CSS там где все стили написины в одну строку.
1) Во первых селектор по тегу то есть мы сразу указываем тег и прописываем свойства .Этот селектор применяет ли ко всем элементам определенного .
2) Свойства второй селектора - это селектр по классу ( нам нужно задать отдельный класс для отдельного элемента):
<p class="text">
Lorem ipsum dolar sit amet .
</p>
<p id="text2">
Lorem ipsum dolar sit amet .
</p>
<style>
    .text{
        color:black
        background-color: yellow
    }
    #text2{
        color:yellow
        background-color: black
    }
</style>
Вид селектора-это селектор по отрибуту .Создадим форму,несколько инпутов , один у нас будет с тайпом , текст другой возмем с тайпом (email) третий будет с тайпом (password) :
<form action="#">
<input type="text"><input type="email"><input type="password">
</form>(стилизовать по отрибуту:)
<style>
    input[type="text"]{
        border:3px ;
    }
    input[type="email"]{
        border:3px ;
    }
    input[type="password"]{
        border:3px ;
    }
    form{display:flex 
    flex-direction: column;}
</style>



