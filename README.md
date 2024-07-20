# random
python
from collections import Counter # Импортируем библиотеку для подсчета, подсчет элементов Counter(randomizer_list)

randomizer_list = [] # Создаем пустой лист

for i in range(10000): # Пишем функцию, в дальнейшим будем ее проходить
    randomizer_list.append(random.choice(name_winners)) # Добавляем в наш рандомный лист с каждой итерацией случайное имя из списка победителей

for i in name_winners: # Выведем следующим циклом все имена и сколько раз они попадались
    print(f'Имя из списка: {i}, Количество выпаданий из 10000 раз: {Counter(randomizer_list)[i]}, Доля в выборке: {Counter(randomizer_list)[i]/10000*100}') # Итеруруем по Counter(randomizer_list)[i], где i обозначает имя из списка name_winners
