# Что это вообще такое 

В первую очередь сборник проектов, которые я выполнил или над которыми я ещё только работаю. Думаю, это будет полезно людям, которые хотят посмотреть на чужие блокноты. Чем эти блокноты примечательны? Ну, для начала, они написаны на русском языке. Проблемы с чтением английского текста мало у кого возникают, но всё же родной язык душе милее. Во-вторых, я стараюсь показывать как можно больше рассуждений, которые привели меня к тому, к чему привели и описать как можно больше грабель, что имели честь приложиться к моей роже. Блокноты на kaggle, по моим наблюдениям, часто (в плане ценности как материал для самообучения) страдают от отстутсвия дополнительных объяснений на тему того, почему что-то сделано так, как сделано, почему автор делает именно так, какая последовательность рассуждений, проб и ошибок к этому привела и что, по мнению автора, можно сделать, чтоб его результат улучшить. 

# Зачем это

1. Поделиться своим опытом с товарищами по цеху
2. Предъявить репозиторий работодателю с словами "вот примерно это я умею, примерно так я рассуждаю, можете сравнить с тем, как я рассуждал раньше, чтоб убедиться, что я не стагнирую"
3. Возвращаться к проектам, выполненным много лет назад и испытывать стыд 
4. Лет через 30 показать подрастающему поколению и пустить скупую мужскую слезу
5. Как оказалось, здесь, помимо всего прочего, могут появляться курсачи, что вполне может оказаться кому-то полезным

# Структура репозитория 

Одна папка - один проект. Пректы указаны снизу. Про каждый проект указана базовая информация, дабы если Вы здесь для того, чтобы посмотреть на блокноты, что относятся к задачам определённого типа, Вам их было легче найти. Базовая информация включает в себя:
1. Устройство данных (таблица, текст, аудио и т.д)
2. Тип задачи (классификация, регрессия, ранжирование и т.д)
3. Подход к решению (классические/нейросетевые методы или комбинированный подход) 
4. Основные использованные в проекте библиотеки
5. Краткое описание непосредственно данных

Более подробная информация о каждом из проектов в `readme` соответствующей папки. Если явно не оговорено обратное, используется Python. Список снизу приведён в порядке, обратном к хронологическому, т.е чем ниже в файле упомянут проект, тем более давно я им занимался. 

# Очень важно
Все рассуждения в присутствующих тут блокнотах на правильность ни в коем случае не претендуют. Использовать эти блокноты с целью научиться несредственно машинному обучению я бы не рекомендовал. Единственное, чему отсюда можно именно научиться - это избегать грабель, что сжигают и нервы, и кучу времени, и шутку сами знаете про кого сами знаете в какой период истории додумайте сами. 

В readme к каждому проекту есть часть "Грабли" и "Чему я научился и что вынес в процессе работы". Это в некоторым смысле одно и то же. Разница в том, что часть с граблями содержит объективные трудности и нюансы - как правильно, подводные камни работы с теми или иными библиотеками

# SP

1. Устройство данных: таблица, преобразованная в граф
2. Тип задачи: рекомендательная система
3. Подход к решению: формально нейросетевой, т.к использовался node2vec и, как следствие, skip-gram, но никакие сети ручками не строились 
4. Основные использованные библиотеки: pandas, node2vec
5. Краткое описание данных: [таблица](https://www.kaggle.com/datasets/andrewmvd/spotify-playlists) с информацией о том, кто что слушал. Вообще, это курсач на тему "построение рекомендательной системы с использованием векторного представления графа знаний". Признавать построенный граф графом знаний преподаватель отказался, однако курсач был принят. Авось кому-нибудь пригодится 

# KMR
1. Устройство данных: текст
2. Тип задачи: классификация (на 3 класса)
3. Подход к решению: нейросетевой
4. Основные использованные библиотеки: numpy, tensorflow. Немножечко gensim
5. Краткое описание данных: краней [интересный датасет](https://www.kaggle.com/datasets/mikhailklemin/kinopoisks-movies-reviews) с отзывами на фильмы из кинопоиска. Все отзывы делятся на положительные, нейтральные и негативные. Что с этим нужно сделать, думаю, догадаться не шибко сложно

# TPS
1. Устройство данных: таблица
2. Тип задачи: классификация (на 10 классов)
3. Подход к решению: классический 
4. Основные использованные библиотеки: numpy, pandas, scikit-learn
5. Краткое описание данных: [Tabular Playground Series - Feb 2022](https://www.kaggle.com/c/tabular-playground-series-feb-2022). Задача классификации бактерий. Подробное описание данных в [этой статье](https://www.frontiersin.org/articles/10.3389/fmicb.2020.00257/full). Описание менее подробное, но достаточное для понимания сути непосредственно в блокноте 

# НР
1. Устройство данных: таблица
2. Тип задачи: регрессия
3. Подход к решению: классический
4. Основные использованные библиотеки: numpy, pandas, scikit-learn
5. Краткое описание данных: классический датасет [House Prices](https://www.kaggle.com/c/house-prices-advanced-regression-techniques). Дома описаны рядом признаков, требуется построить модель, предсказывающую цену. Описание признаков можно найти по ссылке выше или непосредственно в блокноте. В последнем признаки описываются по мере их рассмотрения 