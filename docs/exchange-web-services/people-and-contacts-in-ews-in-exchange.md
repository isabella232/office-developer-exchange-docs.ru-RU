---
title: Пользователи и контакты в EWS для Exchange
manager: sethgros
ms.date: 03/9/2015
ms.audience: Developer
localization_priority: Normal
ms.assetid: 043c33be-a0d1-4bad-a840-85715eda4813
description: 'Сведения о фиктивных пользователях, едином хранилище контактов и работе с контактами с помощью EWS в Exchange или управляемого API для EWS. '
ms.openlocfilehash: fe11c6247cade8e78610d953088f6d593bdb560c
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/11/2018
ms.locfileid: "19761234"
---
# <a name="people-and-contacts-in-ews-in-exchange"></a>Пользователи и контакты в EWS для Exchange

Сведения о фиктивных пользователях, едином хранилище контактов и работе с контактами с помощью EWS в Exchange или управляемого API для EWS.  
  
Контакты — это элементы в Exchange, в которых хранится информация об отдельных людях, группах или организациях. Контакты могут включать имена, электронные адреса и другие данные, в том числе адреса для IM, физические адреса, информацию о семье и днях рождения, фотографию или изображение.
  
Контактные данные хранятся в одном из двух расположений:
  
- Доменных служб Active Directory (AD DS), если контакт находится в пределах организации.
    
- в папке "Контакты" или другой папке почтового ящика пользователя, если контакт находится вне организации.
    
Несколько элементов контактов может представлять отдельный пользователь. Exchange использует действующие лица для объединения этих различных элементов контакта. *Пользователь* является объединенные контактные данные для одного пользователя из различных источников. В дополнение к контактной информации в Exchange, действующие лица можно также объединить на основании сведений в кэше получателей для почтового ящика, скрытые папки для вызывается QuickContacts, контакты обмена мгновенными Сообщениями и из источников данных сторонних производителей. Единого хранилища контактов в Exchange позволяет клиентам обмена мгновенными Сообщениями для использования в этом объединение; Единственное отличие заключается в том, что единого хранилища контактов не вычисляется в Доменных службах Active Directory, сведения, как показано на рисунке 1. 
  
**На рисунке 1. Источники контактные данные для пользователей, а также для единого хранилища контактов**

![Изображение с источниками, объединенными в пользователей, и источниками, включенными в единое хранилище контактов. Единое хранилище контактов не объединяет контактные данные из службы каталогов.](media/EX15_PersonaOverview.png)
  
**В таблице 1. Управляемый API EWS методы и операций веб-служб Exchange для работы с контактами**

