# Lab_2: Автоматизація. Знайомство з CI/CD.

## Pre-requirements:
- віртуальна машина на основі Ubuntu 18.04;
- встановлено програми git, make, Python 3.7, PIP;

## Хід роботи
1. Створив папку lab_2 з README-файлом.
2. Встановив `pipenv` та створив середовище для Python. Ознайомився з командою `pipenv -h`
![](img/pipenv_install.png)
3. Встановив необхідні бібліотеки (`requests`, `ntplib`):
![](img/libinstall.png)
4. Створив файл `app.py`, скопіював код з репозиторію.
5. Перевірив чи програма працює:
![](img/app_works.png)
6. Встановив бібліотеку `pytest`:
![](img/pytest-install.png)
7. Запустив тести:
![](img/tests_run.png)
8. (Захист) - Дописав у програмі функцію для перевірки часу доби (AM/PM) та друкування фрази - "Доброго дня!"/"Доброї ночі":
- ![](img/time_app.png)
- ![](img/time_app_run.png)
9. Написав тести, що перевіряють правильність виконання програми, а також доповнив програму:
- Програма: ![](img/app_rewrote.png)
- Тести: ![](img/tests_rewrote.png)
- Запуск: ![](img/tests_rrun.png)
10. Вивів результат виконання тестів та програми у файл використовуючи оператор спрямування стандартних потоків: `>` - з перезаписом, `>>` - з дописом в кінець файлу. В обох випадках, якщо файл не існує - його буде створено. :
![](img/pipe-to-file.png)
11. Зробив коміт зі змінами
12. Заповнив `Makefile`:
![](img/makefile.png)
13. Закомітив зміни та перейшов на віртуальну машину.
14. Склонував репозиторій та перейшовши в папку запустив `make`.
15. Зроблено