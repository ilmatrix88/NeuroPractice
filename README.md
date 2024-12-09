# NeuroPractice
Решение двух практических задач по нейросетям и выполнение полноценной практической работы, включая ТЗ и оценку проекта

Задача 1. Обнаружение фальшивых новостей
Фальшивые новости — это ложная информация, распространяемая через социальные сети и другие сетевые СМИ для достижения политических или идеологических целей.

Твоя  задача -  используя библиотеку sklearn построить модель классического машинного обучения, которая может с высокой точностью более 90% определять, является ли новость реальной (REAL） или фальшивой（FAKE).

Ты должен самостоятельно изучить и применить к задаче TfidfVectorizer для извлечения признаков из текстовых данных и PassiveAggressiveClassifier.

Ты  можешь использовать данный датасет для обучения.

Построй матрицу ошибок (confusion matrix). Представь, что ваш заказчик очень любит графики и диаграммы. Визуализируй для него результаты там, где это возможно.

Что такое TfidfVectorizer?
Изучение текстовых данных является одной из фундаментальных задач в области анализа данных и машинного обучения.

Однако тексты представляют собой сложные и многомерные структуры, которые не могут быть напрямую обработаны алгоритмами машинного обучения. В этом контексте извлечение признаков — это процесс преобразования текстовых данных в числовые векторы, которые могут быть использованы для обучения моделей и анализа. Этот шаг играет ключевую роль в предварительной обработке данных перед применением алгоритмов.

Term Frequency-Inverse Document Frequency (TF-IDF) — это один из наиболее распространенных и мощных методов для извлечения признаков из текстовых данных. TF-IDF вычисляет важность каждого слова в документе относительно количества его употреблений в данном документе и во всей коллекции текстов. Этот метод позволяет выделить ключевые слова и понять, какие слова имеют больший вес для определенного документа в контексте всей коллекции.

TfidfVectorizer преобразует коллекцию необработанных документов в матрицу объектов TF-IDF.

Что такое пассивно-агрессивный классификатор (PassiveAggressiveClassifier)?
Пассивно-агрессивный классификатор – это алгоритм онлайн-обучения, в котором вы обучаете систему постепенно, загружая ее экземпляры последовательно, отдельно или небольшими группами, называемыми мини-партиями.

При онлайн-обучении модель машинного обучения обучается и развертывается в производственной среде таким образом, чтобы обучение продолжалось по мере поступления новых наборов данных. Таким образом, мы можем сказать, что такой алгоритм, как пассивно-агрессивный классификатор, лучше всего подходит для систем, которые получают данные в непрерывном потоке. Он пассивно реагирует на правильные классификации и агрессивно реагирует на любые просчеты.

Задача 2. Обнаружение болезни паркинсона с помощью XGBoost
Твоя задача с помощью Data Science предсказать заболевание паркинсона на ранней стадии, используя алгоритм машинного обучения XGBoost и библиотеку sklearn для нормализации признаков. Как это сделать? Тебя  придется самостоятельно изучить данный вопрос.

Используй следующий датасет UCI ML Parkinsons. Описание признаков и меток датасета представлены здесь. От тебя  требуется помимо создания самой модели получить ее точность на тестовой выборке. Выборки делить в соотношении 80% обучающая, 20% - тестовая.

Дополнительные баллы ты получишь, если сможешь получить точность более 95%.

Что такое болезнь Паркинсона?
Болезнь Паркинсона - прогрессирующее заболевание центральной нервной системы, влияющее на движение и вызывающее тремор и скованность движений.

У нее 5 стадий, и ежегодно ею страдают более 1 миллиона человек только в одной Индии. Это хроническое заболевание, и его пока не лечат. Это нейродегенеративное расстройство, поражающее нейроны головного мозга, вырабатывающие дофамин.

Что такое XGBoost?
XGBoost - это новый алгоритм машинного обучения, разработанный с учетом скорости и производительности.

XGBoost расшифровывается как экстремальное повышение градиента и основан на деревьях решений.

Многие считают его одним из лучших алгоритмов и из-за его высокой производительности при решении задач регрессии и классификации, рекомендуют его в качестве первого выбора во многих ситуациях. XGBoost прославился тем, что выиграл множество соревнований Kaggle

Есть 2 распространенных способа использования XGBoost:

Learning API: это базовый низкоуровневый способ использования XGBoost. Простой и мощный, он включает встроенный метод перекрестной проверки.
Scikit-Learn API: это интерфейс-оболочка Scikit-Learn для XGBoost. Он позволяет использовать XGBoost совместимым с scikit-learn способом, точно так же, как вы использовали бы любую нативную модель scikit-learn.
В этом задании мы рекомендуем использовать XGBClassifier из библиотеки xgboost, который является реализацией scikit-learn API для классификации XGBoost.
