# Comparing `tmp/MKN_third_codes-0.1.4.tar.gz` & `tmp/MKN_third_codes-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\MKN_third_codes-0.1.4.tar", last modified: Sat Apr 29 10:32:03 2023, max compression
+gzip compressed data, was "dist\MKN_third_codes-0.2.0.tar", last modified: Sat Apr 29 10:57:34 2023, max compression
```

## Comparing `MKN_third_codes-0.1.4.tar` & `MKN_third_codes-0.2.0.tar`

### file list

```diff
@@ -1,11 +1,11 @@
-drwxrwxrwx   0        0        0        0 2023-04-29 10:32:03.414871 MKN_third_codes-0.1.4/
-drwxrwxrwx   0        0        0        0 2023-04-29 10:32:03.409884 MKN_third_codes-0.1.4/MKN_third_codes/
--rw-rw-rw-   0        0        0    10340 2023-04-29 10:29:34.000000 MKN_third_codes-0.1.4/MKN_third_codes/solutions.py
-drwxrwxrwx   0        0        0        0 2023-04-29 10:32:03.413874 MKN_third_codes-0.1.4/MKN_third_codes.egg-info/
--rw-rw-rw-   0        0        0      190 2023-04-29 10:32:03.000000 MKN_third_codes-0.1.4/MKN_third_codes.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      193 2023-04-29 10:32:03.000000 MKN_third_codes-0.1.4/MKN_third_codes.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-29 10:32:03.000000 MKN_third_codes-0.1.4/MKN_third_codes.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       16 2023-04-29 10:32:03.000000 MKN_third_codes-0.1.4/MKN_third_codes.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      190 2023-04-29 10:32:03.414871 MKN_third_codes-0.1.4/PKG-INFO
--rw-rw-rw-   0        0        0       42 2023-04-29 10:32:03.414871 MKN_third_codes-0.1.4/setup.cfg
--rw-rw-rw-   0        0        0      277 2023-04-29 10:28:53.000000 MKN_third_codes-0.1.4/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-29 10:57:34.281148 MKN_third_codes-0.2.0/
+drwxrwxrwx   0        0        0        0 2023-04-29 10:57:34.269179 MKN_third_codes-0.2.0/MKN_third_codes/
+-rw-rw-rw-   0        0        0    15157 2023-04-29 10:57:24.000000 MKN_third_codes-0.2.0/MKN_third_codes/solutions.py
+drwxrwxrwx   0        0        0        0 2023-04-29 10:57:34.280150 MKN_third_codes-0.2.0/MKN_third_codes.egg-info/
+-rw-rw-rw-   0        0        0      190 2023-04-29 10:57:34.000000 MKN_third_codes-0.2.0/MKN_third_codes.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      193 2023-04-29 10:57:34.000000 MKN_third_codes-0.2.0/MKN_third_codes.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-29 10:57:34.000000 MKN_third_codes-0.2.0/MKN_third_codes.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       16 2023-04-29 10:57:34.000000 MKN_third_codes-0.2.0/MKN_third_codes.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      190 2023-04-29 10:57:34.280150 MKN_third_codes-0.2.0/PKG-INFO
+-rw-rw-rw-   0        0        0       42 2023-04-29 10:57:34.281148 MKN_third_codes-0.2.0/setup.cfg
+-rw-rw-rw-   0        0        0      277 2023-04-29 10:55:48.000000 MKN_third_codes-0.2.0/setup.py
```

### Comparing `MKN_third_codes-0.1.4/MKN_third_codes/solutions.py` & `MKN_third_codes-0.2.0/MKN_third_codes/solutions.py`

 * *Files 20% similar despite different names*

```diff
@@ -32,15 +32,17 @@
         depend_probability (float): вероятность достать Б шар из урны с шарами self.balls
         hypo_text (str): строка формата 'H(id): nБ mЧ; P(H(id)) = p; P(A|H(id)) = p`'
         summary_text (str): строка, использующаяся для составления строки для уравнения суммы вероятностей гипотез
 
     Methods:
         None
     """
-    def __init__(self, balls=[0, 0], probability=0, id=0):
+    def __init__(self, balls=None, probability=0, id=0):
+        if balls == None:
+            balls = [0,0]
         self.balls = balls
         self.probability = probability
         self.depend_probability = balls[0]/sum(balls)
         self.id = id
         self.hypo_text = f"H{self.id}: {self.balls[0]} Б, {self.balls[1]} Ч; P(H{self.id}) = {self.probability}; P(A|H{self.id}) = {self.depend_probability}"
         self.summary_text = f"P(A|H{self.id})P(H{self.id})"
 
@@ -63,16 +65,20 @@
                                                         #содержат требуемое по условию количество шаров
         new_mnoz = []
         for i in range(0, len(mnoz)):
             if whites[i] == totalWhite:
                 new_mnoz.append(mnoz[i])
         return(new_mnoz)
     
-    def get_whites_n_blacks_from_boxes(self, wGrab=0, id=0, whites=[], mnoz=[], totalW=0):#посчитать для взятия "wGrab" белых шаров из
+    def get_whites_n_blacks_from_boxes(self, wGrab=0, id=0, whites=None, mnoz=None, totalW=0):#посчитать для взятия "wGrab" белых шаров из
                                                                             #оставшихся урн, включая урну с индексом "id"
+        if whites == None:
+            whites = []
+        if mnoz == None:
+            mnoz = []
         if id >= len(self.U):
             return self.check_correctly(mnoz, whites, totalW)
         
         grabbing = self.U[id].grabbing#сколько всего берём шаров из урны
 
         mx_kW = self.U[id].balls[0]#сколько всего Б шаров
         mx_kB = self.U[id].balls[1]#сколько всего Ч шаров
@@ -129,14 +135,36 @@
 
     def get_zn(self):#получить общий знаменатель для формулы вероятности гипотезы
         if self.main_z == 1:
             for i in range(len(self.U)):
                 self.main_z *= combinations(self.U[i].grabbing, sum(self.U[i].balls))
         return self.main_z
 
+class EttaTableCell():
+    """
+    Ячейка таблицы Етта, со значением и вероятностью
+    """
+    def __init__(self, etta_value:int=0, good_th:int=1, bad_th:int=1, probability:float=None):
+        self.etta_value = etta_value
+        self.good_th = good_th
+        self.bad_th = bad_th
+        self.probability = probability
+        if self.probability == None:
+            self.probability = good_th/(good_th+bad_th)
+
+class EttaTable():
+    """
+    Таблица значений Етта
+    """
+    def __init__(self, cells=None):
+        self.cells = cells
+        if self.cells == None:
+            self.cells=[]
+
+
 def combinations(k:float=0,n:float=0):
     """
     Функция, считающая число сочетаний из n по k
 
     Args:
         k (float): аргумент k - количество повторений
         n (float): аргумент n - всего элементов
