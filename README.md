# antifraud_otus_ml
## Подготовительные расчеты

- 31 536 000 секунд = 1.57 * 10^9 транзакций 

- Максимальное нагрузка в праздники 400 транз / сек. Закладываем х2-х3. 

- Максимальная ошибка FP = 5% 

- FN – 2% - приводят к убыткам 500 т.р. / мес 

## Цели

Разработать антифрод систему: 

- Поддерживающий в 800 транзакций в секунду (х2 от максимальной  нагрузки) 

- FP не должно превышать 5% 

- FN не должно превышать 2% 

- Ущерб клиентов в месяц не более 500 т.р. 

## Метрики машинного обучения

В качестве метрики максимизации предлагается использовать ROC-AUC. С ее помощью предоставляется возможным сравнивать различные подходы между друг другом, не опираясь на подбор порогов. Также модель менее чувствительна к несбалансированным классам, что актуально в антифроуд системе. 

Также при разработке алгоритма необходимо учитывать и финансовую составляющую ошибок, которую допускает наша модель, поэтому считаю необходимым отслеживать и вторую метрику как ущерб клиентов, то есть какая сумма транзакций входит в FN.  


## MISSION Canvas 

![Межкамерный - Frame 13](https://github.com/Misterrendal/antifraud_otus_ml/assets/32695551/e407024f-fb93-48ec-a561-201352f7cc39)

## Функциональные части проекта

- Исследовательские работы по обучению предсказательной модели 

- Backend 

- Настройка сервера 

- Тестирование 
