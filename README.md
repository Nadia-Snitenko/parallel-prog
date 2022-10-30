# Параллельное программирование 

### Лабораторные работы:

Параллельные версии программ рекомендуется запускать на суперкомпьютере «Сергей Королёв».

Порядок выполнения л/р:
1. Создание и отладка программы.
2. Исследование программы (зависимости времени выполнения от объема задачи и параметров распараллеливания).
3. Отчёт в электронной форме содержащий задание, исходный код решения (можно ссылкой на github/gitlab) , результаты экспериментов и выводы.
4. Защита отчёта – собеседование.


#### Лабораторная №1
**Задание:** 
1. Написать программу на языке C/C++ для перемножения двух матриц.  
   **Исходные данные:** файл(ы) содержащие значения исходных матриц.  
   **Выходные данные:** файл со значениями результирующей матрицы, время выполнения, объем задачи.
2. Обязательна автоматизированная верификация результатов вычислений с помощью сторонних библиотек или стороннего ПО (например Matlab).

*При желании, в качестве экспериментальной задачи можно выбрать любую другую вычислительную задачи, которая подвержена распараллеливанию.*

**Результат:** 
1. ***matrix_1.txt*** - файл с исходной матрицей №1
2. ***matrix_2.txt*** - файл с исходной матрицей №2
3. ***matrix_3.txt*** - файл с результирующей матрицей
4. ***check_in_python.py*** - проверка в Python перемножения матриц и построение графика зависимости
5. ***time.txt**** - время, за которое в среднем перемножаются матрицы разных размеров  
{10, 50, 100, 150, 200, 250, 300,350, 400, 500, 600, 700, 800, 900, 1000} - размеры квадратных матриц, используемые для анализа 
зависимости времени работы от величины матрицы
6. ***graph.png*** - график зависимости времени от размера матрицы

**Вывод:**  
Время работы программы для перемножения матриц, написанная на языке С++ увеличивается в 2 раза, 
когда размеры матриц увеличивается на 100. При перемножении матриц 1000x1000 код отрабатывает 16 секунд,
что достаточно долго.

#### Лабораторная №2
 Модифицировать программу из л/р №1 для параллельной работы по технологии OpenMP.

#### Лабораторная №3
 Модифицировать программу из л/р №2 для параллельной работы по технологии MPI.

#### Лабораторная №4
 Модифицировать программу из л/р №3 для параллельной работы по технологии CUDA.