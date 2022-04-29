# Дневник по научной работе
Спецсеминар А. Г. Дьяконова
## Оптимизация гиперпараметров
(тема была выбрана 29.11.21)

Планируется провести обзор существующих методов и программного обеспечения, их сравнение, провести сопутствующие эксперименты, возможно рассмотреть оптимизацию гиперпараметров в приложении к AutoML.

**29.11.21**

Для первоначального ознакомления с темой были выбраны следующие статьи и литература:

[https://www.automl.org/wp-content/uploads/2019/05/AutoML_Book_Chapter1.pdf](https://www.automl.org/wp-content/uploads/2019/05/AutoML_Book_Chapter1.pdf)

[https://proceedings.neurips.cc/paper/2012/file/05311655a15b75fab86956663e1819cd-Paper.pdf](https://proceedings.neurips.cc/paper/2012/file/05311655a15b75fab86956663e1819cd-Paper.pdf)

[https://arxiv.org/pdf/2111.00513.pdf](https://arxiv.org/pdf/2111.00513.pdf)

[https://proceedings.neurips.cc/paper/2011/file/86e8f7ab32cfd12577bc2619bc635690-Paper.pdf](https://proceedings.neurips.cc/paper/2011/file/86e8f7ab32cfd12577bc2619bc635690-Paper.pdf)

[https://arxiv.org/pdf/1502.02127.pdf](https://arxiv.org/pdf/1502.02127.pdf)

[https://jmlr.org/papers/volume13/bergstra12a/bergstra12a.pdf](https://jmlr.org/papers/volume13/bergstra12a/bergstra12a.pdf)

Нужно тщательнее изучить байесовскую оптимизацию и сопутствующую теорию, посмотреть другие источники.

**05.12.21**

Из пакетов было решено рассмотреть hyperopt, scikit-optimize, optuna, scikit-learn (стандартный GridSearch). Возможно в планах ознакомиться с H2O AutoML и bayesopt.

Первоначально планируется провести эксперименты для поиска по сетке, случайного поиска и байесовской оптимизации. Сравниваться будет итоговое качество лучшей модели, время работы, число итераций (+учет особенностей реализации?)

Нужно выбрать датасет и детально спланировать эксперименты, набор рассматриваемых моделей. Возможно попробовать различные типы данных (таблицы, текст).

**12.12.21**

Интересной показалась идея применения эволюционных алгоритмов, стоит почитать на эту тему

[https://www.researchgate.net/publication/301463804_Optimizing_deep_learning_hyper-parameters_through_an_evolutionary_algorithm](https://www.researchgate.net/publication/301463804_Optimizing_deep_learning_hyper-parameters_through_an_evolutionary_algorithm)

[https://arxiv.org/pdf/2011.04434.pdf](https://arxiv.org/pdf/2011.04434.pdf)

Также в планах почитать про AutoML

[https://www.automl.org/book/](https://www.automl.org/book/)

**13.12.21**

Узнал про Google Vizier, нужно будет ознакомиться

[https://storage.googleapis.com/pub-tools-public-publication-data/pdf/bcb15507f4b52991a0783013df4222240e942381.pdf](https://storage.googleapis.com/pub-tools-public-publication-data/pdf/bcb15507f4b52991a0783013df4222240e942381.pdf)

**22.12.21**

Доклад на спецсеминаре по статье "Generalized Anomaly Detection": [https://arxiv.org/pdf/2110.15108.pdf](https://arxiv.org/pdf/2110.15108.pdf)

[Слайды](https://github.com/ezzbreezn/research_seminar/blob/main/Reports/Generalized%20Anomaly%20Detection.pdf)

**29.04.22**

За прошедшее время также были изучены следующие статьи и ресурсы:

[https://www.cs.ubc.ca/~hutter/papers/ICML14-HyperparameterAssessment.pdf](https://www.cs.ubc.ca/~hutter/papers/ICML14-HyperparameterAssessment.pdf)

[https://ai.stanford.edu/~ronnyk/c45ap.pdf](https://ai.stanford.edu/~ronnyk/c45ap.pdf)

[https://docs.aws.amazon.com/sagemaker/latest/dg/automatic-model-tuning.html](https://docs.aws.amazon.com/sagemaker/latest/dg/automatic-model-tuning.html)

[https://pages.cs.wisc.edu/~gangluo/automatic_selection_review.pdf](https://pages.cs.wisc.edu/~gangluo/automatic_selection_review.pdf)

[https://proceedings.neurips.cc/paper/2015/file/11d0e6287202fced83f79975ec59a3a6-Paper.pdf](https://proceedings.neurips.cc/paper/2015/file/11d0e6287202fced83f79975ec59a3a6-Paper.pdf)

[https://pdfs.semanticscholar.org/9078/7a8ebbebcba951fa9ba6579f2f7e221e4522.pdf?_ga=2.155855547.1063695658.1647534095-1731775677.1647534095](https://pdfs.semanticscholar.org/9078/7a8ebbebcba951fa9ba6579f2f7e221e4522.pdf?_ga=2.155855547.1063695658.1647534095-1731775677.1647534095)

[https://docs.yandex.ru/docs/view?tm=1647535073&tld=ru&lang=en&name=bergstra13.pdf&text=making%20a%20science%20of%20model%20search%3A%20Hyperparameter%20optimization%20in%20hundreds%20of%20dimensions%20for%20vision%20architectures&url=https%3A%2F%2Fproceedings.mlr.press%2Fv28%2Fbergstra13.pdf&lr=213&mime=pdf&l10n=ru&sign=2602b5a066e9ceadede74acec97dde61&keyno=0&nosw=1&serpParams=tm%3D1647535073%26tld%3Dru%26lang%3Den%26name%3Dbergstra13.pdf%26text%3Dmaking%2Ba%2Bscience%2Bof%2Bmodel%2Bsearch%253A%2BHyperparameter%2Boptimization%2Bin%2Bhundreds%2Bof%2Bdimensions%2Bfor%2Bvision%2Barchitectures%26url%3Dhttps%253A%2F%2Fproceedings.mlr.press%2Fv28%2Fbergstra13.pdf%26lr%3D213%26mime%3Dpdf%26l10n%3Dru%26sign%3D2602b5a066e9ceadede74acec97dde61%26keyno%3D0%26nosw%3D1 ](https://docs.yandex.ru/docs/view?tm=1647535073&tld=ru&lang=en&name=bergstra13.pdf&text=making%20a%20science%20of%20model%20search%3A%20Hyperparameter%20optimization%20in%20hundreds%20of%20dimensions%20for%20vision%20architectures&url=https%3A%2F%2Fproceedings.mlr.press%2Fv28%2Fbergstra13.pdf&lr=213&mime=pdf&l10n=ru&sign=2602b5a066e9ceadede74acec97dde61&keyno=0&nosw=1&serpParams=tm%3D1647535073%26tld%3Dru%26lang%3Den%26name%3Dbergstra13.pdf%26text%3Dmaking%2Ba%2Bscience%2Bof%2Bmodel%2Bsearch%253A%2BHyperparameter%2Boptimization%2Bin%2Bhundreds%2Bof%2Bdimensions%2Bfor%2Bvision%2Barchitectures%26url%3Dhttps%253A%2F%2Fproceedings.mlr.press%2Fv28%2Fbergstra13.pdf%26lr%3D213%26mime%3Dpdf%26l10n%3Dru%26sign%3D2602b5a066e9ceadede74acec97dde61%26keyno%3D0%26nosw%3D1 )

[https://www.cs.ubc.ca/~hutter/papers/10-TR-SMAC.pdf](https://www.cs.ubc.ca/~hutter/papers/10-TR-SMAC.pdf)

[https://arxiv.org/pdf/1604.00772.pdf](https://arxiv.org/pdf/1604.00772.pdf)

[https://www.researchgate.net/profile/Yuhui-Shi/publication/220801072_Comparison_between_Genetic_Algorithms_and_Particle_Swarm_Optimization/links/54d9a96e0cf2970e4e7c55d1/Comparison-between-Genetic-Algorithms-and-Particle-Swarm-Optimization.pdf?_sg%5B0%5D=4A_BE-2BDj8U1OB0GBJci0R_04cN7yrujdESGo6awV81B2JafPdZsCN6gqjDf4FYORB0D8oJMP4C3OWLRWh4NA.sPAFuzkWNWFJAVTcIr3BntwrsA685D8dcBdvB6r_ercniIt8q4abOMluqjzcYmNoW0uJnMxVjCq7lomY5dt00Q&_sg%5B1%5D=mpu7Oz7jiM9D_eDD4CWib_vtMw86tZHzR8zADdSkbFif0Xjiz2NGwpwS66fMjptivUD81h2UWsne7bNeA44Rzewf1v0t7MjLebPqJHqFt0aD.sPAFuzkWNWFJAVTcIr3BntwrsA685D8dcBdvB6r_ercniIt8q4abOMluqjzcYmNoW0uJnMxVjCq7lomY5dt00Q&_iepl= ](https://www.researchgate.net/profile/Yuhui-Shi/publication/220801072_Comparison_between_Genetic_Algorithms_and_Particle_Swarm_Optimization/links/54d9a96e0cf2970e4e7c55d1/Comparison-between-Genetic-Algorithms-and-Particle-Swarm-Optimization.pdf?_sg%5B0%5D=4A_BE-2BDj8U1OB0GBJci0R_04cN7yrujdESGo6awV81B2JafPdZsCN6gqjDf4FYORB0D8oJMP4C3OWLRWh4NA.sPAFuzkWNWFJAVTcIr3BntwrsA685D8dcBdvB6r_ercniIt8q4abOMluqjzcYmNoW0uJnMxVjCq7lomY5dt00Q&_sg%5B1%5D=mpu7Oz7jiM9D_eDD4CWib_vtMw86tZHzR8zADdSkbFif0Xjiz2NGwpwS66fMjptivUD81h2UWsne7bNeA44Rzewf1v0t7MjLebPqJHqFt0aD.sPAFuzkWNWFJAVTcIr3BntwrsA685D8dcBdvB6r_ercniIt8q4abOMluqjzcYmNoW0uJnMxVjCq7lomY5dt00Q&_iepl= )

[https://www.researchgate.net/profile/Nikolaus-Hansen/publication/227050324_The_CMA_Evolution_Strategy_A_Comparing_Review/links/0deec522f45a9ce7c4000000/The-CMA-Evolution-Strategy-A-Comparing-Review.pdf?_sg%5B0%5D=m_h3w6CV9oWXO63HPUb4_4psRG5IJzFIqoPE5pdfLHNCZxQpsLjzUazdjjg5uLTNP0fsa6bUNzt9-xzAp_nEzQ.3kRcwpnTZudgJa049ekAAdmMEJtkB7TaF8Weehe2QtgJIaW9LNJtlatlad67aN_zbsM8-svKtCRSjjbB5ny0rQ&_sg%5B1%5D=EJ4S7aCY8R4yJftc-LEQx-CvxkFq17QvMvZmRcuHR9vNX88Pj5nAOkOWbz0JWdachIZP4jL6Aybg-R44ALY6FIwDZBX6qXVSns9es3vfZx49.3kRcwpnTZudgJa049ekAAdmMEJtkB7TaF8Weehe2QtgJIaW9LNJtlatlad67aN_zbsM8-svKtCRSjjbB5ny0rQ&_iepl=](https://www.researchgate.net/profile/Nikolaus-Hansen/publication/227050324_The_CMA_Evolution_Strategy_A_Comparing_Review/links/0deec522f45a9ce7c4000000/The-CMA-Evolution-Strategy-A-Comparing-Review.pdf?_sg%5B0%5D=m_h3w6CV9oWXO63HPUb4_4psRG5IJzFIqoPE5pdfLHNCZxQpsLjzUazdjjg5uLTNP0fsa6bUNzt9-xzAp_nEzQ.3kRcwpnTZudgJa049ekAAdmMEJtkB7TaF8Weehe2QtgJIaW9LNJtlatlad67aN_zbsM8-svKtCRSjjbB5ny0rQ&_sg%5B1%5D=EJ4S7aCY8R4yJftc-LEQx-CvxkFq17QvMvZmRcuHR9vNX88Pj5nAOkOWbz0JWdachIZP4jL6Aybg-R44ALY6FIwDZBX6qXVSns9es3vfZx49.3kRcwpnTZudgJa049ekAAdmMEJtkB7TaF8Weehe2QtgJIaW9LNJtlatlad67aN_zbsM8-svKtCRSjjbB5ny0rQ&_iepl=)

[https://conference.scipy.org/proceedings/scipy2013/pdfs/bergstra_hyperopt.pdf](https://conference.scipy.org/proceedings/scipy2013/pdfs/bergstra_hyperopt.pdf)

[http://laboratorios.fi.uba.ar/lsi/RCSJ-27-15-24.pdf](http://laboratorios.fi.uba.ar/lsi/RCSJ-27-15-24.pdf)

[https://www.cs.tufts.edu/comp/150GA/homeworks/hw3/_reading6%201995%20particle%20swarming.pdf](https://www.cs.tufts.edu/comp/150GA/homeworks/hw3/_reading6%201995%20particle%20swarming.pdf)

[https://arxiv.org/pdf/1907.10902.pdf](https://arxiv.org/pdf/1907.10902.pdf)

[https://www.researchgate.net/publication/332412530_Weighted_Random_Search_for_Hyperparameter_Optimization/fulltext/5cb3dc234585156cd79925e8/Weighted-Random-Search-for-Hyperparameter-Optimization.pdf?_sg%5B0%5D=jw3ovbq9JMwXGxUYAaRVzs2ZF-6K7hDkeGz9IN5hid3FvdHGj5R77XZ98y8i_miWvqkWxvfJ1bepdZmirJD5Kg.HIj4o02YP6JwGxsJrRtUmc7Uh2rcWCPjg46fZlRSpFmEUYEHN6Lkf4ohiyUgOh_u0D6lg1_Hm8sdjoakgu08vw&_sg%5B1%5D=PXUYJonUsgytXiGPz7L1yjsl1Bbn_xmb1fwWLx-OMDv7s064HS6uO7mM_uw29i7ikXWuGHrX-neqQmzqtHsd3Z9tWOORC8jT_uPC1kx9F8lw.HIj4o02YP6JwGxsJrRtUmc7Uh2rcWCPjg46fZlRSpFmEUYEHN6Lkf4ohiyUgOh_u0D6lg1_Hm8sdjoakgu08vw&_iepl= ](https://www.researchgate.net/publication/332412530_Weighted_Random_Search_for_Hyperparameter_Optimization/fulltext/5cb3dc234585156cd79925e8/Weighted-Random-Search-for-Hyperparameter-Optimization.pdf?_sg%5B0%5D=jw3ovbq9JMwXGxUYAaRVzs2ZF-6K7hDkeGz9IN5hid3FvdHGj5R77XZ98y8i_miWvqkWxvfJ1bepdZmirJD5Kg.HIj4o02YP6JwGxsJrRtUmc7Uh2rcWCPjg46fZlRSpFmEUYEHN6Lkf4ohiyUgOh_u0D6lg1_Hm8sdjoakgu08vw&_sg%5B1%5D=PXUYJonUsgytXiGPz7L1yjsl1Bbn_xmb1fwWLx-OMDv7s064HS6uO7mM_uw29i7ikXWuGHrX-neqQmzqtHsd3Z9tWOORC8jT_uPC1kx9F8lw.HIj4o02YP6JwGxsJrRtUmc7Uh2rcWCPjg46fZlRSpFmEUYEHN6Lkf4ohiyUgOh_u0D6lg1_Hm8sdjoakgu08vw&_iepl= )

В теоретической части работы рассматриваются следующие алгоритмы и темы:

- Общая постановка задачи, особенности, задание конфигурационного пространства
- Поиск по сетке значений гиперпараметров
- Случайный поиск и некоторые модификации
- CMA-ES
- TPE
- Генетический алгоритм
- Particle Swarm Optimization
- SMAC
- Байесовская оптимизация

Эксперименты проводятся на табличных данных (датасеты Breast Cancer Wisconsin и California Housing Prices) и изображениях (CIFAR-10, MNIST). Рассматриваются задачи классификации и регрессии. 

Оптимизируемые модели:

- SVM с RBF-ядром, оптимизируемые гиперпараметры: коэффициент регуляризации C и параметр ядра $\gamma$
- CatBoostClassifier и CatBoostRegresion, оптимизируемые гиперпараметры: число деревьев, темп обучения, максимальная глубина
- Сверточные сети, оптимизируемые гиперпараметры: число блоков свертки, размер ядра свертки, темп обучения

Применяемые алгоритмы оптимизации гиперпараметров:

- Поиск по сетке
- Случайный поиск
- TPE
- CMA-ES
- Байесовская оптимизация

Основной пакет - optuna и scikit optimize. На табличных данных рассматриваются SVM и градиентный бустинг, на изображениях - сверточные сети. Исследуются время работы, результирующее качество.
