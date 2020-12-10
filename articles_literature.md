**Meta-learning**

1. **UCI++: Improved Support for Algorithm Selection Using Datasetoids**
  - datasetoids - zbiór jest transformowany poprzez zamianę kolejno każdej zmiennej kategorycznej ze zmienną celu, potencjalne problemy: braki, skośność, rozproszenie, brak lub pełna zależność z pozostałymi predyktorami w zmiennej, która staje się targetem,
  - cel meta-modelu - decision trees pruning
2. **[[link](https://www-1sciencedirect-1com-10000981v0742.eczyt.bg.pw.edu.pl/science/article/pii/S0031320312004281?via%3Dihub)]Learner excellence biased by data set selection: A case for data characterisation and artificial data sets**
  - teza: porównania algorytmów są zaburzone wyborem testowych zbiorów
  - analiza wykorzystywanych w benchmarkach zbiorów
  - nacisk na &quot;complexity-measures&quot;, które opisują np. separowalność klas
  - zbudowanie meta-modelu na powyższych meta-features, który wskazał klasy zbiorów gdzie konkretne algorytmy są lepsze od pozostałych
  - propozycja metody budowania puli sztucznych zbiorów do benchmarków
3. **[[link](http://citeseerx.ist.psu.edu/viewdoc/download?doi=10.1.1.401.5995&amp;rep=rep1&amp;type=pdf)]Dataset generation for meta-learning**
  - gotowy generator syntetycznych danych
  - zalety: produkuje zbiory o konkretnych parametrach (np. średnia skośność)
  - wady: nie wprowadza zmiennych istotnych-nieistotnych, zaczyna z losowo wygenerowanych zmiennych i dąży to osiągnięcia parametrów
4. [[link](https://link.springer.com/content/pdf/10.1007/s10994-012-5286-7.pdf)] **Meta-learning for evolutionary parameter optimization of classifiers**
  - główny temat to otymalizacja parametrów przez genetic algorithms wspate meta-features, ale wartościowa referencja do generowania sztucznych zbiorów
5. **[[link](https://www.sciencedirect.com/science/article/abs/pii/S0167865511001103?via%3Dihub)]A Bayes-true data generator for evaluation of supervised and unsupervised learning methods**
  - nowa metoda do generowania sztucznych zbiorów w celu ewaluacji algorytmów ML
  - zmienne kontrolowane bezpośrednio:
    1. number of classes
    2. number of intrinsic dimensions
    3. number of samples
    4. Bayes error between the class densities
  - zmienne kontrolowane post-process:
    1. centroid
    2. external dimensionality
    3. dataset covariance
  - prawdopodobnie wciąż utrzymywany software dostępny [tutaj](https://madm.dfki.de/downloads)
