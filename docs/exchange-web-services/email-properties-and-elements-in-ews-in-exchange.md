---
title: Свойства и элементы электронной почты в EWS в Exchange
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
localization_priority: Normal
ms.assetid: 5266ff9f-d828-4ef4-b8ec-7b27d355c4c5
description: Сведения о первом классе и других свойствах и элементах, которые можно получить в сообщениях электронной почты с помощью управляемого API EWS или EWS в Exchange.
ms.openlocfilehash: 4866c69213eb8b11c785ab14f0595c45448834d8
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/25/2018
ms.locfileid: "19760966"
---
# <a name="email-properties-and-elements-in-ews-in-exchange"></a>Свойства и элементы электронной почты в EWS в Exchange

Сведения о первом классе и других свойствах и элементах, которые можно получить в сообщениях электронной почты с помощью управляемого API EWS или EWS в Exchange.
  
Сообщения электронной почты имеют более 50 свойств и при необходимости могут получить нужные сообщения, если вы не знаете, где их искать. Самое важное, что нужно знать о работе с свойствами и элементами электронной почты, которые включены в набор свойств и элементов первого класса, возвращаемых каждым из основных методов и операций извлечения. Набор возвращаемых свойств первого класса зависит от используемого метода извлечения. Кроме того, не следует обмануть значение Аллпропертиес элемента [басешапе](http://msdn.microsoft.com/library/42c04f3b-abaa-4197-a3d6-d21677ffb1c0%28Office.15%29.aspx) EWS, которое соответствует значению перечисления [басепропертисет. фирстклассмессажепропертиес](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.basepropertyset%28v=exchg.80%29.aspx) в управляемом API EWS. Это значение фактически не включает все свойства, но включает только свойства первого класса. 
  
## <a name="first-class-properties-and-elements-for-email-messages"></a>Свойства и элементы первого класса для сообщений электронной почты
<a name="bk_firstclass"> </a>

Набор свойств и элементов первого класса, возвращаемых методом [EmailMessage. Bind](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.emailmessage.bind%28v=exchg.80%29.aspx) управляемого API EWS и ОПЕРАЦИей EWS, немного отличается от набора свойств и элементов, возвращаемых методом [ExchangeService. FINDITEMS](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.exchangeservice.finditems%28v=exchg.80%29.aspx) управляемого API EWS [и операцией](http://msdn.microsoft.com/library/e8492e3b-1c8d-4b14-8070-9530f8306edd%28Office.15%29.aspx) [FindItem](http://msdn.microsoft.com/library/ebad6aae-16e7-44de-ae63-a95b24539729%28Office.15%29.aspx) . Свойства первого класса, возвращаемые методом **FindItems** и операцией **FindItem** , являются подмножеством свойств, возвращаемых методом **BIND** и операцией **GetItem** . В таблице 1 перечислены все свойства первого класса, возвращаемые методом **BIND** и операцией **GetItem** , и указано, какие из них не возвращаются методом **FindItems** или операцией **FindItem** . Обратите внимание, что нельзя расширять метод **FindItems** или операцию **FindItem** для получения дополнительных свойств и элементов, таких как **ToRecipients**, **CcRecipients**и **BccRecipients**. Если необходимо извлечь эти значения, используйте метод **FindItems** или операцию **FindItem** для получения идентификаторов элементов электронной почты, а затем используйте метод **BIND** или операцию **GetItem** для получения необходимых свойств. Примеры кода, демонстрирующие извлечение элементов с помощью метода **BIND** или **FindItems** , приведены в статье [Получение элемента с помощью управляемого API EWS](how-to-work-with-exchange-mailbox-items-by-using-ews-in-exchange.md#bk_getewsma). Примеры кода, в которых показано, как получить элементы с помощью операций **GetItem** или **FindItem** , можно узнать в статье [Получение элемента с помощью EWS](how-to-work-with-exchange-mailbox-items-by-using-ews-in-exchange.md#bk_getews).
  
Свойства и элементы первого класса перечислены в следующей таблице в том порядке, в котором они отображаются в отклике.
  
**Таблица 1. Свойства и элементы электронной почты первого класса**

|**Свойство управляемого API EWS**|**Элемент EWS**|**Свойство First класса для метода **FindItems** или операции **FindItem** ?**|**Чтение и запись или только чтение**|
|:-----|:-----|:-----|:-----|
|
  [Id](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.item.id%28v=exchg.80%29.aspx) <br/> |[Идентификатор](http://msdn.microsoft.com/library/3350b597-57a0-4961-8f44-8624946719b4%28Office.15%29.aspx) <br/> |Да  <br/> |Только для чтения  <br/> |
|[ParentFolderId](http://msdn.microsoft.com/en-us/library/office/microsoft.exchange.webservices.data.item.parentfolderid%28v=exchg.80%29.aspx) <br/> |[ParentFolderId](http://msdn.microsoft.com/library/258f4b1f-367e-4c7d-9c29-eb775a2398c7%28Office.15%29.aspx) <br/> |Да  <br/> |Только для чтения  <br/> |
|[ItemClass](http://msdn.microsoft.com/en-us/library/office/microsoft.exchange.webservices.data.item.itemclass%28v=exchg.80%29.aspx) <br/> |[ItemClass](http://msdn.microsoft.com/library/56020078-50b4-4880-894a-a9f234033cfb%28Office.15%29.aspx) <br/> |Да  <br/> |Чтение и запись  <br/> |
|[Тема](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.item.subject%28v=exchg.80%29.aspx) <br/> |[Тема](http://msdn.microsoft.com/library/c140d6c2-deb1-4f67-a908-9397197c4ae7%28Office.15%29.aspx) <br/> |Да  <br/> |Чтение и запись  <br/> |
|[Sensitivity](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.item.sensitivity%28v=exchg.80%29.aspx) <br/> |[Sensitivity](http://msdn.microsoft.com/library/d872423a-c26e-4675-9028-23361fb4a43d%28Office.15%29.aspx) <br/> |Да  <br/> |Только для чтения  <br/> |
|[Body](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.item.body%28v=exchg.80%29.aspx) <br/> |[Body](http://msdn.microsoft.com/library/7851ea9b-9f87-4adc-a26f-7a27df4a9bca%28Office.15%29.aspx) <br/> |Нет  <br/> |Чтение и запись  <br/> |
|[Вложения](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.item.attachments%28v=exchg.80%29.aspx) <br/> |[Вложения](http://msdn.microsoft.com/library/b470e614-34bb-44f0-8790-7ddbdcbbd29d%28Office.15%29.aspx) <br/> |Нет  <br/> |Чтение и запись  <br/> |
|[DateTimeReceived](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.item.datetimereceived%28v=exchg.80%29.aspx) <br/> |[DateTimeReceived](http://msdn.microsoft.com/library/8f489bd4-2434-4d0a-91fe-1b5ba7eb5765%28Office.15%29.aspx) <br/> |Да  <br/> |Только для чтения  <br/> |
|[Размер](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.item.size%28v=exchg.80%29.aspx) <br/> |[Размер](http://msdn.microsoft.com/library/966f4daf-c20e-49f8-aeb6-965f3e2da7c3%28Office.15%29.aspx) <br/> |Да  <br/> |Только для чтения  <br/> |
|[Категории](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.item.categories%28v=exchg.80%29.aspx) <br/> |[Категории](http://msdn.microsoft.com/library/d84d4927-b524-4e62-bf3d-1f12fec8c21a%28Office.15%29.aspx) <br/> |Нет  <br/> |Чтение и запись  <br/> |
|[Importance](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.item.importance%28v=exchg.80%29.aspx) <br/> |[Importance](http://msdn.microsoft.com/library/1557f59a-41f2-43fb-9ded-88f3ec5c76cb%28Office.15%29.aspx) <br/> |Да  <br/> |Чтение и запись  <br/> |
|[инреплито](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.item.inreplyto%28v=exchg.80%29.aspx) <br/> |[инреплито](http://msdn.microsoft.com/library/561b8941-1c26-4bbe-aa0f-b49ec8a79af5%28Office.15%29.aspx) <br/> |Да  <br/> |Чтение и запись  <br/> |
|[Отправлено](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.item.issubmitted%28v=exchg.80%29.aspx) <br/> |[Отправлено](http://msdn.microsoft.com/library/2399e27e-bd8c-46b6-a3aa-674842e098c9%28Office.15%29.aspx) <br/> |Да  <br/> |Только для чтения  <br/> |
|[Черновик](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.item.isdraft%28v=exchg.80%29.aspx) <br/> |[Черновик](http://msdn.microsoft.com/library/8b8d9cc9-a512-458a-94e4-af210ac83bd7%28Office.15%29.aspx) <br/> |Да  <br/> |Только для чтения  <br/> |
|[исфромме](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.item.isfromme%28v=exchg.80%29.aspx) <br/> |[исфромме](http://msdn.microsoft.com/library/d3c5fbf0-a95c-46e5-890f-953e50ac49d6%28Office.15%29.aspx) <br/> |Да  <br/> |Только для чтения  <br/> |
|[исресенд](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.item.isresend%28v=exchg.80%29.aspx) <br/> |[исресенд](http://msdn.microsoft.com/library/8f758b6b-dcee-4f95-9d39-e4be2bd92961%28Office.15%29.aspx) <br/> |Да  <br/> |Только для чтения  <br/> |
|[исунмодифиед](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.item.isunmodified%28v=exchg.80%29.aspx) <br/> |[исунмодифиед](http://msdn.microsoft.com/library/8f758b6b-dcee-4f95-9d39-e4be2bd92961%28Office.15%29.aspx) <br/> |Да  <br/> |Только для чтения  <br/> |
|[InternetMessageHeaders](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.item.internetmessageheaders%28v=exchg.80%29.aspx) <br/> |[InternetMessageHeaders](http://msdn.microsoft.com/library/4dcf8671-96df-4a2d-9836-7e8e3a67e0db%28Office.15%29.aspx) <br/> |Нет  <br/> |Только для чтения  <br/> |
|[датетимесент](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.item.datetimesent%28v=exchg.80%29.aspx) <br/> |[датетимесент](http://msdn.microsoft.com/library/81784ef3-8912-4d63-8502-73419a906999%28Office.15%29.aspx) <br/> |Да  <br/> |Только для чтения  <br/> |
|[DateTimeCreated](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.item.datetimecreated%28v=exchg.80%29.aspx) <br/> |[DateTimeCreated](http://msdn.microsoft.com/library/42ae0067-4688-49d9-93c5-c4dbeb54cee1%28Office.15%29.aspx) <br/> |Да  <br/> |Только для чтения  <br/> |
|[алловедреспонсеактионс](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.item.allowedresponseactions%28v=exchg.80%29.aspx) <br/> |[респонсеобжектс](http://msdn.microsoft.com/library/ad29e064-3f3d-4b7b-aa4c-9ec27326381d%28Office.15%29.aspx) <br/> |Нет  <br/> |Только для чтения  <br/> |
|[реминдердуеби](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.item.reminderdueby%28v=exchg.80%29.aspx) <br/> |[реминдердуеби](http://msdn.microsoft.com/library/e28a0485-86af-4a4e-a2ba-3ad2d4ebff6f%28Office.15%29.aspx) <br/> |Да  <br/> |Чтение и запись  <br/> |
|[Попамятка](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.item.isreminderset%28v=exchg.80%29.aspx) <br/> |[реминдериссет](http://msdn.microsoft.com/library/fa366afe-77a0-4c14-9edb-ffc9699131ba%28Office.15%29.aspx) <br/> |Да  <br/> |Чтение и запись  <br/> |
|[ReminderMinutesBeforeStart](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.item.reminderminutesbeforestart%28v=exchg.80%29.aspx) <br/> |[ReminderMinutesBeforeStart](http://msdn.microsoft.com/library/65ea14bc-5f19-48cc-aef1-46227e06f5f5%28Office.15%29.aspx) <br/> |Да  <br/> |Чтение и запись  <br/> |
|[дисплайкк](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.item.displaycc%28v=exchg.80%29.aspx) <br/> |[дисплайкк](http://msdn.microsoft.com/library/af386e06-80f3-42c7-8b3c-1f7993c49d10%28Office.15%29.aspx) <br/> |Да  <br/> |Только для чтения  <br/> |
|[дисплайто](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.item.displayto%28v=exchg.80%29.aspx) <br/> |[дисплайто](http://msdn.microsoft.com/library/16a0b22d-063b-417c-8aba-efcf9490b072%28Office.15%29.aspx) <br/> |Да  <br/> |Только для чтения  <br/> |
|[HasAttachments](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.item.hasattachments%28v=exchg.80%29.aspx) <br/> |[HasAttachments](http://msdn.microsoft.com/library/538b7a85-11d7-4daa-8458-09b540760e8b%28Office.15%29.aspx) <br/> |Да  <br/> |Только для чтения  <br/> |
|[Culture](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.item.culture%28v=exchg.80%29.aspx) <br/> |[Culture](http://msdn.microsoft.com/library/71bd62c6-3fec-48db-9a5e-02121e9bc20b%28Office.15%29.aspx) <br/> |Да  <br/> |Чтение и запись  <br/> |
|[еффективеригхтс](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.item.effectiverights%28v=exchg.80%29.aspx) <br/> |[еффективеригхтс](http://msdn.microsoft.com/library/bf5278eb-3a1a-4d27-9d16-b8be043bb023%28Office.15%29.aspx) <br/> |Да  <br/> |Только для чтения  <br/> |
|[ластмодифиеднаме](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.item.lastmodifiedname%28v=exchg.80%29.aspx) <br/> |[ластмодифиеднаме](http://msdn.microsoft.com/library/4f1a90c1-e27e-4e16-93c3-e79d4cb720d1%28Office.15%29.aspx) <br/> |Да  <br/> |Только для чтения  <br/> |
|[LastModifiedTime](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.item.lastmodifiedtime%28v=exchg.80%29.aspx) <br/> |[LastModifiedTime](http://msdn.microsoft.com/library/6db2cabc-e7f4-4d71-962b-789de6a192a4%28Office.15%29.aspx) <br/> |Да  <br/> |Только для чтения  <br/> |
|[Связанный](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.item.isassociated%28v=exchg.80%29.aspx) <br/> |[Связанный](http://msdn.microsoft.com/library/637f0798-6680-487f-bcbf-aaddc4a74186%28Office.15%29.aspx) <br/> |Да  <br/> |Чтение и запись  <br/> |
|[вебклиентреадформкуеристринг](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.item.webclientreadformquerystring%28v=exchg.80%29.aspx) <br/> |[вебклиентреадформкуеристринг](http://msdn.microsoft.com/library/13e8871a-32a6-4bb9-9493-864c4c07efff%28Office.15%29.aspx) <br/> |Да  <br/> |Только для чтения  <br/> |
|[вебклиентедитформкуеристринг](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.item.webclienteditformquerystring%28v=exchg.80%29.aspx) <br/> |[вебклиентедитформкуеристринг](http://msdn.microsoft.com/library/9e571021-d58f-424b-8db2-48cf683533dc%28Office.15%29.aspx) <br/> |Да  <br/> |Только для чтения  <br/> |
|[ConversationId](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.item.conversationid%28v=exchg.80%29.aspx) <br/> |[ConversationId](http://msdn.microsoft.com/library/d5f1ddb3-9af3-4677-a6ba-111b304a951e%28Office.15%29.aspx) <br/> |Да  <br/> |Только для чтения  <br/> |
|[Флаг](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.item.flag%28v=exchg.80%29.aspx) <br/> |[Флаг](http://msdn.microsoft.com/library/7b47bc74-a60d-4308-8674-5d52444a1753%28Office.15%29.aspx) <br/> |Да  <br/> |Чтение и запись  <br/> |
|[инстанцекэй](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.item.instancekey%28v=exchg.80%29.aspx) <br/> |[инстанцекэй](http://msdn.microsoft.com/library/bb4dbe9b-aea0-4527-b7d6-e928066caf38%28Office.15%29.aspx) <br/> |Да  <br/> |Только для чтения  <br/> |
|[ентитекстрактионресулт](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.item.entityextractionresult%28v=exchg.80%29.aspx) <br/> |[ентитекстрактионресулт](http://msdn.microsoft.com/library/643b99ab-ff90-4411-864c-1077623028d6%28Office.15%29.aspx) <br/> |Нет  <br/> |Только для чтения  <br/> |
|[Sender](http://msdn.microsoft.com/en-us/library/office/microsoft.exchange.webservices.data.emailmessage.sender%28v=exchg.80%29.aspx) <br/> |[Sender](http://msdn.microsoft.com/library/26d1a46e-e1d3-44b8-a02d-fa6f83aa5cda%28Office.15%29.aspx) <br/> |Да  <br/> |Чтение и запись  <br/> |
|[ToRecipients](http://msdn.microsoft.com/en-us/library/office/microsoft.exchange.webservices.data.emailmessage.torecipients%28v=exchg.80%29.aspx) <br/> |[ToRecipients](http://msdn.microsoft.com/library/72dc3be8-30bb-4ae1-acf4-fb94ff490631%28Office.15%29.aspx) <br/> |Нет  <br/> |Только для чтения  <br/> |
|[CcRecipients](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.emailmessage.ccrecipients%28v=exchg.80%29.aspx) <br/> |[CcRecipients](http://msdn.microsoft.com/library/5c20ec3a-0bee-4e67-b220-586ed0d601c9%28Office.15%29.aspx) <br/> |Нет  <br/> |Только для чтения  <br/> |
|[BccRecipients](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.emailmessage.bccrecipients%28v=exchg.80%29.aspx) <br/> |[BccRecipients](http://msdn.microsoft.com/library/c4e05168-d36b-4740-a526-4b7da53553c1%28Office.15%29.aspx) <br/> |Нет  <br/> |Только для чтения  <br/> |
|[исреадрецеиптрекуестед](http://msdn.microsoft.com/en-us/library/office/microsoft.exchange.webservices.data.emailmessage.isreadreceiptrequested%28v=exchg.80%29.aspx) <br/> |[исреадрецеиптрекуестед](http://msdn.microsoft.com/library/7ab6edd5-c7ed-4701-8de3-d7dc7ecfa9c2%28Office.15%29.aspx) <br/> |Да  <br/> |Чтение и запись  <br/> |
|[исделиверирецеиптрекуестед](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.emailmessage.isdeliveryreceiptrequested%28v=exchg.80%29.aspx) <br/> |[исделиверирецеиптрекуестед](http://msdn.microsoft.com/library/97776b7e-942c-4663-8277-165d64364daa%28Office.15%29.aspx) <br/> |Да  <br/> |Чтение и запись  <br/> |
|[ConversationIndex](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.emailmessage.conversationindex%28v=exchg.80%29.aspx) <br/> |[ConversationIndex](http://msdn.microsoft.com/library/fdf47e22-8d93-4ae4-883b-0c9f07f48724%28Office.15%29.aspx) <br/> |Да  <br/> |Только для чтения  <br/> |
|[ConversationTopic](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.emailmessage.conversationtopic%28v=exchg.80%29.aspx) <br/> |[ConversationTopic](http://msdn.microsoft.com/library/46cacf42-4039-4c8a-9b20-c42cdd9f2760%28Office.15%29.aspx) <br/> |Да  <br/> |Только для чтения  <br/> |
|[From](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.emailmessage.from%28v=exchg.80%29.aspx) <br/> |[From](http://msdn.microsoft.com/library/5a52d644-3677-4049-874c-12bd5c3080dc%28Office.15%29.aspx) <br/> |Да  <br/> |Чтение и запись  <br/> |
|[InternetMessageId](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.emailmessage.internetmessageid%28v=exchg.80%29.aspx) <br/> |[InternetMessageId](http://msdn.microsoft.com/library/a5a9563f-e761-4658-9957-0e13566f6a35%28Office.15%29.aspx) <br/> |Да  <br/> |Только для чтения  <br/> |
|[IsRead](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.emailmessage.isread%28v=exchg.80%29.aspx) <br/> |[IsRead](http://msdn.microsoft.com/library/161455d5-a870-4c99-b2eb-c759c538f1bc%28Office.15%29.aspx) <br/> |Да  <br/> |Чтение и запись  <br/> |
|[исреспонсерекуестед](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.emailmessage.isresponserequested%28v=exchg.80%29.aspx) <br/> |[исреспонсерекуестед](http://msdn.microsoft.com/library/8cb874ed-a538-4de6-ab22-2631092dcdd0%28Office.15%29.aspx) <br/> |Да  <br/> |Чтение и запись  <br/> |
|[ReplyTo](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.emailmessage.replyto%28v=exchg.80%29.aspx) <br/> |[ReplyTo](http://msdn.microsoft.com/library/6b6ae792-e2c4-4aa0-95cb-b49b446f1e08%28Office.15%29.aspx) <br/> |Нет  <br/> |Только для чтения  <br/> |
|[References](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.emailmessage.references%28v=exchg.80%29.aspx) <br/> |[References](http://msdn.microsoft.com/library/d78f9a48-cd24-452f-af65-4c01933227ce%28Office.15%29.aspx) <br/> |Да  <br/> |Чтение и запись  <br/> |
|[рецеиведби](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.emailmessage.receivedby%28v=exchg.80%29.aspx) <br/> |[рецеиведби](http://msdn.microsoft.com/library/ac84c9c5-d2fe-4b6f-bf4d-0444131d835b%28Office.15%29.aspx) <br/> |Да  <br/> |Только для чтения  <br/> |
|[рецеиведрепресентинг](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.emailmessage.receivedrepresenting%28v=exchg.80%29.aspx) <br/> |[рецеиведрепресентинг](http://msdn.microsoft.com/library/1157b042-6dce-4cdc-9700-e22b749da39f%28Office.15%29.aspx) <br/> |Да  <br/> |Только для чтения  <br/> |
   
## <a name="other-properties-and-elements-for-email-messages"></a>Другие свойства и элементы для сообщений электронной почты
<a name="bk_notfirstclass"> </a>

Не все важные свойства и элементы электронной почты являются свойствами и элементами первого класса. Чтобы получить другие свойства или элементы, необходимо добавить их в набор [свойств](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.propertyset%28v=exchg.80%29.aspx) , если вы используете управляемый API EWS или используете путь к свойству, чтобы добавить их в вызов операции EWS. Например, чтобы получить текст текста и содержимое MIME сообщения, создайте набор **свойств** , как показано в методе **BIND** или **Load** . 
  
```cs
PropertySet(BasePropertySet.IdOnly, ItemSchema.TextBody, ItemSchema.MimeContent);
```

Если вы используете EWS, добавьте элементы в элемент [аддитионалпропертиес](http://msdn.microsoft.com/library/7a269aed-dcfd-4c3e-9e14-094e53828101%28Office.15%29.aspx) в запросе операции **GetItem** , как показано ниже. 
  
```XML
<t:AdditionalProperties>
    <t:FieldURI FieldURI="item:TextBody" />
    <t:FieldURI FieldURI="item:MimeContent" />
</t:AdditionalProperties>
```

 Свойства **EmailMessage** , унаследованные из объекта [СЕРВИЦЕОБЖЕКТ](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.serviceobject%28v=exchg.80%29.aspx) управляемого API EWS, не могут быть включены в набор свойств для метода **BIND** ; Однако все свойства **сервицеобжект** читаются в объекте **EmailMessage** и извлекаются методом **BIND** . 
  
**Таблица 2. Другие свойства и элементы электронной почты**

|**Свойство управляемого API EWS**|**Элемент EWS**|**Чтение и запись или только чтение**|
|:-----|:-----|:-----|
|[арчиветаг](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.item.archivetag%28v=exchg.80%29.aspx) <br/> |[арчиветаг](http://msdn.microsoft.com/library/c4cb0718-37cd-41aa-86e7-b492c4bb86aa%28Office.15%29.aspx) <br/> |Чтение и запись  <br/> |
|[ExtendedProperties](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.item.extendedproperties%28v=exchg.80%29.aspx) <br/> |[ExtendedProperty](http://msdn.microsoft.com/library/f9701409-b620-4afe-b9ee-4c1e95507af7%28Office.15%29.aspx) <br/> |Только для чтения  <br/> |
|[IconIndex](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.item.iconindex%28v=exchg.80%29.aspx) <br/> |[IconIndex](http://msdn.microsoft.com/library/92020822-2a86-4dfc-aee1-3067af4d4edf%28Office.15%29.aspx) <br/> |Только для чтения  <br/> |
|[Присоединение](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.item.isattachment%28v=exchg.80%29.aspx) <br/> |Недоступно  <br/> |Только для чтения  <br/> |
|[IsDirty](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.serviceobject.isdirty%28v=exchg.80%29.aspx) <br/> |Недоступно  <br/> |Только для чтения  <br/> |
|[IsNew](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.item.isnew%28v=exchg.80%29.aspx) <br/> |Недоступно  <br/> |Только для чтения  <br/> |
|[Элемент](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.serviceobject.item%28v=exchg.80%29.aspx) <br/> |[Элемент](http://msdn.microsoft.com/library/4dfe8f48-e7b4-444d-bdf9-a34e180f598b%28Office.15%29.aspx) <br/> |Только для чтения  <br/> |
|[Сохранитьmimecontent](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.item.mimecontent%28v=exchg.80%29.aspx) <br/> |[Сохранитьmimecontent](http://msdn.microsoft.com/library/4f472a08-5653-4c54-ba65-831dfe32f20f%28Office.15%29.aspx) <br/> |Только для чтения  <br/> |
|Недоступно  <br/> |[MimeContentUTF8](http://msdn.microsoft.com/library/31544c95-5231-4b57-958c-2a689464d29b%28Office.15%29.aspx) <br/> |Только для чтения  <br/> |
|[нормализедбоди](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.item.normalizedbody%28v=exchg.80%29.aspx) <br/> |[нормализедбоди](http://msdn.microsoft.com/library/bfb813e4-642d-4f1b-9e91-1fee89dbd083%28Office.15%29.aspx) <br/> |Только для чтения  <br/> |
|[полицитаг](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.item.policytag%28v=exchg.80%29.aspx) <br/> |[полицитаг](http://msdn.microsoft.com/library/fa4b1447-dc7b-47ad-a677-78fcee443dc6%28Office.15%29.aspx) <br/> |Чтение и запись  <br/> |
|[Предварительная версия](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.item.preview%28v=exchg.80%29.aspx) <br/> |[Предварительная версия](http://msdn.microsoft.com/library/5d33f557-c9d5-4f7f-82c0-d800412f8b7e%28Office.15%29.aspx) <br/> |Чтение и запись  <br/> |
|[ретентиондате](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.item.retentiondate%28v=exchg.80%29.aspx) <br/> |[ретентиондате](http://msdn.microsoft.com/library/0c1df5e2-b56a-4947-a047-2b73b32e5fb7%28Office.15%29.aspx) <br/> |Только для чтения  <br/> |
|[схема](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.serviceobject.schema%28v=exchg.80%29.aspx); <br/> |Недоступно  <br/> |Только для чтения  <br/> |
|[Service](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.serviceobject.service%28v=exchg.80%29.aspx) (Служба) <br/> |Недоступно  <br/> |Только для чтения  <br/> |
|[сторинтрид](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.item.storeentryid%28v=exchg.80%29.aspx) <br/> |[сторинтрид](http://msdn.microsoft.com/library/f536e264-8c4d-4cc5-bab8-22a4fa38de39%28Office.15%29.aspx) <br/> |Только для чтения  <br/> |
|[текстбоди](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.item.textbody%28v=exchg.80%29.aspx) <br/> |[текстбоди](http://msdn.microsoft.com/library/bd0c0bce-3e7c-47c7-af7f-5ee5f5ad9820%28Office.15%29.aspx) <br/> |Только для чтения  <br/> |
|[UniqueBody](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.item.uniquebody%28v=exchg.80%29.aspx) <br/> |[UniqueBody](http://msdn.microsoft.com/library/06bc95d7-121c-433b-bd27-c2b0eb8c011f%28Office.15%29.aspx) <br/> |Только для чтения  <br/> |
   
## <a name="see-also"></a>См. также


- [Электронная почта и веб-службах Exchange](email-and-ews-in-exchange.md)
    
- [Свойства и расширенные свойства в веб-службах Exchange](properties-and-extended-properties-in-ews-in-exchange.md)
    
- [Наборы свойств и формы ответа в веб-службах Exchange](property-sets-and-response-shapes-in-ews-in-exchange.md)
    
- [Работа с элементами почтовых ящиков Exchange с помощью веб-служб Exchange](how-to-work-with-exchange-mailbox-items-by-using-ews-in-exchange.md)
    

