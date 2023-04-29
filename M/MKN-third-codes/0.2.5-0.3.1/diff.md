# Comparing `tmp/MKN_third_codes-0.2.5.tar.gz` & `tmp/MKN_third_codes-0.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\MKN_third_codes-0.2.5.tar", last modified: Sat Apr 29 11:33:56 2023, max compression
+gzip compressed data, was "dist\MKN_third_codes-0.3.1.tar", last modified: Sat Apr 29 15:12:22 2023, max compression
```

## Comparing `MKN_third_codes-0.2.5.tar` & `MKN_third_codes-0.3.1.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxrwxrwx   0        0        0        0 2023-04-29 11:33:56.122619 MKN_third_codes-0.2.5/
--rw-rw-rw-   0        0        0     1073 2023-04-29 11:32:30.000000 MKN_third_codes-0.2.5/LICENSE.txt
--rw-rw-rw-   0        0        0       25 2023-04-29 11:33:13.000000 MKN_third_codes-0.2.5/MANIFEST.in
-drwxrwxrwx   0        0        0        0 2023-04-29 11:33:56.107659 MKN_third_codes-0.2.5/MKN_third_codes/
--rw-rw-rw-   0        0        0    15303 2023-04-29 11:21:07.000000 MKN_third_codes-0.2.5/MKN_third_codes/solutions.py
-drwxrwxrwx   0        0        0        0 2023-04-29 11:33:56.120625 MKN_third_codes-0.2.5/MKN_third_codes.egg-info/
--rw-rw-rw-   0        0        0      231 2023-04-29 11:33:56.000000 MKN_third_codes-0.2.5/MKN_third_codes.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      217 2023-04-29 11:33:56.000000 MKN_third_codes-0.2.5/MKN_third_codes.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-29 11:33:56.000000 MKN_third_codes-0.2.5/MKN_third_codes.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       17 2023-04-29 11:33:56.000000 MKN_third_codes-0.2.5/MKN_third_codes.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      231 2023-04-29 11:33:56.122619 MKN_third_codes-0.2.5/PKG-INFO
--rw-rw-rw-   0        0        0       42 2023-04-29 11:33:56.123618 MKN_third_codes-0.2.5/setup.cfg
--rw-rw-rw-   0        0        0      312 2023-04-29 11:30:51.000000 MKN_third_codes-0.2.5/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-29 15:12:22.593488 MKN_third_codes-0.3.1/
+-rw-rw-rw-   0        0        0     1073 2023-04-29 11:32:30.000000 MKN_third_codes-0.3.1/LICENSE.txt
+-rw-rw-rw-   0        0        0       25 2023-04-29 11:33:13.000000 MKN_third_codes-0.3.1/MANIFEST.in
+drwxrwxrwx   0        0        0        0 2023-04-29 15:12:22.579525 MKN_third_codes-0.3.1/MKN_third_codes/
+-rw-rw-rw-   0        0        0    18143 2023-04-29 15:06:54.000000 MKN_third_codes-0.3.1/MKN_third_codes/solutions.py
+drwxrwxrwx   0        0        0        0 2023-04-29 15:12:22.592490 MKN_third_codes-0.3.1/MKN_third_codes.egg-info/
+-rw-rw-rw-   0        0        0      231 2023-04-29 15:12:22.000000 MKN_third_codes-0.3.1/MKN_third_codes.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      217 2023-04-29 15:12:22.000000 MKN_third_codes-0.3.1/MKN_third_codes.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-29 15:12:22.000000 MKN_third_codes-0.3.1/MKN_third_codes.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       17 2023-04-29 15:12:22.000000 MKN_third_codes-0.3.1/MKN_third_codes.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      231 2023-04-29 15:12:22.593488 MKN_third_codes-0.3.1/PKG-INFO
+-rw-rw-rw-   0        0        0       42 2023-04-29 15:12:22.593488 MKN_third_codes-0.3.1/setup.cfg
+-rw-rw-rw-   0        0        0      312 2023-04-29 14:52:43.000000 MKN_third_codes-0.3.1/setup.py
```

### Comparing `MKN_third_codes-0.2.5/LICENSE.txt` & `MKN_third_codes-0.3.1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `MKN_third_codes-0.2.5/MKN_third_codes/solutions.py` & `MKN_third_codes-0.3.1/MKN_third_codes/solutions.py`

 * *Files 20% similar despite different names*

