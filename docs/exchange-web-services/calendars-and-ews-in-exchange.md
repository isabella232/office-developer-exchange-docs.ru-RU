---
title: Календари и веб-службах Exchange
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
localization_priority: Normal
ms.assetid: b87b0180-f5b5-44e4-b6ac-4f23e476b03b
description: Узнайте о календарей, папкам календаря и элементов, встречи и собрания в Exchange.
ms.openlocfilehash: bb9702118ff1db66862a5788c2d8f58dd55c4d09
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/11/2018
ms.locfileid: "19760934"
---
# <a name="calendars-and-ews-in-exchange"></a>Календари и веб-службах Exchange

Узнайте о календарей, папкам календаря и элементов, встречи и собрания в Exchange.
  
Возможно, вы знакомы с многие функции календаря в клиентов электронной почты, как Outlook, которые позволяют отслеживать встречи, планировать собрания, проверьте доступность людей, пригласить участников и изменение или Отмена собрания.
  
Возможности, связанные с календарем в Exchange, немного отличаются от в клиентом, например Outlook. Вместо отображения данных, веб-служб Exchange в Exchange позволяет выполнять такие действия, как создание, хранить, отправлять или изменить сведения. Чтобы использовать веб-служб Exchange для работы с календарями, необходимо ознакомиться с понятиями, таких как сведения о хранилище, время, повторения и поток сообщений. В частности необходимо ознакомиться со следующими:
  
- Папки календаря, элементы календаря и представления календаря
    
- Приглашения на собрания, ответы, планирования, участников, ресурсы, комнат и доступности
    
- Продолжительность времени, часовые пояса и времени начала и окончания собрания и встречи
    
- Ряд повторяющейся, шаблоны повторения, исключения и одиночных встреч и собраний
    
К счастью веб-служб Exchange и управляемый API EWS обеспечивают широкий набор операций и методы, которые позволяют выполнять множество задач, связанных с календаря. Например с помощью управляемого интерфейса API веб-служб Exchange, можно организовать собрание и отправлять приглашения на собрания с помощью нескольких строк кода, как показано в следующем примере.
  
```cs
            Appointment meeting = new Appointment(service);
            // Set the properties on the meeting object to create the meeting.
            meeting.Subject = "Team building exercise";
            meeting.Body = "Let's learn to really work as a team and then have lunch!";
            meeting.Start = DateTime.Now.AddDays(2);
            meeting.End = meeting.Start.AddHours(2);
            meeting.Location = "Conference Room 12";
            meeting.RequiredAttendees.Add("Mack.Chaves@contoso.com");
            meeting.RequiredAttendees.Add("Sadie.Daniels@contoso.com");
            meeting.OptionalAttendees.Add("Magdalena.Kemp@contoso.com");
            meeting.ReminderMinutesBeforeStart = 60;
            // Send the meeting request
            meeting.Save(SendInvitationsMode.SendToAllAndSaveCopy);

```

## <a name="calendar-folders-and-calendar-items"></a>Папки календаря и элементы календаря
<a name="bk_CalendarFolder"> </a>

