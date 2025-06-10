# Реализация библиотеки s21_containers.h
Необходимо реализовать классы библиотеки `s21_containers.h` (спецификации указаны в соответствующих разделах материалов, см. пункт **«Основные контейнеры»**). \
Список классов: `list` (список), `map` (словарь), `queue` (очередь), `set` (множество), `stack` (стек), `vector` (вектор).
Тебе необходимо реализовать функции библиотеки `s21_containersplus.h`
Список классов, которые нужно реализовать дополнительно: `array` (массив), `multiset` (мультимножество).
- Оформи решение в виде заголовочного файла `s21_containersplus.h`, который включает в себя другие заголовочные файлы с реализациями необходимых контейнеров (`s21_array.h`, `s21_multiset.h`);
- Предусмотри Makefile для тестов написанной библиотеки (с целями clean, test);
- За основу лучше всего взять классическую реализацию контейнеров, но конечный выбор алгоритма остается свободным.
Дополнены классы соответствующими методами согласно таблице:

| Modifiers      | Definition                                      | Containers |
|----------------|-------------------------------------------------| -------------------------------------------|
| `iterator insert_many(const_iterator pos, Args&&... args)`          | Inserts new elements into the container directly before `pos`.  | List, Vector. |
| `void insert_many_back(Args&&... args)`          | Appends new elements to the end of the container.  | List, Vector, Queue. |
| `void insert_many_front(Args&&... args)`          | Appends new elements to the top of the container.  | List, Stack. |
| `vector<std::pair<iterator,bool>> insert_many(Args&&... args)`          | Inserts new elements into the container.  | Map, Set, Multiset. |