|**Если вы хотите...**|**Используйте этот метод управляемый API EWS**|**Используйте эту операцию EWS**|
|:-----|:-----|:-----|
|Создать контакт  <br/> |Создайте экземпляр объекта [контакта](http://msdn.microsoft.com/en-us/library/office/microsoft.exchange.webservices.data.contact%28v=exchg.80%29.aspx) и использовать [Contact.Save](http://msdn.microsoft.com/en-us/library/office/microsoft.exchange.webservices.data.contact.save%28v=exchg.80%29.aspx) <br/> |[CreateItem](http://msdn.microsoft.com/library/417e994b-0a17-4c24-9527-04796b80b029%28Office.15%29.aspx) <br/> |
|Копировать контакт  <br/> |[Contact.Copy](http://msdn.microsoft.com/en-us/library/office/microsoft.exchange.webservices.data.contact.copy%28v=exchg.80%29.aspx) <br/> |[CopyItem](http://msdn.microsoft.com/library/bcc68f9e-d511-4c29-bba6-ed535524624a%28Office.15%29.aspx) <br/> |
|Переместить контакт  <br/> |[Contact.Move](http://msdn.microsoft.com/en-us/library/office/microsoft.exchange.webservices.data.contact.move%28v=exchg.80%29.aspx) <br/> |[MoveItem](http://msdn.microsoft.com/library/dcf40fa7-7796-4a5c-bf5b-7a509a18d208%28Office.15%29.aspx) <br/> |
|Обновить существующий контакт  <br/> |[Contact.Bind](http://msdn.microsoft.com/en-us/library/office/microsoft.exchange.webservices.data.contact.bind%28v=exchg.80%29.aspx) и [Contact.Update](http://msdn.microsoft.com/en-us/library/office/microsoft.exchange.webservices.data.contact.update%28v=exchg.80%29.aspx) <br/> |[UpdateItem](http://msdn.microsoft.com/library/298fdd71-a83d-4407-9728-4f0a8e2d857c%28Office.15%29.aspx) <br/> |
|Удалить контакт  <br/> |[Contact.Bind](http://msdn.microsoft.com/en-us/library/office/microsoft.exchange.webservices.data.contact.bind%28v=exchg.80%29.aspx) и [Contact.Delete](http://msdn.microsoft.com/en-us/library/office/microsoft.exchange.webservices.data.contact.delete%28v=exchg.80%29.aspx) <br/> |[DeleteItem](http://msdn.microsoft.com/library/3e26c416-fa12-476e-bfd2-5c1f4bb7b348%28Office.15%29.aspx) <br/> |
|Найти контакт  <br/> |[ExchangeService.FindItems](http://msdn.microsoft.com/en-us/library/office/microsoft.exchange.webservices.data.exchangeservice.finditems%28v=exchg.80%29.aspx) <br/> |[FindItem](http://msdn.microsoft.com/library/ebad6aae-16e7-44de-ae63-a95b24539729%28Office.15%29.aspx) <br/> |
|Найти пользователей  <br/> |Н/д  <br/> |[FindPeople](http://msdn.microsoft.com/library/446106b7-ff2d-4107-90c1-29f4d38ba128%28Office.15%29.aspx) <br/> |
|Развернуть группу рассылки  <br/> |[ExchangeService.ExpandGroup](http://msdn.microsoft.com/en-us/library/office/microsoft.exchange.webservices.data.exchangeservice.expandgroup%28v=exchg.80%29.aspx) <br/> |[ExpandDL](http://msdn.microsoft.com/library/1f7837e7-9eff-4e10-9577-c40f7ed6af94%28Office.15%29.aspx) <br/> |
|Устранить неоднозначность имени  <br/> |[ExchangeService.ResolveName](http://msdn.microsoft.com/en-us/library/office/microsoft.exchange.webservices.data.exchangeservice.resolvename%28v=exchg.80%29.aspx) <br/> |[ResolveNames](http://msdn.microsoft.com/library/6b4eb4b3-9ad6-4804-a09f-7e20cfea4dbb%28Office.15%29.aspx) <br/> |
|Получить фиктивного пользователя  <br/> |Н/д  <br/> |[GetPersona](http://msdn.microsoft.com/library/e2146df0-53d0-4caf-9758-b600bbc14b6a%28Office.15%29.aspx) <br/> |
|Обработать фотографии контакта  <br/> |[Contact.SetContactPicture](http://msdn.microsoft.com/en-us/library/office/microsoft.exchange.webservices.data.contact.setcontactpicture%28v=exchg.80%29.aspx), [Contact.GetContactPictureAttachment](http://msdn.microsoft.com/en-us/library/office/microsoft.exchange.webservices.data.contact.getcontactpictureattachment%28v=exchg.80%29.aspx)или [Contact.RemoveContactPicture](http://msdn.microsoft.com/en-us/library/office/microsoft.exchange.webservices.data.contact.setcontactpicture%28v=exchg.80%29.aspx) <br/> |[GetUserPhoto](http://msdn.microsoft.com/library/f6e8143d-4235-428e-8f9c-ab6e9b1cfa6e%28Office.15%29.aspx) или [GetAttachment](http://msdn.microsoft.com/library/24d10a15-b942-415e-9024-a6375708f326%28Office.15%29.aspx) <br/> |
   
## <a name="personas"></a>Фиктивные пользователи
<a name="PEOPLESEARCH"> </a>

До недавних пор контакты обычно сохранялись централизованно (как правило, в почтовом клиенте). Сейчас контакты все чаще сохраняются в различных расположениях (например, на телефоне, сайте социальной сети, в папке "Контакты" почтового ящика Exchange или службе каталогов организации). Из-за размещения контактных данных в различных расположениях несколько контактов, представляющих одного и того же человека, могут включать неодинаковые сведения. Например, один контакт может содержать рабочий номер телефона, а другой — личный. Имя контакта, сохраненного в папке "Контакты", может также отличаться от имени контакта, сохраненного на телефоне.
  
В Exchange Online, Exchange Online в составе Office 365 и локальной версии Exchange, начиная с Exchange 2013 контакты из различных источников, которые представляют тот же связаны друг с другом, аналогичную то, как сообщения электронной почты, объединить в беседах с помощью общего связать код. При возвращении сводный контактные данные с сервера Exchange, он содержит набор атрибутов для каждого контакта, такие как исходной папки, отображаемое имя, идентификатор и идентификатор источника Сумма свойства и атрибуты, возвращаемые называется пользователя и набор свойств, возвращаемых называется [фигуры пользователя](http://msdn.microsoft.com/library/61d87cd5-3270-40d1-bab7-d0d5bf938607%28Office.15%29.aspx).
  
Поскольку данные, составляющих пользователя не хранятся в одном месте, и эти сведения можно изменить в любое время, пользователя создается только в том случае, если для выполнения запроса к серверу Exchange. Используйте операцию EWS [FindPeople](http://msdn.microsoft.com/library/446106b7-ff2d-4107-90c1-29f4d38ba128%28Office.15%29.aspx) для создания запроса поиска пользователя. Запрос может включать порядок сортировки и могут быть отфильтрованы в соответствии с строки запроса, которые помогут вам найти правильный пользователя, сортировки и фильтрации результатов, полученных. Например, вы можете получить отображаемое имя и набор всех адресов электронной почты, связанные с определенным контактом, из папки «Контакты», учетной записи Hotmail, учетную запись LinkedIn и службой каталогов, или можно извлечь набор всех пользователей, иметь адреса обмена мгновенными Сообщениями. Связывание контактов в действующие лица осуществляется автоматически на основании алгоритм, который определяет отношение между контакты, хранящиеся на различных устройствах. 
  
> [!NOTE]
> Управляемый API EWS не реализует эту функцию. 
  
**В таблице 2. Операции EWS для работы с пользователями**

|**Имя операции**|**Описание**|
|:-----|:-----|
|[FindPeople](http://msdn.microsoft.com/library/446106b7-ff2d-4107-90c1-29f4d38ba128%28Office.15%29.aspx) <br/> |Возвращает всех доступных фиктивных пользователей из указанной папки контактов или извлекает контакты, которые соответствуют заданной строке запроса.  <br/> |
|[GetPersona](http://msdn.microsoft.com/library/e2146df0-53d0-4caf-9758-b600bbc14b6a%28Office.15%29.aspx) <br/> |Возвращает набор свойств, сопоставленных с определенным фиктивным пользователем, таких как все адреса для IM или отображаемые имена, по указанному идентификатору фиктивного пользователя.  <br/> |
   
Операции **GetPersona** и **FindPeople** можно использовать для эффективного получения контактных сведений из нескольких источников. Так как все элементы, связанные с пользователя, связанные с ИД ссылки, можно использовать эти операции в широком спектре различных приложений, использующих контактные данные. Ниже приведены некоторые примеры: 
  
- Приложение мобильного телефона, использующего операция **GetPersona** , когда пользователь вызывает контакт и предлагает дополнительные номера телефонов для вызова, если никто не отвечает. 
    
- Приложение, использующее **FindPeople** операции для сканирования папки «Входящие» сообщения для адресов электронной почты определить, является ли они находятся в существующего. Адреса, которые не связаны с пользователя уже используется для создания продаж или список всех последних сообщений с человеком, представленное этого пользователя. 
    
- [Почтовое приложение для Outlook](mail-apps-for-outlook-and-ews-in-exchange.md) , в котором представлены различные приветствия в зависимости от того, является ли соответствие строгая или свободная. Официальные приветствий в телефонном отображаемые имена из службы каталогов и неофициальные приветствий поступают из отображаемое имя, которая исходит в социальных сетях контакты. 
    
## <a name="unified-contact-store"></a>Единое хранилище контактов
<a name="PEOPLESEARCH"> </a>

Фиктивные пользователи доступны не только в почтовом клиенте. Если вы разрабатываете клиент для обмена мгновенными сообщениями, задайте себе такие вопросы (можно все):
  
- Как можно подготовить Lync клиентских приложений по умолчанию набор элементов контактов обмена мгновенными Сообщениями?
    
- Как управлять списками групп и контактов для IM?
    
- Как управлять специальным клиентским доступом Lync к контактам и группам для IM?
    
Единое хранилище контактов незаметно работает в Exchange, объединяя контактные данные из Exchange и других источников в единую сущность (создавая фиктивного пользователя). Хотя операции EWS, которые вы используете для доступа к единому хранилищу контактов, касаются только контактов для IM, с помощью этого хранилища в Exchange можно работать с фиктивными пользователями в приложениях всех типов. Помните, что у единого хранилища контактов нет доступа к контактным данным AD DS.
  
Служб обмена мгновенными сообщениями, хранятся в скрытых папку с именем QuickContacts. Операции **AddNewImContactToGroup** и **AddImContactToGroup** можно использовать для добавления контактов в группы, которые хранятся в этой папке скрытых. И так, как можно использовать единого хранилища контактов группы мгновенные сообщения контактам, могут получить доступ к и более простое редактирование групп контактов. 
  
> [!NOTE]
> Управляемый API EWS не реализует эту функцию. 
  
**В таблице 3. Операции веб-служб Exchange для доступа к единого хранилища контактов**

|**Имя операции**|**Описание**|
|:-----|:-----|
|[AddNewImContactToGroup](http://msdn.microsoft.com/library/0cb5525f-faa3-48f1-9551-df55ffc26f46%28Office.15%29.aspx) <br/> |Добавляет новый контакт для IM в группу для IM (количество контактов не должно превышать 1000).   <br/> |
|[AddImContactToGroup](http://msdn.microsoft.com/library/376acc42-2684-4596-aca1-82a4a10865c9%28Office.15%29.aspx) <br/> |Добавляет существующий контакт для IM в группу для IM (количество контактов не должно превышать 1000).   <br/> |
|[AddImGroup](http://msdn.microsoft.com/library/6df6e504-b7c8-4773-b10f-ffa5defac229%28Office.15%29.aspx) <br/> |Добавляет новую группу для IM (максимальное количество групп — 64).  <br/> |
|[AddDistributionGroupToImList](http://msdn.microsoft.com/library/5aa9bec8-71cf-4a6e-8ec8-b4965b40fd4a%28Office.15%29.aspx) <br/> |Добавляет новую группу рассылки в группу для IM (максимальное количество групп — 64).  <br/> |
|[GetImItemList](http://msdn.microsoft.com/library/e31d14e1-0c1f-4b69-98b7-157d59c13698%28Office.15%29.aspx) <br/> |Получает список групп для IM и фиктивных пользователей, включающих контакты для IM.  <br/> |
|[GetImItems](http://msdn.microsoft.com/library/51186691-46d2-4d5c-b8bc-4ee2bb20fbe7%28Office.15%29.aspx) <br/> |Получает сведения о конкретных группах для IM и фиктивных пользователях, включающих контакты для IM.  <br/> |
|[RemoveContactFromImList](http://msdn.microsoft.com/library/28ec96c3-45af-48ff-9f17-718a527dc0ad%28Office.15%29.aspx) <br/> |Удаляет контакт из группы для IM.  <br/> |
|[RemoveImContactFromGroup](http://msdn.microsoft.com/library/a190bbec-c71b-4e6a-880b-55854c724d8c%28Office.15%29.aspx) <br/> |Удаляет контакт для IM из группы для IM.  <br/> |
|[RemoveDistributionGroupFromImList](http://msdn.microsoft.com/library/252bddf2-98b6-4824-b548-2fba2bda5384%28Office.15%29.aspx) <br/> |Удаляет группу рассылки из группы для IM.  <br/> |
|[RemoveImGroup](http://msdn.microsoft.com/library/5e788016-68e0-4a3f-9243-03f6b6c6b389%28Office.15%29.aspx) <br/> |Удаляет группу для IM.  <br/> |
|[SetImGroup](http://msdn.microsoft.com/library/2d48aa07-8152-4c3d-a519-061253e80174%28Office.15%29.aspx) <br/> |Изменяет отображаемое имя группы для IM.  <br/> |
   
## <a name="in-this-section"></a>В этом разделе
<a name="PEOPLESEARCH"> </a>

- [Процесс контакты партиями с помощью веб-служб Exchange в Exchange](how-to-process-contacts-in-batches-by-using-ews-in-exchange.md)
    
- [Разрешения неоднозначных имен с помощью веб-служб Exchange в Exchange 2013](how-to-resolve-ambiguous-names-by-using-ews-in-exchange-2013.md)
    
- [Получение фотографий с помощью веб-служб Exchange в Exchange](how-to-get-user-photos-by-using-ews-in-exchange.md)
    
## <a name="see-also"></a>См. также
<a name="PEOPLESEARCH"> </a>

- [Разработка клиентов веб-служб для Exchange](develop-web-service-clients-for-exchange.md)
    
- [Начать работу с использованием веб-служб Exchange](start-using-web-services-in-exchange.md)
    
- [Общие сведения о разработке клиента EWS для Exchange](ews-client-design-overview-for-exchange.md)
    

