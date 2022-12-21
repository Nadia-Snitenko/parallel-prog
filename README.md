## Параллельное программирование 
#### Лабораторная №3
**Задание:** 
 Модифицировать программу из л/р №2 для параллельной работы по технологии MPI.

**Результат:** 
1. ***matrix_1.txt*** - файл с исходной матрицей №1
2. ***matrix_2.txt*** - файл с исходной матрицей №2
3. ***matrix_3.txt*** - файл с результирующей матрицей
4. ***time.txt**** - время, за которое в среднем перемножаются матрицы разных размеров с разным количеством работающих потоков 

{ 100, 150, 200, 250, 300,350, 400, 500, 600, 700, 800, 900, 1000} - размеры квадратных матриц, используемые для анализа 
зависимости времени работы от величины матрицы

**Вывод:**  
Время работы программы для перемножения матриц, написанная на языке С++ увеличивается в 2 раза, 
когда размеры матриц увеличивается на 100. При перемножении матриц 1000x1000 код отрабатывает 16 секунд,
что достаточно долго.

#### Зависимость времени от количества процессов
Размер матрицы: 100x100 - 400x400 элементов
![time_100-400](https://user-images.githubusercontent.com/90641953/208870036-425af75e-db69-47d1-8806-c0d3fe144e72.png)

Матрица: 1000x1000 элементов
![image](https://user-images.githubusercontent.com/90641953/208862948-6ae48c63-0c56-4c64-92c7-ee34c5a704ba.png)
