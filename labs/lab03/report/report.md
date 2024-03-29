﻿**РОССИЙСКИЙ УНИВЕРСИТЕТ ДРУЖБЫ НАРОДОВ** 

**Факультет физико-математических и естественных наук Кафедра прикладной информатики и теории вероятностей** 

**ОТЧЕТ**  

**ПО ЛАБОРАТОРНОЙ РАБОТЕ № 3** 

*дисциплина:  Архитектура компьютера ![](Aspose.Words.d2a681ce-25a4-4145-a655-a9b5316407c1.001.png)*

Студент: Алади Принц Чисом                                    

Группа:Нкабд-05-22                                

**МОСКВА** 2022г. 

**Содержание** 

1. Цель работы                                                                       
2. Настройка github                                                                  

2. Базовая настройка git                                                            
3. Создание SSH ключа                                                               
3. Создание рабочего пространства и репозитория курса на основе шаблона              
1. Сознание репозитория курса на основе шаблон    
2. Настройка каталога курса    
3. Задание для самостоятельной работы  
4  Выводы     

1  Цель работы: 

Целью  работы  является  изучить  идеологию  и  применение  средств  контроля версий. Приобрести практические навыки по работе с системой git. 

2. Задание 
1. Описание: Настройка github 

![](Aspose.Words.d2a681ce-25a4-4145-a655-a9b5316407c1.003.jpeg)

(Рис. 1)Создал учетную запись github для выполнения лабораторных работ. ![](Aspose.Words.d2a681ce-25a4-4145-a655-a9b5316407c1.002.png)

2. Описание: Базовая настройка git 

![](Aspose.Words.d2a681ce-25a4-4145-a655-a9b5316407c1.004.jpeg)

(Рис. 2) Я открыл терминал  и ввел следующие команды выше, указав имя и адрес электронной почты для репозитория. 

После этого настроил utf-8 в его выводе, название начальной ветви по умолчанию и вызвал ее (master), также определил параметры autocrlf и safecrlf. ![](Aspose.Words.d2a681ce-25a4-4145-a655-a9b5316407c1.002.png)

3. Описание: Создание SSh ключа 

![](Aspose.Words.d2a681ce-25a4-4145-a655-a9b5316407c1.005.jpeg)

(Рис. 3)  Для последующей идентификации пользователя на сервере репозитория я сгенерировал пару ключей (закрытый и открытый). ![](Aspose.Words.d2a681ce-25a4-4145-a655-a9b5316407c1.002.png)

![](Aspose.Words.d2a681ce-25a4-4145-a655-a9b5316407c1.006.jpeg)

(Рис. 4) Используя команду cat, я скопировал ключ в буфер обмена ![](Aspose.Words.d2a681ce-25a4-4145-a655-a9b5316407c1.002.png)

![](Aspose.Words.d2a681ce-25a4-4145-a655-a9b5316407c1.007.jpeg)

(Рис. 5) Я зашел на сайт github, под своей учетной записью и перешел в меню настроек. После этого я выбрал ключи SSH и GPG. 

` `![](Aspose.Words.d2a681ce-25a4-4145-a655-a9b5316407c1.008.jpeg)![](Aspose.Words.d2a681ce-25a4-4145-a655-a9b5316407c1.009.jpeg)

(Рис. 6) Я выбрал ключи SSH и GPG в боковом меню и нажал кнопку new SSH key, скопировав ключ из локальной консоли в буфер обмена. ![](Aspose.Words.d2a681ce-25a4-4145-a655-a9b5316407c1.002.png)

3. Описание: Создание рабочего пространства и репозитория курса на основе шаблона 

![](Aspose.Words.d2a681ce-25a4-4145-a655-a9b5316407c1.010.jpeg)

(Рис.  7)  Я открыл  терминал  и  создал  структуру  каталогов  для  предмета  "Я  открыл терминал и создал структуру каталогов для предмета "Архитектура Компьютера”. 

1. Сознание репозитория курса на основе шаблона 

![](Aspose.Words.d2a681ce-25a4-4145-a655-a9b5316407c1.011.jpeg)

(Рис. 8) На github я создал репозиторий с именем study\_2022-2023\_arch-pc.git ![](Aspose.Words.d2a681ce-25a4-4145-a655-a9b5316407c1.002.png)

![](Aspose.Words.d2a681ce-25a4-4145-a655-a9b5316407c1.012.jpeg)

(Рис. 9) Перешел в ранее созданный каталог и клонировал туда только что созданный репозиторий с помощью команды git clone –recursive “link”. Ссылку взял на github. 

![](Aspose.Words.d2a681ce-25a4-4145-a655-a9b5316407c1.013.jpeg)

(Рис. 10) Клонирование репозитория ![](Aspose.Words.d2a681ce-25a4-4145-a655-a9b5316407c1.002.png)

2. Настройка каталога курса

![](Aspose.Words.d2a681ce-25a4-4145-a655-a9b5316407c1.014.jpeg)

![](Aspose.Words.d2a681ce-25a4-4145-a655-a9b5316407c1.015.jpeg)

(Рис. 11) Перейдите в каталог курса:  

cd ~/work/study/2022-2023/"Архитектура компьютера"/arch-pc  Удалите лишние файлы: 

rm package.json 

Создайте необходимые каталоги:  

echo arch-pc > COURSE  

make  

Отправьте файлы на сервер:  

git add . git commit -am 'feat(main): make course structure'  

git push ![](Aspose.Words.d2a681ce-25a4-4145-a655-a9b5316407c1.002.png)

![](Aspose.Words.d2a681ce-25a4-4145-a655-a9b5316407c1.016.jpeg)

(Рис. 12)Я проверил иерархию рабочей области в локальном репозитории, и на странице github все работало правильно. ![](Aspose.Words.d2a681ce-25a4-4145-a655-a9b5316407c1.002.png)

3. 3 Задание для самостоятельной работы 

![](Aspose.Words.d2a681ce-25a4-4145-a655-a9b5316407c1.017.jpeg)

(Рис. 13)На фотографии выше показан репозиторий на github с разделами лабораторных работ (11 папок с лабораторными работами) ![](Aspose.Words.d2a681ce-25a4-4145-a655-a9b5316407c1.002.png)

![](Aspose.Words.d2a681ce-25a4-4145-a655-a9b5316407c1.018.jpeg)

(Рис. 14) Загрузил отчеты lab1 и lab2 на GitHub с помощью midnight commander. ![](Aspose.Words.d2a681ce-25a4-4145-a655-a9b5316407c1.002.png)

![](Aspose.Words.d2a681ce-25a4-4145-a655-a9b5316407c1.019.jpeg)

![](Aspose.Words.d2a681ce-25a4-4145-a655-a9b5316407c1.020.jpeg)

![](Aspose.Words.d2a681ce-25a4-4145-a655-a9b5316407c1.021.jpeg)

(Рис. 15) фотографии выше, показывающие лабораторные отчеты, были добавлены в github.  

4. **Вывод:**  Я  изучил  идеологию  и  применение  версий  controls.  И  приобрел практические навыки работы с системой git. ![](Aspose.Words.d2a681ce-25a4-4145-a655-a9b5316407c1.002.png)