```diff
@@ -138,32 +138,77 @@
             for i in range(len(self.U)):
                 self.main_z *= combinations(self.U[i].grabbing, sum(self.U[i].balls))
         return self.main_z
 
 class EttaTableCell():
     """
     Ячейка таблицы Етта, со значением и вероятностью
+
+    Args:
+        etta_value (int): значение СВ "Етта"
+        good_th (int): количество удачных исходов
+        bad_th (int): количество неудачных исходов
+        probability (float): вероятность
+
+    Methods:
+        reset_probability
     """
     def __init__(self, etta_value:int=0, good_th:int=1, bad_th:int=1, probability:float=None):
         self.etta_value = etta_value
         self.good_th = good_th
         self.bad_th = bad_th
         self.probability = probability
         if self.probability == None:
-            self.probability = good_th/(good_th+bad_th)
+            self.reset_probability()
+
+    def reset_probability(self):
+        self.probability = self.good_th/(self.good_th+self.bad_th)
 
 class EttaTable():
     """
     Таблица значений Етта
+
+    Args:
+        cells (): массив ячеек
     """
     def __init__(self, cells=None):
         self.cells = cells
         if self.cells == None:
             self.cells=[]
 
+class Meetiner():
+    """
+    Класс, использующийся для решения задач типа встречи двух целей
+
+    Args:
+        start_time (float): начальный момент, относительно нулевой координаты, когда может появиться участник
+        end_time (float): конечный момент, относительно нулевой координаты, когда может появиться участник
+        waitind_time (float): кол-во меры, в течении которой участник ждёт
+    
+    Methods:
+        calculate_square
+    """
+    def __init__(self, start_time:float=0, end_time:float='inf', waiting_time:float=1):
+        if start_time >= 0:
+            self.start_time = start_time
+        else:
+            self.start_time = 0
+        if end_time >= 0:
+            self.end_time = end_time
+        else:
+            self.end_time = float('inf')
+        if waiting_time >= 0:
+            self.waiting_time = waiting_time
+        else:
+            self.waiting_time = 1
+
+    def calculate_square(self, maxEnd:float, waiter_time):
+        return ((min(self.end_time, maxEnd) - self.start_time - waiter_time)**2)/2
+
+
 
 def combinations(k:float=0,n:float=0):
     """
     Функция, считающая число сочетаний из n по k
 
     Args:
         k (float): аргумент k - количество повторений
@@ -230,82 +275,91 @@
     txt = txt[:-3]
     txt += f"\nP(B) = {result[1]}"
     print(txt)
 
 def things_complexity_terminal():
     """
     Общее решение задачи о 'невнимательной секретарше' (сколько людей получат свои вещи)
-    WARNING: Очень неоптимизированное! Не рекоммендую пытаться решить для количества людей > 9
+    WARNING: Очень неоптимизированное! Не рекоммендую пытаться решить для количества людей > 11
     """
     humans = int(input("Введите количество человек: "))
     result = things_complexity_solution(humans)
     print("Таблица:")
     for cell in result.cells:
         print(f"E = {cell.etta_value}; P = {cell.probability} ({cell.good_th}/{cell.bad_th})")
 
 def things_complexity_solution(humans:int = 0):
     """
     Решение задачи о 'невнимательной секретарше' (сколько людей получат свои вещи)
-    WARNING: Очень неоптимизированное! Не рекоммендую пытаться решить для количества людей > 9
+    WARNING: Очень неоптимизированное! Не рекоммендую пытаться решить для количества людей > 11
 
     Args:
         humans (int): кол-во людей
 
     Returns:
         EttaTable: таблица ячеек таблицы
     """
-    tickets = [-1 for _ in range(humans)]
     #следующей строчкой находим количество всех перестановок
     allPerestan = math.factorial(humans)
 
-    def editCopy(array, k, value):
-        array[k] = value
-        return array
-
-    #Функция, позволяющая найти количество перестановок, удовлетворяющих условию:
-    #"n человек получили нужные вещи"
-    def findCountNumber(n, layer, tick, setting:set, i=0):
-        #выход из рекурсии, когда все вещи рапределены
-        if -1 not in tick:
-            #если нам осталось распределить 0 вещей правильно
-            if n == 0:
-                #перевод массива в хэшируемый вид
-                bigTick = 0
-                for el in range(0, len(tick)):
-                    bigTick += tick[el]*(humans**el)
-                #добавляем новую перестановку в set()
-                setting.add(bigTick)
-            return setting
-        start = min(tick)+1
-        #если предемт ещё не выдан
-        if tick[i] == -1:
-            copy = []
-            for el in tick:
-                copy.append(el)
-            #проходимся по всем вещам
-            for k in range(start, humans):
-                #если вещь ещё не выдана
-                if k not in tick:
-                    #если вещь принадлежит человку, которому сейчас выдаем
-                    if i == k:
-                        #проверяем, можем ли мы ему выдать (и выдаём, если да)
-                        if n > 0:
-                            #при этом в следующем шаге рекурсии уменьшаем n
-                            setting = findCountNumber(n-1, layer+1, editCopy(copy,i,k), setting, i+1)
-                    #иначе
-                    else:
-                        #в следующем шаге рекурсии n остаётся прежним
-                        setting = findCountNumber(n, layer+1, editCopy(copy,i,k), setting, i+1)
-        
-        return setting
-    
     myTable = EttaTable(cells=[])
 
     #для каждой "Этта" от 0 до humans вычисляем вероятность (Этта людей получили свои вещи)
     for j in range(0, humans+1):
-        cnt = findCountNumber(j, 0, tickets, set())
-        myTable.cells.append(EttaTableCell(j, len(cnt), allPerestan, len(cnt)/allPerestan))
+        myTable.cells.append(EttaTableCell(j, 0, allPerestan))
+
+    #Функция, проходящаяся по всем перестановкам, и записивыающая их в таблицу
+    def goThrough(n, layer, used):
+        if layer == humans:#раздали все предметы
+            myTable.cells[n].good_th += 1
+            return
+        for ticket in range(0, humans):#раздаем следующий предмет
+            if ticket not in used:#он ещё не использован
+                if ticket == layer:#если индекс редмета равен индексу человека, то повышаем n
+                    goThrough(n+1, layer+1, used+[ticket])
+                else:#иначе не трогаем
+                    goThrough(n, layer+1, used+[ticket])
+
+    goThrough(0, 0, [])
+
+    #пересчёт вероятностей
+    for j in range(0, humans+1):
+        myTable.cells[j].reset_probability()
     
     return myTable
 
+def geometric_meeting_terminal():
+    """
+    Общее решение задачи о встрече двух участников
+    """
+    ln = float(input("Введите отрезок меры: "))
+    fM = Meetiner(float(input("Введите начальный момент, когда может появиться участник первый (-1 для расширения на полный отрезок): ")), 
+    float(input("Введите конечный момент, когда может появиться участник первый (-1 для расширения на полный отрезок): ")), 
+    float(input("Введите, сколько времени будет ждать участник первый: ")))
+
+    sM = Meetiner(float(input("Введите начальный момент, когда может появиться участник второй (-1 для расширения на полный отрезок): ")), 
+    float(input("Введите конечный момент, когда может появиться участник второй (-1 для расширения на полный отрезок): ")), 
+    float(input("Введите, сколько времени будет ждать участник второй: ")))
+
+    print("Обозначим за A - участники встретятся")
+    print(f"P(A) = {geometric_meeting_solution(ln, fM, sM)}")
+
+def geometric_meeting_solution(length:float = 0, firstAim:Meetiner=None, secondAim:Meetiner=None):
+    """
+    Решение задачи о встрече двух участников
+
+    Args:
+        length (float): длина участка меры, на которой могут встретиться участники
+        firstAim (Meetiner): первый участник
+        secondAim (Meetiner): второй участник
+
+    Returns:
+        float: вероятность встречи первого и второго участника
+    """
+    square = ( length - max([firstAim.start_time, secondAim.start_time, 0]) - ( length - min([firstAim.end_time, secondAim.end_time, length]) ) )**2
+    square -= firstAim.calculate_square(length, secondAim.waiting_time)
+    square -= secondAim.calculate_square(length, firstAim.waiting_time)
+
+    return square/(length**2)
 
-__all__ = ['combinations', 'buckets_n_balls_solution', 'buckets_n_balls_terminal', 'things_complexity_terminal', 'things_complexity_solution']
+__all__ = ['combinations', 'buckets_n_balls_solution', 'buckets_n_balls_terminal', 'things_complexity_solution', 'things_complexity_terminal',
+'geometric_meeting_solution', 'geometric_meeting_terminal']
```

