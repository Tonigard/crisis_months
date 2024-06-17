# crisis_months
division into a crisis sample

Для разделения временного ряда были использованы следующие данные:
1.	Индекс S&P 500
2.	Данные о 10-летней ставке бондов США
3.	Данные о показателе уровня VIX

Модель MarkovRegression способна формировать несколько линейных моделей, которые могут переключаться между собой при достижении некого порогового значения. В данном случае мы будем иметь два режима: кризис и некризис. 
Каждый день элемент временного ряда модель относит к одному из двух режимов с определенной вероятностью. Кризисным считается месяц, у которого больше 19 кризисных дней. 
