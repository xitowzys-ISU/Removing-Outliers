# Зачетная работа по анализу данных (Вариант #4)

## Задача
Написать программу для удаления выбросов и удалить выбросы.

## Требования
1. Программа для обработки
2. Описание на страницу - как работает, какие результаты


## Структура проекта

1. [`data` - Папка с датасетами](https://gitlab.com/ISU-Applied-Computer-Science/5th-semester/data-analysis/removing-outliers/-/tree/main/data)
2. [`raw` - Папка для файла README.md](https://gitlab.com/ISU-Applied-Computer-Science/5th-semester/data-analysis/removing-outliers/-/tree/main/raw)
3. [`exam.ipynb` - Реализация функционала удаление выбросов из датасета](https://gitlab.com/ISU-Applied-Computer-Science/5th-semester/data-analysis/removing-outliers/-/blob/main/exam.ipynb)

## Краткое описание блокнота

### [`exam.ipynb`](https://gitlab.com/ISU-Applied-Computer-Science/5th-semester/data-analysis/removing-outliers/-/blob/main/exam.ipynb)

1. Импорт необходимых библиотек
2. Загружает датасет в массив и визуализируем его
3. Чтобы увидеть более хошоро, где могут быть выбросы вырезаем линейный тренд 
4. Визуализируем полученный результат
5. Делим датасет на ровные части. В данном примере датасет поделен по 1%
6. Ищем среднее крадратичное отклонение и выявляем отклонения для каждой части датасета
7. Отделяет отдельно выбросы и датасет без выбросов
8. Заносим все в массивы
   ```python
    outliers = [] # Выбросы
    outliers_removed = [] # Чистые данные
   ```
9. Визуализируем полученные результаты

#### Дополнительно

Были попытки найти выборосы кластеризатор DBScan

## Результаты

| Чистый датасет |
| ------------------------------------------------------------ |
| ![demo_1](https://gitlab.com/ISU-Applied-Computer-Science/5th-semester/data-analysis/removing-outliers/-/raw/main/raw/demo_1.png?inline=false) |

| Датасет с отмеченными точками которые попали под выброс |
| ------------------------------------------------------------ |
| ![demo_1](https://gitlab.com/ISU-Applied-Computer-Science/5th-semester/data-analysis/removing-outliers/-/raw/main/raw/demo_2.png?inline=false) |

| Датасет без выбросов |
| ------------------------------------------------------------ |
| ![demo_1](https://gitlab.com/ISU-Applied-Computer-Science/5th-semester/data-analysis/removing-outliers/-/raw/main/raw/demo_3.png?inline=false) |

| Датасет с выбросами |
| ------------------------------------------------------------ |
| ![demo_1](https://gitlab.com/ISU-Applied-Computer-Science/5th-semester/data-analysis/removing-outliers/-/raw/main/raw/demo_4.png?inline=false) |

| Попытка использовать кластеризатор DBScan |
| ------------------------------------------------------------ |
| ![demo_1](https://gitlab.com/ISU-Applied-Computer-Science/5th-semester/data-analysis/removing-outliers/-/raw/main/raw/demo_5.png?inline=false) |