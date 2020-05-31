---
title: Новые возможности в веб-службах EWS и других веб-службах в Exchange
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
localization_priority: Normal
ms.assetid: aff6328f-cff1-42a6-9a4d-ea4d2d0461cf
description: Узнайте о новых возможностях веб-служб Exchange и веб-службах Exchange и управляемом API EWS.
ms.openlocfilehash: 9e848babc96707152be767f42b561a587fc6cff0
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/25/2018
ms.locfileid: "19761255"
---
# <a name="whats-new-in-ews-and-other-web-services-in-exchange"></a>Новые возможности в веб-службах EWS и других веб-службах в Exchange

Узнайте о новых возможностях веб-служб Exchange и веб-службах Exchange и управляемом API EWS.
  
Веб-службы в Exchange обновлены с добавлением новых функций. 
  
**Таблица 1. Новые возможности веб-служб в Exchange Online, Exchange 2013 и управляемом API EWS**

|Компонент|Реализовано в Exchange Online|Реализовано в Exchange 2013|Реализовано в управляемом API EWS|
|:-----|:-----:|:-----:|:-----:|
|[Обнаружение электронных данных](#eDisc) <br/> |Да  <br/> |Да  <br/> |Да  <br/> |
|[Архивация](#arch) <br/> |Да  <br/> |Да  <br/> |Да  <br/> |
|[Фиктивные пользователи](#personas) <br/> |Да  <br/> |Да  <br/> |Нет  <br/> |
|[Единая база контактов](#unified) <br/> |Да  <br/> |Да  <br/> |Нет  <br/> |
|[Политики хранения](#retentionpolicy) <br/> |Да  <br/> |Да  <br/> |Да  <br/> |
|[Фотографии пользователя](#userphoto) <br/> |Да  <br/> |Да  <br/> |Нет  <br/> |
|[Почтовые приложения для управления Outlook](#ewsmailapps) <br/> |Да  <br/> |Да  <br/> |Да  <br/> |
|[Предложение нового времени собрания](#propose) <br/> |Да  <br/> |Нет  <br/> |Нет  <br/> |

<a name="eDisc"> </a>

## <a name="ediscovery-in-ews"></a>Обнаружение электронных данных в EWS

Обнаружение электронных данных — это веб-служба федеративных запросов, которая позволяет внешним приложениям, например SharePoint 2013, выполнять запросы данных Exchange. Обнаружение состоит из нескольких этапов, в том числе определения и сохранения данных ключей, отбора и просмотра данных, а также создания данных в суд. запросы eDiscovery упрощают процесс обнаружения, предоставляя единый рабочий процесс обнаружения в Exchange и SharePoint.
  
**Таблица 2. Операции служб EWS и методы управляемого API EWS для работы с обнаружением электронных данных**

|**Имя операции**|**Метод управляемого API EWS**|**Описание**|
|:-----|:-----|:-----|
|[Операция GetDiscoverySearchConfiguration](http://msdn.microsoft.com/library/8a54a6dc-110c-4972-a8bc-5ddb43c4b857%28Office.15%29.aspx) <br/> |[ExchangeService. GetDiscoverySearchConfiguration ()](http://msdn.microsoft.com/en-us/library/jj670206%28v=exchg.80%29.aspx) <br/> |Получает сведения о конфигурации для удержаний на месте, сохраненных поисков и почтовых ящиков, которые включены для поиска при обнаружении.  <br/> |
|[Операция GetHoldOnMailboxes](http://msdn.microsoft.com/library/9157f329-80b4-4cd0-a158-378064966ae6%28Office.15%29.aspx) <br/> |[ExchangeService. GetHoldOnMailboxes ()](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.exchangeservice.getholdonmailboxes%28v=exchg.80%29.aspx) <br/> |Получает состояние хранения на основе запроса, которое задается с помощью операции **SetHoldOnMailboxes** .  <br/> |
|[Операция GetNonIndexableItemDetails](http://msdn.microsoft.com/library/9279c3ad-f7c8-4bbc-b0a7-2c78416cb39a%28Office.15%29.aspx) <br/> |[ExchangeService. GetNonIndexableItemDetails ()](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.exchangeservice.getnonindexableitemdetails%28v=exchg.80%29.aspx) <br/> |Получает сведения о элементах, которые не удается индексировать. Это относится только к идентификатору элемента, к коду ошибки, описанию ошибки, при попытке индексирования элемента и дополнительным сведениям об элементе.  <br/> |
|[Операция GetNonIndexableItemStatistics](http://msdn.microsoft.com/library/ed077877-9d98-4434-b8b6-a4a905e7f7a6%28Office.15%29.aspx) <br/> |[ExchangeService. GetNonIndexableItemStatistics ()](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.exchangeservice.getnonindexableitemstatistics%28v=exchg.80%29.aspx) <br/> |Получает количество элементов, которые не удается индексировать в почтовом ящике.  <br/> |
|[Операция GetSearchableMailboxes](http://msdn.microsoft.com/library/47f8ff57-4835-4d2d-9136-44afb31a4cbe%28Office.15%29.aspx) <br/> |[ExchangeService. GetSearchableMailboxes ()](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.exchangeservice.getsearchablemailboxes%28v=exchg.80%29.aspx) <br/> |Получает список почтовых ящиков, у которых у клиента есть разрешение на поиск и выполнение обнаружения электронных данных.  <br/> |
|[Операция SearchMailboxes](http://msdn.microsoft.com/library/8a67c1d8-d021-4e68-aa62-35f7d9c2edc7%28Office.15%29.aspx) <br/> |[ExchangeService. SearchMailboxes ()](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.exchangeservice.searchmailboxes%28v=exchg.80%29.aspx) <br/> |Ищет элементы в определенных почтовых ящиках, которые совпадают с ключевыми словами запроса.  <br/> |
|[Операция SetHoldOnMailboxes](http://msdn.microsoft.com/library/9015a0d8-3495-461b-aa79-797d23169585%28Office.15%29.aspx) <br/> |[ExchangeService. SetHoldOnMailboxes ()](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.exchangeservice.setholdonmailboxes%28v=exchg.80%29.aspx) <br/> |Задает для элементов удержание на основе запроса.  <br/> |

<a name="arch"> </a>

## <a name="archiving-in-ews"></a>Архивация в EWS

Архивные почтовые ящики это дополнительные почтовые ящики, связанные с пользователем. Архивные почтовые ящики обычно используются для управления пределами хранилища электронной почты. Например, старые элементы электронной почты можно периодически перемещать из папки "Входящие" в архивный почтовый ящик. 
  
Exchange вводит две новые операции EWS, которые можно использовать для архивации набора почтовых элементов из основного почтового ящика. Архивирование элементов папки "Входящие" таким способом сохраняет иерархию папок для элементов. Кроме того, архивные почтовые ящики теперь можно хранить локально на клиенте или удаленно, как правило, как правило, непрозрачным для пользователя, используя путь к папке для ссылки на содержимое архива.
  
**Таблица 3. Операции служб EWS и методы управляемого API EWS для работы с архивацией**

|**Имя операции**|**Метод управляемого API EWS**|**Описание**|
|:-----|:-----|:-----|
|[Операция ArchiveItem](http://msdn.microsoft.com/library/1af216b3-13ea-498e-b4fc-23513755d731%28Office.15%29.aspx) <br/> |[ExchangeService. Арчивеитемс ()](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.exchangeservice.archiveitems%28v=exchg.80%29.aspx) <br/> |Перемещает элемент из основного почтового ящика в архивный.  <br/> |
|[Операция CreateFolderPath](http://msdn.microsoft.com/library/5a10aa5e-3f25-4ec3-a0b9-284c30918a1f%28Office.15%29.aspx) <br/> |Не реализовано.  <br/> |Создает иерархию папок в основном или архивном почтовом ящике.  <br/> |

<a name="personas"> </a>

## <a name="personas-in-ews"></a>Персонажи в EWS

*Пользователь* — это набор данных, связанных с отдельным пользователем. Данные могут поступать из одного или нескольких источников и сопоставлены с пользователями с помощью общего идентификатора ссылки. Пользователи в EWS позволяют связывать, искать, просматривать и получать сведения о человеке из нескольких источников, а также организовывать их в одну логическую сущность. Пользователи отличаются от контактов в том, что контакт представляет собой коллекцию данных из одного источника, связанного с отдельным пользователем; Например, личный контакт Outlook или запись в глобальном списке адресов (GAL). 
  
Управляемый API EWS не реализует эту функцию.
  
> [!NOTE]
> Единое хранилище контактов также предоставляет функциональные возможности для пользователей с помощью операций, поддерживающих эту функцию. 
  
**Таблица 4. Операции EWS для работы с пользователями**

|**Имя операции**|**Описание**|
|:-----|:-----|
|[Операция FindPeople](http://msdn.microsoft.com/library/446106b7-ff2d-4107-90c1-29f4d38ba128%28Office.15%29.aspx) <br/> |Возвращает все объекты персоны из указанной папки контактов или получает все контакты, которые совпадают с указанной строкой запроса.  <br/> |
|[Операция GetPersona](http://msdn.microsoft.com/library/e2146df0-53d0-4caf-9758-b600bbc14b6a%28Office.15%29.aspx) <br/> |Получает пользователя.  <br/> |

<a name="unified"> </a>

## <a name="unified-contact-store-in-ews"></a>Единое хранилище контактов в EWS

Единое хранилище контактов — это функция, обеспечивающая единообразное взаимодействие между продуктами Office и которая выступает в качестве точки интеграции для сторонних приложений для использования одного хранилища контактов. Она позволяет пользователям и приложениям хранить, управлять и получать доступ к контактным данным и делать их глобально доступными для Lync, Exchange 2013, Outlook, Outlook Web App и любого другого приложения, реализующего доступ к единому хранилищу контактов. Exchange это хранилище контактов для единого хранилища контактов. 
  
Управляемый API EWS не реализует эту функцию.
  
**Таблица 5. Операции EWS для работы с единым хранилищем контактов**

|**Имя операции**|**Описание**|
|:-----|:-----|
|[Операция AddNewImContactToGroup](http://msdn.microsoft.com/library/0cb5525f-faa3-48f1-9551-df55ffc26f46%28Office.15%29.aspx) <br/> |Добавляет новый контакт для обмена мгновенными сообщениями в группу. Единое хранилище контактов может содержать не более 1000 контактов.  <br/> |
|[Операция AddImContactToGroup](http://msdn.microsoft.com/library/376acc42-2684-4596-aca1-82a4a10865c9%28Office.15%29.aspx) <br/> |Добавляет существующий контакт для обмена мгновенными сообщениями в группу. Единое хранилище контактов может содержать не более 1000 контактов.  <br/> |
|[Операция AddImGroup](http://msdn.microsoft.com/library/6df6e504-b7c8-4773-b10f-ffa5defac229%28Office.15%29.aspx) <br/> |Добавление новой группы для обмена мгновенными сообщениями. Единое хранилище контактов может содержать не более 64 групп.  <br/> |
|[Операция AddNewTelUriContactToGroup](http://msdn.microsoft.com/library/c9688ce8-2465-45bb-8bd2-94b32ed4885c%28Office.15%29.aspx) <br/> |Добавляет новый контакт в группу на основе номера телефона контакта.  <br/> |
|[Операция AddDistributionGroupToImList](http://msdn.microsoft.com/library/5aa9bec8-71cf-4a6e-8ec8-b4965b40fd4a%28Office.15%29.aspx) <br/> |Добавление новой группы списка рассылки. Единое хранилище контактов может содержать не более 64 групп.  <br/> |
|[Операция GetImItemList](http://msdn.microsoft.com/library/e31d14e1-0c1f-4b69-98b7-157d59c13698%28Office.15%29.aspx) <br/> |Получает список групп для IM и фиктивных пользователей, включающих контакты для IM.  <br/> |
|[Операция GetImItems](http://msdn.microsoft.com/library/51186691-46d2-4d5c-b8bc-4ee2bb20fbe7%28Office.15%29.aspx) <br/> |Получает сведения об указанных группах IM и пользователях контактов для обмена мгновенными сообщениями.  <br/> |
|[Операция RemoveContactFromImList](http://msdn.microsoft.com/library/28ec96c3-45af-48ff-9f17-718a527dc0ad%28Office.15%29.aspx) <br/> |Удаляет указанного контакта из всех групп IM.  <br/> |
|[Операция RemoveImContactFromGroup](http://msdn.microsoft.com/library/a190bbec-c71b-4e6a-880b-55854c724d8c%28Office.15%29.aspx) <br/> |Удаляет контакт для обмена мгновенными сообщениями из группы.  <br/> |
|[Операция RemoveDistributionGroupFromImList](http://msdn.microsoft.com/library/252bddf2-98b6-4824-b548-2fba2bda5384%28Office.15%29.aspx) <br/> |Удаляет указанную группу списка рассылки для обмена мгновенными сообщениями.  <br/> |
|[Операция RemoveImGroup](http://msdn.microsoft.com/library/5e788016-68e0-4a3f-9243-03f6b6c6b389%28Office.15%29.aspx) <br/> |Удаляет указанную группу мгновенных сообщений.  <br/> |
|[Операция SetImGroup](http://msdn.microsoft.com/library/2d48aa07-8152-4c3d-a519-061253e80174%28Office.15%29.aspx) <br/> |Изменение отображаемого имени группы.  <br/> |

<a name="retentionpolicy"> </a>
  
## <a name="retention-policies-in-ews"></a>Политики хранения в EWS

Политики хранения — это политики, используемые в Exchange для группирования одного или нескольких тегов хранения, для применения параметров хранения к папкам или отдельным элементам, таким как сообщения электронной почты и голосовой почты, а также для применения параметров хранения к почтовому ящику.
  
Exchange содержит три типа тегов хранения:
  
- Теги политики по умолчанию, применяемые к элементам почтовых ящиков, для которых не применяется другой тип тега хранения.
    
- Теги политики системных папок, которые применяются к папкам по умолчанию, таким как папка "Входящие".
    
- Личные теги, которые пользователь может применять к создаваемым папкам или отдельным элементам.
    
Почтовому ящику может быть назначена только одна политика хранения, но эта политика может иметь один или несколько тегов хранения различных типов, связанных с ним. Теги хранения можно связать с политикой хранения или удалить из нее в любое время. Служба EWS в Exchange предоставляет новую операцию, [GetUserRetentionPolicyTags](http://msdn.microsoft.com/library/57c6ff23-5c2c-42ee-824b-5a1b6dafab8c%28Office.15%29.aspx), а управляемый API EWS реализует новый метод, [ExchangeService. GetUserRetentionPolicyTags ()](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.exchangeservice.getuserretentionpolicytags%28v=exchg.80%29.aspx), который предоставляет список всех тегов, связанных с политикой хранения. Вы можете задавать и получать Теги политики хранения для элементов и папок с помощью операций **CreateItem**, **CreateFolder**, **UpdateItem**, **операцию UpdateFolder**, **GetItem и GetItem**. **GetFolder** 

<a name="userphoto"> </a>

## <a name="requesting-user-photos"></a>Запрос фотографий пользователей

Вы можете запрашивать фотографии пользователей с сервера Exchange Server с помощью одной из двух реализаций [операции GetUserPhoto](http://msdn.microsoft.com/library/f6e8143d-4235-428e-8f9c-ab6e9b1cfa6e%28Office.15%29.aspx): [REST](how-to-get-user-photos-by-using-ews-in-exchange.md) или SOAP. Конечная точка REST использует стандартный запрос **Get** HTTPS для получения фотографии пользователя. Служба возвратит фотографию пользователя, сохраненную в Exchange, или фотографию из доменных служб Active Directory (AD DS). 
  
Управляемый API EWS не реализует эту функцию. Тем не менее, вы можете использовать управляемый API EWS, чтобы вернуть фотографии пользователей, которые хранятся в почтовом ящике, получив фотографию, вложенную в контакт.

<a name="blocksender"> </a>

## <a name="block-senders-and-mark-email-as-junk-in-ews"></a>Блокировка отправителей и пометка электронной почты как нежелательного в EWS

Теперь вы можете заблокировать отправители и пометить сообщение как нежелательное с помощью новой [операции MarkAsJunk](http://msdn.microsoft.com/library/1f71f04d-56a9-4fee-a4e7-d1034438329e%28Office.15%29.aspx) в службах EWS или метода [ExchangeService. MarkAsJunk ()](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.exchangeservice.markasjunk%28v=exchg.80%29.aspx) в управляемом API EWS. 

<a name="ewsmailapps"> </a>

## <a name="mail-apps-for-outlook"></a>Почтовые приложения для Outlook

Теперь в EWS включена поддержка управления почтовыми приложениями для Outlook. 
  
**Таблица 6. Операции служб EWS и методы управляемого API EWS для работы с почтовыми приложениями для Outlook**

|**Имя операции**|**Метод управляемого API EWS**|**Описание**|
|:-----|:-----|:-----|
|[Операция DisableApp](http://msdn.microsoft.com/library/211731a3-2470-49af-bda3-1ddfc15a8e46%28Office.15%29.aspx) <br/> |[ExchangeService. DisableApp ()](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.exchangeservice.disableapp%28v=exchg.80%29.aspx) <br/> |Отключает установленное приложение.  <br/> |
|[Операция GetAppManifests](http://msdn.microsoft.com/library/21a4987c-c24d-4a6e-ace4-e81edcda6303%28Office.15%29.aspx) <br/> |[ExchangeService. GetAppManifests ()](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.exchangeservice.getappmanifests%28v=exchg.80%29.aspx) <br/> |Получает манифесты приложения для почтового ящика.  <br/> |
|[Операция GetAppMarketplaceUrl](http://msdn.microsoft.com/library/2c016fc3-0e13-4624-9a5b-d3e84577a860%28Office.15%29.aspx) <br/> |[ExchangeService. GetAppMarketplaceUrl ()](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.exchangeservice.getappmarketplaceurl%28v=exchg.80%29.aspx) <br/> |Получает URL-адрес Marketplace для приложения.  <br/> |
|[Операция GetClientAccessToken](http://msdn.microsoft.com/library/086876cc-e22c-4e89-89f9-19e78af51217%28Office.15%29.aspx) <br/> |[ExchangeService. GetClientAccessToken ()](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.exchangeservice.getclientaccesstoken%28v=exchg.80%29.aspx) <br/> |Получает маркеры клиентского доступа.  <br/> |
|[Операция InstallApp](http://msdn.microsoft.com/library/596eae95-3e78-489a-8bb2-d2dd4a026405%28Office.15%29.aspx) <br/> |[ExchangeService. InstallApp ()](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.exchangeservice.installapp%28v=exchg.80%29.aspx) <br/> |Устанавливает приложение для почтового ящика.  <br/> |
|[Операция UninstallApp](http://msdn.microsoft.com/library/7707aa6a-381d-43f7-a454-54f6343ed127%28Office.15%29.aspx) <br/> |[ExchangeService. UninstallApp](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.exchangeservice.uninstallapp%28v=exchg.80%29.aspx) <br/> |Удаляет приложение из почтового ящика.  <br/> |

<a name="propose"> </a>

## <a name="propose-new-meeting-time"></a>Предложение нового времени собрания

Функция "предложить новое время" была введена в версии 15.00.0800.007 Exchange. Это позволяет участникам собрания [предлагать новое время проведения собрания](how-to-propose-a-new-meeting-time-by-using-ews-in-exchange.md) организатору собрания. 
  
Управляемый API EWS не реализует эту функцию.
  
## <a name="see-also"></a>См. также

- [Сведения об управляемом API EWS, EWS и веб-службах в Exchange](explore-the-ews-managed-api-ews-and-web-services-in-exchange.md)  
- [Общие сведения о разработке клиента EWS для Exchange](ews-client-design-overview-for-exchange.md)
- [Приложения электронной почты для Outlook и служб EWS в Exchange](mail-apps-for-outlook-and-ews-in-exchange.md)
- [Архивация в веб-служб Exchange в Exchange](archiving-in-ews-in-exchange.md)
- [обнаружение электронных данных в веб-службах Exchange](ediscovery-in-ews-in-exchange.md)
- [Пользователи и контакты в EWS для Exchange](people-and-contacts-in-ews-in-exchange.md)
    

