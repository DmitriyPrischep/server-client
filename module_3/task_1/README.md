### Задание 3.1
# Представление графа
 
Дан базовый интерфейс для представленияориентированного графа:
```C++
virtual ~IGraph() {}
	// Добавление ребра от from к to.
    virtual void AddEdge(int from, int to) = 0;
    virtual int VerticesCount() const  = 0;
    virtual void GetNextVertices(int vertex, std::vector<int>& vertices) const = 0;
    virtual void GetPrevVertices(int vertex, std::vector<int>& vertices) const = 0;
};
```

Необходимо написать несколько реализаций интерфейса:
- CListGraph, хранящий граф в виде массива списков смежности,
- CMatrixGraph, хранящий граф в виде матрицы смежности,
- CSetGraph, хранящий граф в виде массива хэш-таблиц,
- CArcGraph, хранящий граф в виде одного массива пар {from, to}.  

Также необходимо реализовать конструктор, принимающий const IGraph*. Такой конструктор должен скопировать переданный граф в создаваемый объект.
Для каждого класса создавайте отдельные h и cpp файлы.
Число вершин графа задается в конструкторе каждой реализации.