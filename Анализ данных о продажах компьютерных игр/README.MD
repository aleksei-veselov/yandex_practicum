# Анализ данных о продаже компьютерных игр

**Описание проекта**

Вы работаете в интернет-магазине «Стримчик», который продаёт по всему миру компьютерные игры. Из открытых источников доступны исторические данные о продажах игр, оценки пользователей и экспертов, жанры и платформы (например, Xbox или PlayStation). Вам нужно выявить определяющие успешность игры закономерности. Это позволит сделать ставку на потенциально популярный продукт и спланировать рекламные кампании.

Перед вами данные до 2016 года. Представим, что сейчас декабрь 2016 г., и вы планируете кампанию на 2017-й. Нужно отработать принцип работы с данными. Неважно, прогнозируете ли вы продажи на 2017 год по данным 2016-го или же 2027-й — по данным 2026 года.

В наборе данных попадается аббревиатура ESRB (Entertainment Software Rating Board) — это ассоциация, определяющая возрастной рейтинг компьютерных игр. ESRB оценивает игровой контент и присваивает ему подходящую возрастную категорию, например, «Для взрослых», «Для детей младшего возраста» или «Для подростков».

# Вывод:
При планировании интернет-магазину «Стримчик» рекламных кампании для различных игр в 2017-ом году стоит ориентироваться на следующие игровые платформы:
- PS4;
- Х360;
- PS3;


При расммотрении отзывов критиков и пользователей c осторожностью стоит ориентироваться на оценки критиков, чем пользователей, т.к. корелляция между оценками критиков и продажами игр немного выше. 

Среди жанров наиболее продаваемыми являются Shooter, Sports и Action.

При рассмотрении особенностей региональных продаж при выборе пользователями игровых платформ и жанров, можно отметить схожесть предпочтений в Северной Америке и Европе. Выбор пользователей Японии, значительно отличается от проанализированных регионов. 
****
Региональные отличия заметны как в выборе пользователями игровых платформ, так и жанров, при этом в Северной Америке и Европе предпочтения схожи между собой, а в Японии заметно отличаются. Также различия по популярности платформ зависят от влияния бренда производителя. 

**Платформы**
- В Северной Америке компания Microsoft (XOne и X360);
- В Японии компания Nintendo (3DS и WiiU);
- Рынок Европы опирается на общую популярность платформ из-за отсутсвия крупных игроков.

**Жанры**
 В Северной Америке и Европе популярны: Action, Shooter, Sports, Role-Playing.
 В Японии популярны: Role-Playing, Action, Misc, Platform.

Ориентироваться на ретинг ESBR стоит в Европе и Северной Америке, т.к. в Японии много игр без этой оценки (игры, созданные в самой Японии). Стоит отметить, что рейтинг ESRB предназначен для рецензирования игр на территории Северной Америки (США, Канады, Мексики).

****
**Проверка гипотез**
- Средние пользовательские рейтинги платформ Xbox One и PC скорее всего одинаковые
- Средние пользовательские рейтинги жанров Action и Sports скорее всего разные
