# Идея
построение и автоматическое обновления узкоспециализированного графа знаний на основе выбранных пользователем темы (с использованием логических правил?). 

# Описание идеи 
автоматически находить готовую онтологию (или брать какую-то часть из уже имеющейся?) для сравнительно небольшого графа знаний на тему выбранную пользователем, на основей который бы генерировался сам граф знаний. 

Предполагаемые плюсы: 1) высокая точность извлекаемых знаний (за счет логических правил, применимых на небольших графах знаний), 2) граф должен содержать узкоспециализированные знания строго по заданной пользователем темы

Предполагаемые минусы: 1) граф будет небольшой, 2) онтологию/правила строить сложно


# Предполагаемые задачи и их оценка сложности выполнения
1. Создание правил/отнологии по заданной пользоваетелем темы (вероятно, самая сложная часть, не знаю, есть ли готовые библиотеки)
2. Парсинг соответствующих веб-страниц википедии для выделения текстов по заданной теме (простая задача, готовые библиотеки есть)
3. Работа с референциональными тождествами - видимо, приведение их к одному обозначению. Пример: "Солнце встало, оно ярко светит" -> "Солнце встало, солнце ярко светит" (средней сложности задача, готовые библиотеки есть)
4. Выделение узлов из текста (средней сложности задача, готовые библиотеки есть)
5. Связывание узла с узлом из открытых графов знаний - DBpedia и тд (вероятно, сложная задача, не знаю, есть ли готовые библиотеки)
6. Создание ребер/отношений (средней сложности задача, готовые библиотеки есть)
