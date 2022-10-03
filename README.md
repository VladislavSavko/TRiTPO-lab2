# TRiTPO-lab2

# Требования к проекту
---
# Содержание
1 [Введение](#intro)
1.1 [Название продукта](#product_name)
1.2 [Назначение документа](#appointment)  
1.3 [Бизнес-требования](#business_requirements)  
1.3.1 [Исходные данные](#initial_data)  
1.2.2 [Возможности бизнеса](#business_opportunities)  
1.2.3 [Границы проекта](#project_boundary)  
1.3 [Аналоги](#analogues)  
2 [Требования пользователя](#user_requirements)  
2.1 [Программные интерфейсы](#software_interfaces)  
2.2 [Интерфейс пользователя](#user_interface)  
2.3 [Характеристики пользователей](#user_specifications)  
2.3.1 [Классы пользователей](#user_classes)  
2.3.2 [Аудитория приложения](#application_audience)  
2.3.2.1 [Целевая аудитория](#target_audience)  
2.3.2.1 [Побочная аудитория](#collateral_audience)  
2.4 [Предположения и зависимости](#assumptions_and_dependencies)  
3 [Системные требования](#system_requirements)  
3.1 [Функциональные требования](#functional_requirements)  
3.1.1 [Основные функции](#main_functions)  
3.1.1.1 [Вход пользователя в приложение](#user_logon_to_the_application)  
3.1.1.2 [Настройка профиля активного пользователя](#setting_up_the_profile_of_the_active_user)  
3.1.1.3 [Загрузка новостей](#download_news)  
3.1.1.4 [Просмотр информации об отдельной новости](#view_information_about_an_individual_newsletter)  
3.1.1.5 [Выход пользователя из учётной записи](#active_user_change)  
3.1.1.6 [Регистрация нового пользователя после входа в приложение](#add_new_user)  
3.1.2 [Ограничения и исключения](#restrictions_and_exclusions)  
3.2 [Нефункциональные требования](#non-functional_requirements)  
3.2.1 [Атрибуты качества](#quality_attributes)  
3.2.1.1 [Требования к удобству использования](#requirements_for_ease_of_use)  
3.2.1.2 [Требования к безопасности](#security_requirements)  
3.2.2 [Внешние интерфейсы](#external_interfaces)  
3.2.3 [Ограничения](#restrictions)  
---


# 1 Введение

## 1.1 Название продукта
MovieBox

## 1.2 Назначение документа
В этом документе описаны функциональные и нефункциональные требования к приложению «MovieBox» для ОС Windows 10.
Этот документ предназначен для команды, которая будет реализовывать и проверять корректность работы приложения.

## 1.3 Бизнес-требования

### 1.3.1 Исходные данные
Просмотр фильмов является одним из самых распространенных видов досуга. Буквально 10 лет назад основными ресурсами просмотра фильмов для людей
любых возрастных категорий были телевидение и кинотеатры. Однако, не все жанры фильмов могут быть интересны зрителю, или может не быть возможности
сходить в кинотеатр на приглянувшийся фильм. С развитием технологий онлайн-кинотеатров люди получили возможность персонализировать свои интересы,
ознакамливаться с интересами других людей и выбирать фильм любого жанра и рейтинга, не заботясь о подборе времени для просмотра или фильма по интересам.
В связи с этим появляется множество интернет-приложений(сервисов), позволяющих использовать технологии просмотра и подборки фильмов онлайн.

### 1.3.2 Возможности бизнеса
Многие люди желают иметь приложение(веб-сервис), позволяющее просматривать фильмы любых жанров онлайн, подбирать фильмы для пользователя, основываясь на
его предпочтениях и оценках. Подобное приложение позволит им тратить меньше времени на поиск необходимой информации и использовать приложение в удобное время, 
не подстаиваясь под ТВ-расписание или прокат в кинотеатрах. Интерфейс, спроектированный с учётом всех особенностей похожих технологий, и дополнение приложения подробной инструкцией позволят увеличить количество людей, использующих данное приложение.

### 1.3.3 Границы проекта
Приложение "MovieBox" позволит зарегистрированным пользователям просматривать фильмы любого жанра и года выпуска онлайн, скачивать фильмы для дальнейшего просмотра
оффлайн, формировать свой рейтинг фильмов, получать подборку от пользователей с похожими оценками на фильмы и от самого приложения, основываясь на предпочтениях
пользователя и его оценках, видеть сформированный приложением рейтинг фильмов и оставлять отзывы на фильмы на общем ресурсе. Незарегистрированным пользователям будут доступны только:просмотр трейлеров фильмов, просмотр оценок на фильмы и чтение отзывов

## 1.4 Аналоги
«Кинопо́иск» — крупнейший русскоязычный интернет-сервис о кино. С 2018 года также доступен онлайн-кинотеатр (до 2 ноября 2021 имевший отдельное название — КиноПоиск HD) с несколькими тысячами фильмов, сериалов, мультфильмов, в том числе премьерных и эксклюзивных. Сервис позволяет просматривать фильмы и получать подборки, основываясь на предпочтениях пользователя.
Internet Movie Database (IMDb, в переводе с англ. — «Интернет-база фильмов») — веб-сайт со свободно редактируемой и крупнейшей в мире базой данных о кинематографе. По состоянию на январь 2021 года, в базе собрана информация о более чем 6,5 млн кинофильмов, телесериалов и отдельных их серий, а также о 10,4 млн персоналий, связанных с кино и телевидением, — актёрах, режиссёрах, сценаристах и других[1]. Сервис позволяет получать любые сведения о фильмах и изучать оценки и отзывы пользователей
Netflix, Inc. — американская развлекательная компания, а также стриминговый сервис фильмов и сериалов. Основана 29 августа 1997 года Ридом Хастингсом и Марком Рэндольфом[3]. Штаб-квартира находится в Лос-Гатосе, Калифорния. Cервис позволяет просматривать фильмы и получать доступ к оценкам и рецензиям.

#2 Требования пользователя

#2.1 Программные интерфейсы
Главное окно приложения()
Окно входа в приложение()
Окно регистрации нового пользователя()
Главное окно приложения после выбора фильма()
Окно настройки профиля пользователя()








