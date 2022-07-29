# Задачи


1. Реализовать численное нахождение определённых интегралов от произвольной функции (квадратурные формулы треугольников, трапеций, Симпсона).
2. Выполнить тестирование на 8 различных тестовых интегралах. Сравнить погрешности полученных результатов. (Интегралы для точной оценки можно вычислить в ручную) 
3. Построить графики функций и квадратур. Сравнить погрешности полученных для различного числа точек, разбивающих отрезок.  
 
 
 Краткое описание выполнения задания:
1. Создаем форму и обработчики событий.
2.	Определяем основной класс программы.
	* Класс - математическая функция которую нужно проинтегрировать. 
	Область определения функций это наш отезок интегрирования от a до b с указанным шагом.
	Область значений это массив значений выбранной функции, которые она принимает при переборе всех x из области определения.
	
	Используемые методы:
	
	*	Метод трапеций
	*	Метод центральных прямоугольников.
	*	Метод Симпсона
	
3.	Определяем массив из 8 функций которые хотим проинтегрировать: 

	*	y=sin(x)    									
	*	y=cos(x)  									
	*	y=2*x²									
	*	y=x                                                       
	*	y=5ᵡ                                                      
	*	y=1/5²+x²                                                 
	*	y=eᵡ                                                      
	*	y=(x+2)³

4.	Оцениваем погрешности для двух первых методов по формулам:
	
	![image](https://user-images.githubusercontent.com/39415744/181807716-fc73b547-ccd8-436b-942a-b9b0a437d9d9.png)
	
	![image](https://user-images.githubusercontent.com/39415744/181807945-b301776e-25e6-4ef9-a203-8982ec287702.png)

Использовать при отображении погорешностей знак ± мы считаем уместным, так как при вычислении второй производной была использована приближенная формула для вычисления производной, которая тоже зависит от выбранной точности интегрирования и дает собственную погрешность.

![image](https://user-images.githubusercontent.com/39415744/181814642-e9ab1179-363d-4134-96f2-2eca8298d9b7.png)

	
 
# Демонстрация
### Данные интегралы по умолчанию в границах от -4 до 5. Точность по умолчанию 0,1. 
### Графики строятся по результатам метода центральных прямоугольников (это видно если увеличить точность до 0,5).

* Общий функционал

![демонстрация работы](https://user-images.githubusercontent.com/39415744/181803964-fd7d49ba-26d5-4ded-81c6-c9218dc85438.gif)

* Демонстрация зависимости погрешностей от изменения точности

https://user-images.githubusercontent.com/39415744/181811897-327b1359-98f3-4a4b-93d7-eb0685f0ed82.mp4





 
 
 
 


# Выводы
**На выходе получаем программу, которая различными методами высчитывает значения интегралов для 8 заданных функций, и на их основе строит графики.
Мы знаем, что при уменьшении шага h в 2 раза погрешность методов трапеций и прямоугольников уменьшится в 4 раза. На видео**

# Выполнили

   * [Конопченко Л.Б](https://github.com/leonrew) | Работа с кодом (C++ CLR)
   * [Рау М.А](https://github.com/R3MSKy) | Документация проекта
  





