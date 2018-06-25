---
title: Группы рассылки и EWS в Exchange
manager: sethgros
ms.date: 03/9/2015
ms.audience: Developer
localization_priority: Normal
ms.assetid: fe08c2e3-92a0-43ec-bc61-69b14caee8fe
description: Сведения о различных типах групп рассылки, доступных в Exchange, и способах управления ими с использованием приложения EWS или управляемого API EWS.
ms.openlocfilehash: 9b54bfd75f7d68f08c767171d99251b5ce86b7c4
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/25/2018
ms.locfileid: "19760951"
---
# <a name="distribution-groups-and-ews-in-exchange"></a>Группы рассылки и EWS в Exchange

Информация, содержащаяся в этом документе, может относиться к функциям и продуктам предварительной версии и может претерпеть значительные изменения до окончательного коммерческого выпуска. Настоящий документ предоставляется "как есть" и служит только для информационных целей. Корпорация Майкрософт не предоставляет никаких гарантий, явных или подразумеваемых, в связи с этим документом Сведения о различных типах групп рассылки, доступных в Exchange, и способах управления ими с использованием приложения EWS или управляемого API EWS.
  
Группа рассылки  это набор электронных адресов, связанных с одним псевдонимом или электронным адресом. Группы рассылки (также иногда называются списками рассылки) позволяют отправлять сообщения нескольким людям, используя один адрес получателя. Так как членством в группе рассылки (следовательно, и получателями сообщений) можно управлять, не открывая отдельные цепочки сообщений, группы рассылки  отличный способ отправлять почту группе пользователей. Можно программными средствами создавать группы рассылки и управлять ими, используя управляемые API EWS, EWS и командную консоль Exchange. Прежде чем приступить к программированию, рассмотрите различные доступные вам типы групп рассылки и возможности управления ими.
  
## <a name="types-of-distribution-groups"></a>Типы групп рассылки

Exchange поддерживает три типа групп рассылки:
  
