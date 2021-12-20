# Дневник по научной работе
Спецсеминар А. Г. Дьяконова
## Оптимизация гиперпараметров
Планируется провести обзор существующих методов и программного обеспечения, их сравнение, провести сопутствующие эксперименты, возможно рассмотреть оптимизацию гиперпараметров в приложении к AutoML.

Для первоначального ознакомления с темой были выбраны следующие статьи и литература:

[https://www.automl.org/wp-content/uploads/2019/05/AutoML_Book_Chapter1.pdf](https://www.automl.org/wp-content/uploads/2019/05/AutoML_Book_Chapter1.pdf)

[https://proceedings.neurips.cc/paper/2012/file/05311655a15b75fab86956663e1819cd-Paper.pdf](https://proceedings.neurips.cc/paper/2012/file/05311655a15b75fab86956663e1819cd-Paper.pdf)

[https://arxiv.org/pdf/2111.00513.pdf](https://arxiv.org/pdf/2111.00513.pdf)

[https://proceedings.neurips.cc/paper/2011/file/86e8f7ab32cfd12577bc2619bc635690-Paper.pdf](https://proceedings.neurips.cc/paper/2011/file/86e8f7ab32cfd12577bc2619bc635690-Paper.pdf)

[https://arxiv.org/pdf/1502.02127.pdf](https://arxiv.org/pdf/1502.02127.pdf)

[https://jmlr.org/papers/volume13/bergstra12a/bergstra12a.pdf](https://jmlr.org/papers/volume13/bergstra12a/bergstra12a.pdf)

Нужно тщательнее изучить байесовскую оптимизацию и сопутствующую теорию, посмотреть другие источники.

Из пакетов было решено рассмотреть hyperopt, scikit-optimize, optuna, scikit-learn (стандартный GridSearch). Возможно в планах ознакомиться с H2O AutoML и bayesopt.

Первоначально планируется провести эксперименты для поиска по сетке, случайного поиска и байесовской оптимизации. Сравниваться будет итоговое качество лучшей модели, время работы, число итераций (+учет особенностей реализации?)

Нужно выбрать датасет и детально спланировать эксперименты, набор рассматриваемых моделей. Возможно попробовать различные типы данных (таблицы, текст).

Интересной показалась идея применения эволюционных алгоритмов, стоит почитать на эту тему

[https://www.researchgate.net/publication/301463804_Optimizing_deep_learning_hyper-parameters_through_an_evolutionary_algorithm](https://www.researchgate.net/publication/301463804_Optimizing_deep_learning_hyper-parameters_through_an_evolutionary_algorithm)

[https://arxiv.org/pdf/2011.04434.pdf](https://arxiv.org/pdf/2011.04434.pdf)

Также в планах почитать про AutoML

[https://www.automl.org/book/](https://www.automl.org/book/)

Узнал про Google Vizier, нужно будет ознакомиться

[https://storage.googleapis.com/pub-tools-public-publication-data/pdf/bcb15507f4b52991a0783013df4222240e942381.pdf](https://storage.googleapis.com/pub-tools-public-publication-data/pdf/bcb15507f4b52991a0783013df4222240e942381.pdf)
