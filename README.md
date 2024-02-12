## Решение конфликтов слияния Git.

Дана схема git-репозитория. Есть исходная ветка main и ветки, содержащие изменения, которые не могут быть применены одновременно. В зависимости от изменений на экран выводится тот или иной рецепт пиццы.
Задачей является слить (merge) ветки [big-pepper, middle-chicken, small-cheese] в ветку main и решить возникающие конфликты. 
Решением практической работы будет полученная в результате слияния веток пицца.

**Задание 1. Сделать форк данного репозитория.**

Ссылку на форк прикрепить к соответствующей задаче в карточке на доске в Taiga.

**Задание 2. Получить в результате слиянии веток пиццу по рецепту из варианта.**

Результатом будет скриншот с выводом результата при выполнении файла main.py, а так же история слияний с репозитория.
Данные результаты приложить к задаче на карточке.

Для решения можно воспользоваться утилитой Meld на Linux/Windows или Kdiff на MacOS.

Инструкция для установки инструмента разрешения конфликтов: https://git-scm.com/docs/git-mergetool
Пример команды:

```
git mergetool [--tool=<tool>], где <tool> ставите meld или kdiff
```
```
git mergetool --tool=kdiff
```

Инструкция для котлеток:
Есть main. В нём ничего нет. И есть три ветки: [big-pepper, middle-chicken, small-cheese], в которых наши программисты создали три полных комплекта из основы и ингредиентов (сначала создаётся основа, потом, один за другим, добавляются ингредиенты начинки). 
Задача состоит в том, чтобы смёрджить три ветки в одну, и в результате получить пиццу из варианта.

Форкаем репозиторий, и по одной мёрджим ветки [big-pepper, middle-chicken, small-cheese] в main, попутно решая конфликты так, чтобы получить нужный результат.

Варианты рецептов (выбираются согласно номеру в журнале):

 1. [middle pizza][pepper][cheese][chicken]
 2. [big pizza][pepper][cheese][chicken]
 3. [big pizza][cheese][pepper][cheese]
 4. [small pizza][pepper][cheese][chicken]
 5. [middle pizza][cheese][cheese][cheese]
 6. [small pizza][cheese][chicken][cheese]
 7. [middle pizza][cheese][cheese][chicken]
 8. [middle pizza][chicken][chicken][pepper]
 9. [small pizza][cheese][cheese][cheese]
10. [middle pizza][chicken][cheese][cheese]
11. [big pizza][cheese][pepper][cheese]
12. [middle pizza][cheese][chicken][cheese]
13. [big pizza][cheese][pepper][pepper]
14. [big pizza][chicken][chicken][pepper]
15. [small pizza][pepper][cheese][pepper]
16. [middle pizza][chicken][cheese][chicken]
17. [small pizza][chicken][chicken][pepper]
18. [big pizza][chicken][chicken][chicken]
19. [middle pizza][cheese][chicken][cheese]
20. [middle pizza][cheese][cheese][cheese]
21. [big pizza][pepper][pepper][pepper]
22. [big pizza][cheese][cheese][chicken]
23. [middle pizza][pepper][pepper][chicken]
24. [big pizza][pepper][cheese][cheese]
25. [small pizza][cheese][chicken][pepper]
26. [big pizza][chicken][cheese][pepper]
27. [middle pizza][pepper][chicken][chicken]
28. [big pizza][chicken][chicken][chicken]
29. [middle pizza][cheese][chicken][chicken]
30. [small pizza][cheese][pepper][chicken]
31. [small pizza][chicken][cheese][pepper]
32. [small pizza][chicken][chicken][chicken]
33. [middle pizza][pepper][chicken][chicken]
34. [middle pizza][cheese][pepper][cheese]
35. [small pizza][chicken][cheese][chicken]
   
   
