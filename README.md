f33-js-project1
Natalia
Девчонки, ловите код-ревью на ваш проект:
Верстка
https://github.com/itgirlschool/f33-js-project1/blob/cd00a3ef2a59abf43f434c2d6e02d9bca3d33404/index.html#L25 Ссылка на корень сайта это /
https://github.com/itgirlschool/f33-js-project1/blob/cd00a3ef2a59abf43f434c2d6e02d9bca3d33404/index.html#L216 Если по БЭМ, то классы могут быть примерно такие articles -> articles-wrap -> articles__cards -> articles__card -> card__title + card__date и тд
 https://github.com/itgirlschool/f33-js-project1/blob/cd00a3ef2a59abf43f434c2d6e02d9bca3d33404/index.html#L260 тут доделать микроразметку и ссылки на соц сети по примерам, которые я скидывала.
В целом верстка сделана хорошо :+1: Правильно разбита на блоки, в большинстве случаев правильно подобраны имена классов по БЭМ.
js.js
Индексный (главный, корневой) файл js принято называть index.js :подмигивание: (edited)
https://github.com/itgirlschool/f33-js-project1/blob/cd00a3ef2a59abf43f434c2d6e02d9bca3d33404/js/js.js#L6 лучше scrollHandler
 https://github.com/itgirlschool/f33-js-project1/blob/cd00a3ef2a59abf43f434c2d6e02d9bca3d33404/js/js.js#L16 и https://github.com/itgirlschool/f33-js-project1/blob/cd00a3ef2a59abf43f434c2d6e02d9bca3d33404/js/js.js#L24 эти 2 участка кода лучше не оставлять просто в глобальной области видимости и обернуть в функции с "говорящими" именами. Так вы улучшите читаемость кода и избежите непредсказуемого поведения вашего кода.
cart.js
https://github.com/itgirlschool/f33-js-project1/blob/cd00a3ef2a59abf43f434c2d6e02d9bca3d33404/js/cart.js#L7 Лучше showQuantity или displayQuantity (edited)
https://github.com/itgirlschool/f33-js-project1/blob/cd00a3ef2a59abf43f434c2d6e02d9bca3d33404/js/cart.js#L14 вот эта функция написана и использована отлично (edited)
 products.js
https://github.com/itgirlschool/f33-js-project1/blob/cd00a3ef2a59abf43f434c2d6e02d9bca3d33404/js/products.js#L67 Если уж создавать класс, то это будет Product :подмигивание: И не забывайте, зачем нам нужны классы: чтобы создавать объекты одного типа. У вас эти объекты уже есть (ваш JSON), поэтому не вижу особого смысла писать тут класс. (edited)
В этом файле в принципе можно было написать 2 функции: renderProductList(data)  и addEventListeners(selectedItems)
tips&trick.js
Лучше не используйте небуквенные символы в названиях файлов. Иногда это приводит к багам чтения таких имен. Лучше tips_tricks или tips_and_tricks
https://github.com/itgirlschool/f33-js-project1/blob/cd00a3ef2a59abf43f434c2d6e02d9bca3d33404/js/tips%26trick.js#L6 не используйте в коде "Магические цифры" :улыбка_во_весь_рот: Тут можно почитать, что это такое и почему их лучше не использовать https://code-basics.com/languages/javascript/lessons/magic-numbers
Над чем еще поработать:
потренируйтесь подключать и настраивать библиотеки.Лучше через npm, но для начала можно и просто ссыкой в head :подмигивание:
Перед добавлением проекта в портфолио обязательно заполните readme файл (несколько слов о проекте и стеке). Будет огромным плюсом, если этот файл будет отредактированным :подмигивание: Вот тут подробнее о редактировании readme https://docs.github.com/en/get-started/writing-on-github/getting-started-with-writing-and-formatting-on-github/basic-writing-and-formatting-syntax
структура проекта в целом правильная, но в идеале еще положить js styles и images в папку assets 
В целом проект написан неплохо :сердце: Немного подправьте его и можно смело добавлять в портфолио 
