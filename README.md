# result.txt
## Домашнее задание №9: Регулярные выражения
1. *Первым пунктом* было удалить все пустые строки. Я сделала это при помощи регулярного выражения: ^\s+ . Графу "Replace" я оставила пустой.
![Удаление пустых строчек](https://pp.userapi.com/c831409/v831409374/10f17c/MEYTu7rj6Do.jpg "")
2. *Вторым заданием* было найти всех князей и города, имя и название которых оканчивается на "слав". Использовалось регулярное выражение: [А-ЯѢ]+[а-яѣ]+(слав)[а-яѣ]+ . Всего найдено 564 вхождения.
![Князья и города](https://pp.userapi.com/c831409/v831409374/10f172/wa4WOqrX9-c.jpg "")
3. *Третьим заданием* было найти все упоминания Новогорода. Я использовала регулярное выражение: (Нов)+.(город)[^W] . Найдено 58 упоминаний Новогорода.
![Упоминания Новгорода](https://pp.userapi.com/c831409/v831409374/10f168/tm9LHFF3SLc.jpg "")
4. *БОНУС*
Бонусным пунктом было отредактировать текст следующим образом:
- надо добавить пробел после двоеточия;  
- надо добавить пробел после запятой;  
- надо добавить пробел после точки с запятой;  
- перед квадратной скобкой должен быть пробел;  
- после точки должен быть пробел, если до нее буква или кавычка, а после нее нет другой точки.  
Для начала я использовала регулярку ([!,.;:"]) с заменой \1  
![БОНУС 1](https://pp.userapi.com/c834301/v834301558/157890/YwggdNXxMs8.jpg "")
Затем я сделала вторую регулярку (\[) так же с заменой \1, чтобы удовлетворить предпоследнему условию, где перед квадратной скобкой должен быть пробел.  
![БОНУС 2](https://pp.userapi.com/c834301/v834301558/157886/vP3e0sxX2Gg.jpg "")
И наконец я ввела регулярное выражение . . . и заменила его на ... , чтобы исключить наличие пробелов между точками в многоточии.  
![БОНУС 3](https://pp.userapi.com/c834301/v834301558/15789a/s0B-O_Fw8HE.jpg "")
Также я заменила два пробела на один, чтобы окончательно привести текст в порядок.
![БОНУС 4](https://pp.userapi.com/c834301/v834301558/15787c/ldbroygC_nA.jpg "")
