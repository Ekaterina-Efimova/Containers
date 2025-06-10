# s21_containers.h library

You need to implement the `s21_containers.h` library classes (specifications are given in the relevant material sections, see **"Main containers"**). \
List of classes: `list`, `map`, `queue`, `set`, `stack`, `vector`.
You need to implement the `s21_containersplus.h` library functions (see **"Additional containers"** for specifications). \
List of classes to be implemented additionally: `array`, `multiset`.
You need to complete the classes with the appropriate methods, according to the table:

| Modifiers      | Definition                                      | Containers |
|----------------|-------------------------------------------------| -------------------------------------------|
| `iterator insert_many(const_iterator pos, Args&&... args)`          | Inserts new elements into the container directly before `pos`.  | List, Vector. |
| `void insert_many_back(Args&&... args)`          | Appends new elements to the end of the container.  | List, Vector, Queue. |
| `void insert_many_front(Args&&... args)`          | Appends new elements to the top of the container.  | List, Stack. |
| `vector<std::pair<iterator,bool>> insert_many(Args&&... args)`          | Inserts new elements into the container.  | Map, Set, Multiset. |
