# Lab1
Лабораторная 1
В копиях одинаковый код за исключением train_percent = 0.8, 0.85, 0.9

Задача 1
Так мы мы находим минимум MSE на тестовой выборке. Он достигается :
s_best = MSE_all[MSE_all['MSE_test'] == min(MSE_all['MSE_test'])].index[0]
print(s_best)

![image](https://user-images.githubusercontent.com/98012309/193695827-57444a11-9886-4f93-b805-6f39aa70b6b4.png)

Чем больше наблюдений, через который прошел сплайн, тем точнее будет моделью Лучшая модель будет в минимуме на кривой MSE на тестовой выборке

![image](https://user-images.githubusercontent.com/98012309/193696139-281b683f-064a-4323-b946-842b55595b55.png)

График лучшего сплайна

Задача 2
Меняем train_percent = 0.8, 0.85, 0.9 и можно заметить что меняется сплайн
При train_percent = 0.8, MSE =312
При train_percent = 0.85, MSE =325
При train_percent = 0.9, MSE =324
