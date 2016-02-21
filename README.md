# Try catch

Тестовое задание для кейса «Разработка  ПО для информационного табло в отдел продаж»     

Рассмотрим простую задачу – имеется отдел продаж из 10 сотрудников, каждый из них совершает различное число продаж услуг в течение дня, так же сотрудник может не совершить ни одной продажи за день. 

### В качестве перечня услуг и расценок введём следующее: 

* Базовые тарифы на интернет: http://spb.rt.ru/homeinternet/order_internet/base_tarifs
* Базовые тарифы на телевидение: http://spb.rt.ru/hometv/tariff 
* Базовые тарифы на цифровое телевидение: http://spb.rt.ru/digtv/tariffs
* Базовые тарифы на телефонию: http://spb.rt.ru/hometel/local 

### Примем в качестве условия, что стоимость подключения услуги равна стоимости первого месяца обслуживания. 

* Необходимо спроектировать и реализовать базу данных в которой будут отражены следующие сущности:         
    - Услуга – одна услуга из списка на сайте             
    - Продавец – физическое лицо              
    - Клиент – физическое лицо             
    - Продажа – дата+клиент+продавец+услуги купленные клиентом.            
* Сформированную базу данных заполнить сгенерированными записями:                
    - 10 сотрудников               
    - 10000 клиентов                   
    - Распределение услуг (тарифы можно заполнить случайно, все услуги были куплены в течение месяца):           
        * 10% клиентов приобрели только интернет (по одному из тарифов)           
        * 10% клиентов приобрели только телефонию              
        * 15% - только телевидение              
        * 5% - цифровое телевидение             
        * 25% - телевидение (любое) + телефон          
        * 15% - телевидение (любое) + телефон + интернет          
        * 20% - приобрели полный пакет услуг.            

### Задача приложения: 

	•	Формировать статистику по продавцам в виде графика:
	o	Продажи в разрезе дня по продавцам – гистограмма продавец-продажи;
	o	Продажи в разрезе месяца для каждого продавца - аналогично;
	o	Продажи в разрезе месяца для каждого продавца по конкретной услуге. 
	o	График продаж продавца в течение месяца – суммарно и по группам услуг. 

