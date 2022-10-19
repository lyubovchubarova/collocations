# Проект по сравнению метрик извлечения коллокаций

## [Ссылка на папку с данными](https://drive.google.com/drive/folders/1uE5bhxzQpmNj8lFodAAtI1ZOdTDYwqhc?usp=sharing)

## [Спорные случаи для обсуждения](https://docs.google.com/document/d/1zb0CAif6QkNL_1BUSX-lOoSHiQuQA0j-84t5SdTF50c/edit)

## План работы

- [x] Подготовим корпус, из которого в дальнейшем будем извлекать коллокации: В качестве основы возьмем новостной подкорпус «Тайги»;
- [x] Освоим базовые навыки программирования на ЯП Python и поработаем с т.н. «регулярными выражениями»;
- [x] Разделим новостные тексты на предложения, удалим пунктуацию и приведем к нижнему регистру.
- [x] Выберем т.н. «node-word», для которого будем извлекать коллокации; ???
- [x] Выделим коллокации на основе поверхностной встречаемости (surface cooccurrence);
- [x] Для каждой гипотетической коллокации рассчитаем частотные характеристики (frequency signatures): O, f1, f2, N, а также значение ожидаемой частотности (expected frequency): E;
- [x] Для каждой гипотетической коллокации рассчитаем ее ассоциативные метрики (association measures): MI, MI , local-MI, z-score, t-score, simple-ll и др.; 
- [ ] Оценим приемлемость полученных коллокаций и проанализируем все статистические данные;
- [ ] Установим, какая из ассоциативных метрик наилучшим образом справилась с извлечением коллокаций.

## План занятий

| № | Тема                                                                            | Дата | Материалы |
|---|---------------------------------------------------------------------------------|------|-----------|
| 1 | Что такое коллокации? (Любовь)                                                                        | 13 октября | [Презентация](https://github.com/lyubovchubarova/collocations/blob/main/Presentations/1.%20%D0%9A%D0%BE%D0%BB%D0%BB%D0%BE%D0%BA%D0%B0%D1%86%D0%B8%D0%B8.pptx)    |
| 2 | Лексические функции + (Not) a deep dive into sketch engine (Любовь)                                                                    | 14 октября | [SketchEngine](https://www.sketchengine.eu/), [Глагольная сочетаемость имён](http://dict.ruslang.ru/abstr_noun.php), [Сочетания со значением высокой степени](http://dict.ruslang.ru/magn.php), [Презентация](https://github.com/lyubovchubarova/collocations/blob/main/Presentations/3.%20%D0%9A%D0%BE%D1%80%D0%BF%D1%83%D1%81%D0%B0%20%D0%B8%20%D0%BE%D0%BA%D0%BE%D0%BB%D0%BE%20%D1%82%D0%BE%D0%B3%D0%BE.pptx), [Про другие лексические функции](https://ruscorpora.ru/new/help-lexical-functions.html) |
| 3 | Совместная встречаемость и частотность. (Любовь)                                                                          | 14 октября | [Презентация](https://github.com/lyubovchubarova/collocations/blob/main/Presentations/2.%20%D0%A1%D0%BE%D0%B2%D0%BC%D0%B5%D1%81%D1%82%D0%BD%D0%B0%D1%8F%20%D0%B2%D1%81%D1%82%D1%80%D0%B5%D1%87%D0%B0%D0%B5%D0%BC%D0%BE%D1%81%D1%82%D1%8C%20%D0%B8%20%D1%87%D0%B0%D1%81%D1%82%D0%BE%D1%82%D0%BD%D0%BE%D1%81%D1%82%D1%8C.pptx)    |
| 4 |  Общий план работы + что может (Национальный) корпус (Дарья)                                                                        | 15 октября |  [Презентация](https://github.com/lyubovchubarova/collocations/blob/main/Presentations/%D0%9F%D0%BB%D0%B0%D0%BD%20%D1%80%D0%B0%D0%B1%D0%BE%D1%82%D1%8B%20%2B%20%D0%BA%D0%BE%D1%80%D0%BF%D1%83%D1%81.pdf)   | 
| 5 | Проектная работа: получение корпуса                                                                             | 15 октября | [Colab-конспект: Introduction to Python](https://colab.research.google.com/drive/14O5oBbM5MUNAoBpnanpTFRaoOs8vgnMw?usp=sharing)    |
| 6 | Проектная работа: получение корпуса                                                                             | 17 октября |  [Colab-база для работы](https://colab.research.google.com/drive/1kUuROM2s_RmUaYUhBhM9f0S83s5V0Rft#scrollTo=c-YhiMCjkwQ)   |
| 7 | Проектная работа: извлечение корпуса (Любовь)   + Меры ассоциации (эмпирические) Дарья                                                                        | 17 октября | [Конспект по метрикам](https://docs.google.com/document/d/1xpwSM2ppOa0MKlxlLhQ8xx82dcSCLdzBB0I-_6EDafk)    |
| 8 | Проектная работа: подсчет встречаемости                                                                       | 18 октября |  [Colab-тетрадка для работы](https://colab.research.google.com/drive/1PH-0O8CKCe1dZKOT8XLHetCZ__lvokTX?usp=sharing)   |
| 9 | Проектная работа: реализация эмпирических метрик                                                                           | 18 октября |     |
| 10 | Оценка работы метрик (Любовь)                                                                      | 19 октября |   [Презентация](https://github.com/lyubovchubarova/collocations/blob/main/Presentations/4.%20%D0%9E%D1%86%D0%B5%D0%BD%D0%BA%D0%B0%20%D0%BC%D0%BE%D0%B4%D0%B5%D0%BB%D0%B5%D0%B9%20%D0%B8%20%D0%BC%D0%B5%D1%82%D1%80%D0%B8%D0%BA.pptx)  |
| 11 | Проектная работа: разметка коллокаций                                                                            | 19 октября |     |
| 12 | Проектная работа: обсуждение спорных случаев, подсчет метрик                                                                          | 20 октября |     |
| 13 | Excel: визуализация + проектная работа                                                                             | 20 октября |     |
| 14 | Вывод метрик + статистические метрики?                                                                           | 22 октября |     |
| 15 | Проектная работа: разметка | 22 октября |
| 16 | Проектная работа: визуализация                                                                            | 23 октября |     |
| 17 | Байки из склепа: где в индустрии используются коллокации (Любовь + Дарья)                                                                    | 22 октября                                                                             | 23 октября |     |


