# Решающее дерево. Алгоритм ID3.
Задача: Реализовать алгоритм ID3. На входе получаем editor_corrected.csv с информацией по используемым текстовым редакторам, 
языкам программирования и другим данным. Необходимо построить решающее дерево для целевого признака "Операционная система"

# Решение
Код алгоритма находится в файле id3.ipynb

# Установка
Понадобится pandas и [GraphViz](https://www.graphviz.org/).
Для установки graphviz можно установить [бинарные файлы](https://graphviz.gitlab.io/_pages/Download/Download_windows.html),
а также выполнить команду:
```
conda install graphviz
conda install python-graphviz
```
Возможно  потребуется установить переменные среды:
```
C:\Program Files (x86)\Graphviz2.38\bin в User path
C:\Program Files (x86)\Graphviz2.38\bin\dot.exe в System Path
```
Это гарантирует, что graphviz будет работать корректно.

В качестве исходных данных используется файл **editor_corrected.csv** в нем убрана строка "vim,Python,tea,windows" так как она противоречит другой строке с os unix, если использовать аутентичные данные программа уйдет в бесконечный цикл. Целевой атрибут в **id3.ipynb** задается константой TARGET_COLUMN.
При разработке использовались следующие источники:
- https://medium.com/machine-learning-guy/an-introduction-to-decision-tree-learning-id3-algorithm-54c74eb2ad55
- https://logic.pdmi.ras.ru/~sergey/teaching/mlcsclub/02-dectrees.pdf
- https://www.youtube.com/watch?v=UdTKxGQvYdc&t=357s
- https://github.com/Bladefidz/machine-learning-tutorials/blob/master/decision-tree/decision_tree.py
- https://github.com/tofti/python-id3-trees
- https://github.com/svaante/decision-tree-id3


Кирилл Прохоров<br>
Павел Смирнов<br>
Альберт Латыпов<br>
Глеб Довгерд<br>
Игнат Довгерд<br>
