Анализ предвыборных статей кандидатов
=====================================

В этом каталоге лежат агитационные материалы кандидатов, которые они поместили в свои профили на сайте ЦВК, в пригодном для автоматического анализа виде (по возможности очищенные от видео, фотографий, Википедии и прочего мусора).

А именно:
+ candidates.txt — соответствие GUID → имя автора (гуиды любезно предоставлены сайтом ЦВК);
+ articles.txt — урлы статей для каждого гуида;
+ candidate_articles.zip/GUID_NUM.html — исходные HTML'ки статей (номера соответствуют порядку строк в articles.txt);
+ candidate_articles.zip/GUID_NUM.txt — выдранный HTML-сегментатором текст статьи, очищенный от тегов. Если сегментатор не нашёл, где в HTML находится основное содержимое, то файл будет пустым.
+ candidate_articles.zip/GUID_NUM.lemmas — токенизированный и лемматизированный текст. Формат каждой строки: <лемма> \t <граммемы леммы>. Граммемы разделяются запятой, часть речи идёт в самом начале. Над текстами было проведено снятие омонимии: если возможных лемм несколько, то выбирается не первая попавшаяся, а наиболее вероятная в данном контексте.
