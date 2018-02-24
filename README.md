# CSS tutorail

- [Progressive Enhancement](#progressive-enhancement)
- [Graceful degradation](#graceful-degradation)

## Progressive Enhancement
Прогресивне поліпшення передбачає, що веб-інтерфейси повинні створюватися поетапно, циклічно, від простого до складного. На кожному з етапів повинен виходити закінчений веб-інтерфейс, який буде краще, красивіше і зручніше попереднього. Можна сказати, що зараз таких етапів чотири:

- «Старий-добрий-HTML» етап
- CSS етап
- CSS3 етап
- JavaScript етап

На першому етапі початковий зміст сторінки розмічається за допомогою HTML. На цьому етапі необхідно зробити логічну і семантично правильну розмітку. Ніякого додаткового оформлення не провадиться. В результаті виходить коректно розмічений HTML-документ, який браузер відображає так, як вважає за потрібне. Такий документ можна назвати «найменшим спільним знаменником», так як він буде коректно відображатися в будь-якому, навіть самому простому, браузері. Прогресивне поліпшення наполягає, що перший етап є найважливішим, тому що немає в інтернеті нічого важливішого, ніж зміст.

На другому етапі документ оформляється за допомогою старого доброго CSS і знаходить більш акуратний вигляд: з'являється сітка сторінки, задаються параметри шрифту елементів, фонові зображення і так далі.

На третьому етапі застосовуються нові можливості з сімейства специфікацій CSS3, і документ доводиться до блиску: напівпрозорі плашки, круглі куточки, тіні. Також за допомогою CSS3 можна додати різні анімаційний-декоративні фішечки: поступове згасання або зсув елементів, підсвічування полів форм і так далі.

На четвертому етапі до розуму доводиться процес взаємодії з інтерфейсом: різні AJAX рішення, динамічні елементи, ті ж календарики і так далі. Тут у всю використовується JavaScript. Цей етап відповідає за зручність.

Все ж відзначимо ключові відмінності **Graceful degradation** і  **Progressive Enhancement**:

- Graceful degradation - більш широке поняття, ніж progressive enhancement, який обмежений тільки веб-інтерфейсами. Progressive enhancement - це наше, рідне, вебовское.

- Progressive enhancement задає вектор руху (починай з простого!), А для graceful degradation це не так важливо.

- Progressive enhancement наполягає на важливості змісту, а для graceful degradation воно на другому плані.

## Graceful degradation
Це здатність системи продовжувати своє функціонування в разі відмови деяких її компонентів. І чим серйозніше відмова призводить до погіршення якості роботи системи і роботи з системою.

Ця замітка присвячена більш окремого випадку поступової деградації, а саме відмовостійкості динамічних веб-інтерфейсів і в ній розбирається приклад побудови і роботи такого інтерфейсу.

Основна ідея при проектуванні таких інтерфейсів полягає в наступному: «Користувач може повноцінно працювати з системою і з повністю відключеним JavaScript. Однак, з включеним JavaScript йому буде набагато зручніше ».

Веб-дизайн, який заснований на принципі graceful degradation, спочатку призначений для перегляду в сучасних браузерах, тоді як в старих браузерах він буде відображатися з тим же функціоналом і набором можливостей, але при цьому з меншою кількістю особливостей

Основна відмінність між принципами **graceful degradation** і **progressive enhancement** це те, звідки починається дизайн. Якщо починати верстку з найстарішого, але все ще общеіспользуемих браузера, а після додавати деякі особливості для новіших версій, то це - **progressive enhancement**. Якщо ж починати створення сайту під новітні браузери, а потім просто «урізати» деякі наріжні особливості для старіших - це і є принцип **graceful degradation**.