@@ -199,7 +227,82 @@
         txt += hypo.summary_text + " + "
     
     print(f"Обозначим событие B - достать шар из {len(boxes)+1} урны")
     txt = txt[:-3]
     txt += f"\nP(B) = {result[1]}"
     print(txt)
 
+def things_complexity_terminal():
+    """
+    Общее решение задачи о 'невнимательной секретарше' (сколько людей получат свои вещи)
+    WARNING: Очень неоптимизированное! Не рекоммендую пытаться решить для количества людей > 9
+    """
+    humans = int(input("Введите количество человек: "))
+    result = things_complexity_solution(humans)
+    print("Таблица:")
+    for cell in result.cells:
+        print(f"E = {cell.etta_value}; P = {cell.probability} ({cell.good_th}/{cell.bad_th})")
+
+def things_complexity_solution(humans:int = 0):
+    """
+    Решение задачи о 'невнимательной секретарше' (сколько людей получат свои вещи)
+    WARNING: Очень неоптимизированное! Не рекоммендую пытаться решить для количества людей > 9
+
+    Args:
+        humans (int): кол-во людей
+
+    Returns:
+        EttaTable: таблица ячеек таблицы
+    """
+    tickets = [-1 for _ in range(humans)]
+    #следующей строчкой находим количество всех перестановок
+    allPerestan = math.factorial(humans)
+
+    def editCopy(array, k, value):
+        array[k] = value
+        return array
+
+    #Функция, позволяющая найти количество перестановок, удовлетворяющих условию:
+    #"n человек получили нужные вещи"
+    def findCountNumber(n, layer, tick, setting:set, i=0):
+        #выход из рекурсии, когда все вещи рапределены
+        if -1 not in tick:
+            #если нам осталось распределить 0 вещей правильно
+            if n == 0:
+                #перевод массива в хэшируемый вид
+                bigTick = 0
+                for el in range(0, len(tick)):
+                    bigTick += tick[el]*(humans**el)
+                #добавляем новую перестановку в set()
+                setting.add(bigTick)
+            return setting
+        start = min(tick)+1
+        #если предемт ещё не выдан
+        if tick[i] == -1:
+            copy = []
+            for el in tick:
+                copy.append(el)
+            #проходимся по всем вещам
+            for k in range(start, humans):
+                #если вещь ещё не выдана
+                if k not in tick:
+                    #если вещь принадлежит человку, которому сейчас выдаем
+                    if i == k:
+                        #проверяем, можем ли мы ему выдать (и выдаём, если да)
+                        if n > 0:
+                            #при этом в следующем шаге рекурсии уменьшаем n
+                            setting = findCountNumber(n-1, layer+1, editCopy(copy,i,k), setting, i+1)
+                    #иначе
+                    else:
+                        #в следующем шаге рекурсии n остаётся прежним
+                        setting = findCountNumber(n, layer+1, editCopy(copy,i,k), setting, i+1)
+        
+        return setting
+    
+    myTable = EttaTable(cells=[])
+
+    #для каждой "Этта" от 0 до humans вычисляем вероятность (Этта людей получили свои вещи)
+    for j in range(0, humans+1):
+        cnt = findCountNumber(j, 0, tickets, set())
+        myTable.cells.append(EttaTableCell(j, len(cnt), allPerestan, len(cnt)/allPerestan))
+    
+    return myTable
```