Папки календаря содержат элементы календаря. Папки календаря имеют [папки класс](http://msdn.microsoft.com/library/0041d135-2869-4612-89a5-d1aa86aa1093%28Office.15%29.aspx) **IPF. Встреча**и может содержать только элементы, определенные в свойстве управляемый API EWS [ItemClass](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.item.itemclass%28v=exchg.80%29.aspx) , связанной с объектом [Класса встречи](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.appointment%28v=exchg.80%29.aspx) или элемент веб-служб Exchange [CalendarItemType](http://msdn.microsoft.com/library/1feb0788-adf7-4a7c-830c-005214ad930f%28Office.15%29.aspx) . 
  
Элементов в папке календаря являются немного отличаться от элементов в других папках в почтовый ящик, поскольку вхождений в ряду и исключения из серии повторяющихся не фактические элементов в почтовом ящике, но вместо хранятся во внутренней сети, в виде вложений повторяющейся Образец. Таким образом Чтобы получить все встречи в определенный период, необходимо использовать календарном представлении. Дополнительные сведения о получении встреч и представления календаря видеть [получить встречи и собрания с помощью веб-служб Exchange в Exchange](how-to-get-appointments-and-meetings-by-using-ews-in-exchange.md).
  
## <a name="meetings-and-appointments"></a>Собрания и встречи
<a name="bk_meetings"> </a>

Важные различия между собраний и встреч —, что у участников собрания, а не встреч. Для внутреннего использования Exchange использует тот же объект для собраний и встреч. Использовать управляемый API EWS [класс встречи](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.appointment%28v=exchg.80%29.aspx) или элемент веб-служб Exchange [элемента календаря, имеющего](http://msdn.microsoft.com/library/b0c1fd27-b6da-46e5-88b8-88f00c71ba80%28Office.15%29.aspx) для работы с собраний и встреч. 
  
Встречи и собрания могут быть отдельные экземпляры или частью [серии повторяющихся](recurrence-patterns-and-ews.md), но поскольку встреч не включать участников, комнат или ресурсов, не требуется отправить сообщение.
  
Так как собраний отправки и отвечать на запросы и обновления, они включают в себя больше, чем просто доступ к элементов в папке календаря. Они также могут связанного рабочего процесса. Необходимо запланировать собрания, если участники доступны и может также включать в себя резервирование конференц-зала или ресурсов, таких как проектор или другого оборудования.
  
Рабочий процесс собрания обычно состоит из следующих действий:
  
1. Собрания созданы и заполнены с начала и время окончания, расположение и текст сообщения.
    
2. Создать список потенциальных участников, ресурсы и комнаты.
    
3. Проверяется состояние доступности участников. 
    
4. Приглашения на собрание отправляется участников.
    
5. Участники ответ на собрание с выполняемое посещение или нет. Участники могут также предложить новое время собрания.
    
6. Собрания можно остановить или обновления, который обычно запуск новых сообщений, отправляемых участникам.
    
## <a name="calendars-and-time"></a>Календари и времени
<a name="bk_Time"> </a>

Функции, связанные с временем включается ведение календаря. Встречи и собрания иметь начала и окончания, длительности и другие свойства, связанные с времени, например, время создания, отправки и получения сообщения. Существующие встречи и собрания могут быть получены из папки календаря на основе времени начала и окончания. Повторяющееся иметь основные компоненты и заканчивается. И собраний в пределах указанной часовой пояс, который является очень важно в глобальной экономики.
  
Время хранятся во внутренней сети на сервере Exchange server в формате UTC. Exchange преобразует их в локальный часовой пояс, на основе параметров клиента. Свойства [даты и времени](http://msdn.microsoft.com/library/9c6ecd4c-779c-4fa5-8082-dd2bc0a751f4%28Office.15%29.aspx) распространяются локального часового пояса. 
  
## <a name="recurring-series"></a>Повторяющееся
<a name="bk_recurrence"> </a>

Ряд повторяющейся встречи или собрания включает в себя образцом повторения набора элементов вхождение и при необходимости набора элементов исключение. Сведения о повторения хранятся на повторяющегося элемента шаблона. Элемент веб-служб Exchange [RecurringMasterItemId](http://msdn.microsoft.com/library/5800b58c-f3d7-4d8f-acc0-d13e02f4e258%28Office.15%29.aspx) связан с вхождений и исключений из серии, или можно использовать метод веб-служб Exchange [Appointment.BindToRecurringMaster](http://msdn.microsoft.com/en-us/library/dd635978%28v=EXCHG.80%29.aspx) управляемого интерфейса API для получения регулярное главной. С помощью экземпляра ряда, можно найти все элементы и сведения, связанные с серии. 
  
Обратите внимание на то, что повторения свойства существуют во всех элементах календаря, но записываются только на повторяющиеся основные элементы. Помимо индекса все вхождения из серии повторяющихся главных содержит ссылку на измененные и удаленные вхождений и повторов рядов (например, ежедневно, еженедельно, ежемесячно или ежегодно).
  
## <a name="in-this-section"></a>В этом разделе
<a name="bk_inthissection"> </a>

- [Создание встречи и собрания с помощью веб-служб Exchange в Exchange 2013](how-to-create-appointments-and-meetings-by-using-ews-in-exchange-2013.md)
    
- [Создание событий на целый день с помощью веб-служб Exchange в Exchange](how-to-create-all-day-events-by-using-ews-in-exchange.md)
    
- [Получение встречи и собрания с помощью веб-служб Exchange в Exchange](how-to-get-appointments-and-meetings-by-using-ews-in-exchange.md)
    
- [Обновление встречи и собрания с помощью веб-служб Exchange в Exchange](how-to-update-appointments-and-meetings-by-using-ews-in-exchange.md)
    
- [Удаление встреч и отмены собраний с помощью веб-служб Exchange в Exchange](how-to-delete-appointments-and-cancel-meetings-by-using-ews-in-exchange.md)
    
- [Получить список помещений с помощью веб-служб Exchange в Exchange](how-to-get-room-lists-by-using-ews-in-exchange.md)
    
- [Получение сведений о доступности с помощью веб-служб Exchange в Exchange](how-to-get-free-busy-information-by-using-ews-in-exchange.md)
    
- [Предложение нового времени проведения собрания с помощью веб-служб Exchange в Exchange](how-to-propose-a-new-meeting-time-by-using-ews-in-exchange.md)
    
- [В Exchange обработки элементов календаря в пакетах](how-to-process-calendar-items-in-batches-in-exchange.md)
    
- [Шаблоны повторения и веб-служб Exchange](recurrence-patterns-and-ews.md)
    
## <a name="see-also"></a>См. также


- [Разработка клиентов веб-служб для Exchange](develop-web-service-clients-for-exchange.md)
    
- [Начать работу с использованием веб-служб Exchange](start-using-web-services-in-exchange.md)
    
- [Общие сведения о разработке клиента EWS для Exchange](ews-client-design-overview-for-exchange.md)
    