- [Универсальные группы рассылки](distribution-groups-and-ews-in-exchange.md#bk_DistributionGroup)  объекты универсальной группы рассылки Active Directory с включенной поддержкой почты. Такие группы рассылки используются для доставки сообщений группе получателей. 
    
- [Группы безопасности](distribution-groups-and-ews-in-exchange.md#bk_SecurityGroup)  объекты Active Directory с включенной поддержкой почты, или универсальные группы безопасности. Группы безопасности используются для назначения прав доступа ресурсам в доменных службах Active Directory (AD DS), а также для распространения сообщений. 
    
- [Группы контактов](distribution-groups-and-ews-in-exchange.md#bk_ContactGroup)  частные группы безопасности, расположенные в почтовом ящике пользователя. 
    
При выборе типа группы рассылки следует учитывать, где вы планируете хранить такую группу, кем и в каких целях она будет использоваться.
  
### <a name="universal-distribution-groups"></a>Универсальные группы рассылки
<a name="bk_DistributionGroup"> </a>

С помощью универсальных групп рассылки можно объединять группы получателей под одним псевдонимом или электронным адресом. Так как универсальные группы рассылки хранятся в AD DS, кто угодно может использовать их для отправки электронной почты, в том числе пользователи за пределами организации. Вы можете использовать управляемый API EWS или EWS для развертывания групп рассылки, но для их создания и управления ими нужны [командлеты командной консоли Exchange](#bk_UsingEMS).
  
В универсальных группах рассылки также можно хранить набор комнат. Например, чтобы облегчить пользователям поиск переговорной для собрания. Пользователи могут добавить список комнат (универсальную группу рассылки, которая содержит почтовые ящики ресурсов комнат) в приглашение на собрание, чтобы находить доступную комнату без необходимости добавлять каждую комнату отдельно.
  
Можно создать статическую универсальную группу рассылки, которая остается неизменной до обновления членства, или динамическую универсальную группу рассылки. Динамическая универсальная группа рассылки запрашивает объекты Active Directory, поддерживающие почту, и создает членство в группе на основе результатов. Членство в группе пересчитывается при каждой отправке электронного сообщения группе. 
  
### <a name="security-groups"></a>Группы безопасности
<a name="bk_SecurityGroup"> </a>

Универсальные группы рассылки во многом подобны группам безопасности. Но в отличие от групп рассылки, вы можете использовать группы безопасности для назначения разрешений сетевым ресурсам в AD DS. Создавать группы безопасности или управлять ими невозможно с помощью управляемого API EWS или EWS. Для этого подходят [командлеты командной консоли Exchange](#bk_UsingEMS). Но как и в случае универсальных групп рассылки, для развертывания групп безопасности можно использовать управляемый API EWS или EWS.
  
### <a name="contact-groups"></a>Группы контактов
<a name="bk_ContactGroup"> </a>

Если вы не хотите предоставлять каждому пользователю административный доступ к серверу для создания групп рассылки, а только позволить им отправлять одно сообщение большой группе людей, вы можете сделать это с помощью группы контактов. С такой группой не сопоставлен электронный адрес, и она существует только в почтовом ящике одного пользователя. У других пользователей нет доступа к ней. Вы можете [использовать управляемый API EWS или EWS для создания групп контактов](how-to-create-contact-groups-by-using-ews-in-exchange.md).
  
## <a name="managing-distribution-groups-by-using-the-ews-managed-api-or-ews"></a>Управление группами рассылки с использованием управляемого API EWS или EWS

Вы можете использовать управляемый API EWS или EWS для развертывания универсальной группы рассылки или группы безопасности и контроля над созданием и управлением группы контактов. Но эти технологии не позволяют создавать и редактировать членов этих групп. 
  
**Таблица 1. Методы управляемого API EWS и операции EWS для управления группами рассылки**

|**Метод управляемого API EWS**|**Операция EWS**|**Используйте, чтобы…**|
|:-----|:-----|:-----|
|[Методы класса ContactGroup](http://msdn.microsoft.com/en-us/library/office/microsoft.exchange.webservices.data.contactgroup%28v=exchg.80%29.aspx)  <br/> |[CreatItem](http://msdn.microsoft.com/library/78a52120-f1d0-4ed7-8748-436e554f75b6%28Office.15%29.aspx) <br/> |Создать группу контактов в хранилище Exchange.  <br/> > [!NOTE]> Не создается универсальная группа рассылки или группу безопасности с помощью управляемого интерфейса API веб-служб Exchange или веб-служб Exchange.           |
|[ExpandGroup](http://msdn.microsoft.com/en-us/library/office/microsoft.exchange.webservices.data.exchangeservice.expandgroup%28v=exchg.80%29.aspx) <br/> |[ExpandDL](http://msdn.microsoft.com/library/1f7837e7-9eff-4e10-9577-c40f7ed6af94%28Office.15%29.aspx) <br/> |Развернуть универсальную группу рассылки, группу безопасности или группу контактов, получив список ее членов.  <br/> |
|[FindItems](http://msdn.microsoft.com/en-us/library/office/microsoft.exchange.webservices.data.exchangeservice.finditems%28v=exchg.80%29.aspx) <br/> |[FindItem](http://msdn.microsoft.com/library/ebad6aae-16e7-44de-ae63-a95b24539729%28Office.15%29.aspx) <br/> |Искать группу контактов в почтовом ящике.  <br/> |
|[GetRooms](http://msdn.microsoft.com/en-us/library/office/microsoft.exchange.webservices.data.exchangeservice.getrooms%28v=exchg.80%29.aspx) <br/> |[GetRooms](http://msdn.microsoft.com/library/5501ddc0-3bfa-4da6-8e15-4223ca5499a3%28Office.15%29.aspx) <br/> |Получить набор всех комнат в указанном списке комнат в организации. Список комнат представляет собой группу рассылки, которая содержит только почтовые ящики ресурсов комнат.  <br/> |
|[ResolveName](http://msdn.microsoft.com/en-us/library/office/microsoft.exchange.webservices.data.exchangeservice.resolvename%28v=exchg.80%29.aspx) <br/> |[ResolveNames](http://msdn.microsoft.com/library/6b4eb4b3-9ad6-4804-a09f-7e20cfea4dbb%28Office.15%29.aspx) <br/> |Поиск и возврат возможных кандидатов, соответствующих неоднозначному имени. Кандидатами могут быть группы рассылки.  <br/> |
   
Вы можете использовать информацию, возвращенную методом [ExpandGroup](http://msdn.microsoft.com/en-us/library/office/microsoft.exchange.webservices.data.exchangeservice.expandgroup%28v=exchg.80%29.aspx) или операцией [ExpandDL](http://msdn.microsoft.com/library/1f7837e7-9eff-4e10-9577-c40f7ed6af94%28Office.15%29.aspx), для определения типов членов в группе. Типы членов определяются перечислением [MailboxType](http://msdn.microsoft.com/en-us/library/office/microsoft.exchange.webservices.data.mailboxtype%28v=exchg.80%29.aspx) управляемого API EWS и элементом [MailboxType](http://msdn.microsoft.com/library/696e5fdb-d8c5-40f0-9e79-885eae65dfa4%28Office.15%29.aspx) EWS. 
  
**Таблица 2. Типы членов группы рассылки**

|**Значение перечисления MailboxType**|**Значение элемента MailboxType**|**Описание**|
|:-----|:-----|:-----|
|Почтовый ящик  <br/> |Почтовый ящик  <br/> |Объект Active Directory, поддерживающий почту.  <br/> |
|PublicGroup  <br/> |PublicDL  <br/> |Группа рассылки в группе, которую вы только что развернули. Чтобы открыть полный список членов, разверните также и эту группу.  <br/> |
|ContactGroup  <br/> |PrivateDL  <br/> |Группа контактов, расположенная в почтовом ящике и доступная только его пользователям.  <br/> |
|Контакт  <br/> |Контакт  <br/> |Контакт базы данных Exchange или почтовый контакт Active Directory.  <br/> |
   
## <a name="managing-distribution-groups-by-using-the-exchange-management-shell"></a>Управление группами рассылки с использованием командной консоли Exchange
<a name="bk_UsingEMS"> </a>

С помощью [командлетов командной консоли Exchange](http://msdn.microsoft.com/en-us/library/ff326159%28v=exchg.140%29.aspx) можно создавать универсальные группы рассылки и группы безопасности и управлять ими, используя код. 
  
> [!NOTE]
> [!Примечание] Командлеты командной консоли Exchange не подходят для управления группами контактов. 
  
**Таблица 3. Командлеты командной консоли Exchange для работы с группами рассылки**

|**Командлет**|**Используйте, чтобы…**|
|:-----|:-----|
|[Disable-DistributionGroup](http://technet.microsoft.com/en-us/library/aa997942%28v=exchg.150%29.aspx) <br/> |Удалить возможности почты из группы рассылки, поддерживающей почту.  <br/> |
|[Enable-DistributionGroup](http://technet.microsoft.com/en-us/library/aa998916%28v=exchg.150%29.aspx) <br/> |Добавить поддержку почты в существующую универсальную группу.  <br/> |
|[Get-DistributionGroup](http://technet.microsoft.com/en-us/library/bb124755%28v=exchg.150%29.aspx) <br/> |Отправить запрос на получение существующих групп рассылки.  <br/> |
|[Новый DistributionGroup](http://technet.microsoft.com/en-us/library/aa998856%28v=exchg.150%29.aspx) <br/> |Создать группу рассылки.  <br/> |
|[Remove-DistributionGroup](http://technet.microsoft.com/en-us/library/aa997627%28v=exchg.150%29.aspx) <br/> |Удалить существующую группу рассылки из AD DS.  <br/> |
|[SET-DistributionGroup](http://technet.microsoft.com/en-us/library/bb124955%28v=exchg.150%29.aspx) <br/> |Изменить параметры существующей группы рассылки.  <br/> |
|[Добавление DistributionGroupMember](http://technet.microsoft.com/en-us/library/bb124340%28v=exchg.150%29.aspx) <br/> |Добавить получателя в группу рассылки.  <br/> |
|[Get-DistributionGroupMember](http://technet.microsoft.com/en-us/library/aa996367%28v=exchg.150%29.aspx) <br/> |Искать членов существующей группы рассылки.  <br/> |
|[Remove-DistributionGroupMember](http://technet.microsoft.com/en-us/library/aa998016%28v=exchg.150%29.aspx) <br/> |Удалить существующего получателя из группы рассылки.  <br/> |
|[Update-DistributionGroupMember](http://technet.microsoft.com/en-us/library/dd335049%28v=exchg.150%29.aspx) <br/> |Обновить члена указанной группы рассылки.  <br/> |
|[Get-DynamicDistributionGroup](http://technet.microsoft.com/en-us/library/bb124762%28v=exchg.150%29.aspx) <br/> |Получить параметры существующей динамической группы рассылки.  <br/> |
|[Новый DynamicDistributionGroup](http://technet.microsoft.com/en-us/library/bb125127%28v=exchg.150%29.aspx) <br/> |Создать динамическую группу рассылки.  <br/> |
|[Remove-DynamicDistributionGroup](http://technet.microsoft.com/en-us/library/bb125038%28v=exchg.150%29.aspx) <br/> |Удалить существующую динамическую группу рассылки. Этот командлет удаляет динамическую группу рассылки из AD DS.  <br/> |
|[SET-DynamicDistributionGroup](http://technet.microsoft.com/en-us/library/bb123796%28v=exchg.150%29.aspx) <br/> |Изменить параметры существующей динамической группы рассылки.  <br/> |
   
## <a name="in-this-section"></a>В этом разделе
<a name="bk_UsingEMS"> </a>

- [Создание группы контактов с помощью веб-служб Exchange в Exchange](how-to-create-contact-groups-by-using-ews-in-exchange.md)
    
- [Разверните узел группы рассылки с помощью веб-служб Exchange в Exchange 2013](how-to-expand-distribution-groups-by-using-ews-in-exchange-2013.md)
    
## <a name="see-also"></a>См. также


- [Разработка клиентов веб-служб для Exchange](develop-web-service-clients-for-exchange.md)
    
- [Вызов командлетов командной консоли Exchange из управляемого кода](http://msdn.microsoft.com/en-us/library/ff326159%28v=exchg.140%29.aspx)
    

