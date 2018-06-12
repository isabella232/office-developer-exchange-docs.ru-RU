---
title: Новые возможности веб-служб Exchange и другие веб-службы в Exchange
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
localization_priority: Normal
ms.assetid: aff6328f-cff1-42a6-9a4d-ea4d2d0461cf
description: Узнайте, новые возможности в веб-служб Exchange и веб-службы в Exchange и управляемый API веб-служб Exchange.
ms.openlocfilehash: 9e848babc96707152be767f42b561a587fc6cff0
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/11/2018
ms.locfileid: "19761255"
---
# <a name="whats-new-in-ews-and-other-web-services-in-exchange"></a>Новые возможности веб-служб Exchange и другие веб-службы в Exchange

Узнайте, новые возможности в веб-служб Exchange и веб-службы в Exchange и управляемый API веб-служб Exchange.
  
Веб-службы в Exchange были обновлены для включения новых функций. 
  
**В таблице 1. Новые веб-службы средства в Exchange Online, Exchange 2013 и управляемый API веб-служб Exchange**

|Компонент|Реализованы в Exchange Online|Реализованный в Exchange 2013|Реализованный в управляемый API веб-служб Exchange|
|:-----|:-----:|:-----:|:-----:|
|[обнаружение электронных данных](#eDisc) <br/> |Да  <br/> |Да  <br/> |Да  <br/> |
|[Архивации](#arch) <br/> |Да  <br/> |Да  <br/> |Да  <br/> |
|[Действующие лица](#personas) <br/> |Да  <br/> |Да  <br/> |Нет  <br/> |
|[Единое хранилище контактов](#unified) <br/> |Да  <br/> |Да  <br/> |Нет  <br/> |
|[Политики хранения](#retentionpolicy) <br/> |Да  <br/> |Да  <br/> |Да  <br/> |
|[Фотографии пользователя](#userphoto) <br/> |Да  <br/> |Да  <br/> |Нет  <br/> |
|[Почтовые приложения для управления Outlook](#ewsmailapps) <br/> |Да  <br/> |Да  <br/> |Да  <br/> |
|[Предложение нового времени проведения собрания](#propose) <br/> |Да  <br/> |Нет  <br/> |Нет  <br/> |

<a name="eDisc"> </a>

## <a name="ediscovery-in-ews"></a>обнаружение электронных данных в веб-служб Exchange

обнаружение электронных данных является федеративным запроса веб-службы, которая позволяет внешних приложений, таких как SharePoint 2013 выполнять запросы данных Exchange. Обнаружение включает несколько этапов, включая определение и сохранение данных ключа, отбора вниз и просмотра данных и создания данных в суд. запросов обнаружения электронных данных упростить процесс обнаружения с указанием одного обнаружения рабочего процесса в Exchange и SharePoint.
  
**В таблице 2. Операции веб-служб Exchange и управляемый API EWS методы для работы с обнаружения электронных данных**

|**Имя операции**|**Метод управляемого API EWS**|**Описание**|
|:-----|:-----|:-----|
|[Операция GetDiscoverySearchConfiguration](http://msdn.microsoft.com/library/8a54a6dc-110c-4972-a8bc-5ddb43c4b857%28Office.15%29.aspx) <br/> |[ExchangeService.GetDiscoverySearchConfiguration()](http://msdn.microsoft.com/en-us/library/jj670206%28v=exchg.80%29.aspx) <br/> |Получает данные конфигурации для удержания на месте, сохраненные операций поиска обнаружения и почтовые ящики, которые разрешены для поиска обнаружения.  <br/> |
|[Операция GetHoldOnMailboxes](http://msdn.microsoft.com/library/9157f329-80b4-4cd0-a158-378064966ae6%28Office.15%29.aspx) <br/> |[ExchangeService.GetHoldOnMailboxes()](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.exchangeservice.getholdonmailboxes%28v=exchg.80%29.aspx) <br/> |Получает состояние запроса на удержание, которая задается с помощью операции **SetHoldOnMailboxes** .  <br/> |
|[Операция GetNonIndexableItemDetails](http://msdn.microsoft.com/library/9279c3ad-f7c8-4bbc-b0a7-2c78416cb39a%28Office.15%29.aspx) <br/> |[ExchangeService.GetNonIndexableItemDetails()](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.exchangeservice.getnonindexableitemdetails%28v=exchg.80%29.aspx) <br/> |Возвращает подробные сведения об элементах, которые не могут быть индексированы. Это включает в себя, но не ограничивается идентификатор элемента, код ошибки, описание ошибки при попытке индексировать элемент, а также дополнительные сведения об элементе.  <br/> |
|[Операция GetNonIndexableItemStatistics](http://msdn.microsoft.com/library/ed077877-9d98-4434-b8b6-a4a905e7f7a6%28Office.15%29.aspx) <br/> |[ExchangeService.GetNonIndexableItemStatistics()](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.exchangeservice.getnonindexableitemstatistics%28v=exchg.80%29.aspx) <br/> |Получает число элементов, которые не могут быть индексированы в почтовом ящике.  <br/> |
|[Операция GetSearchableMailboxes](http://msdn.microsoft.com/library/47f8ff57-4835-4d2d-9136-44afb31a4cbe%28Office.15%29.aspx) <br/> |[ExchangeService.GetSearchableMailboxes()](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.exchangeservice.getsearchablemailboxes%28v=exchg.80%29.aspx) <br/> |Получает список почтовых ящиков, который имеет разрешение на поиска или обнаружения электронных данных на клиенте.  <br/> |
|[Операция SearchMailboxes](http://msdn.microsoft.com/library/8a67c1d8-d021-4e68-aa62-35f7d9c2edc7%28Office.15%29.aspx) <br/> |[ExchangeService.SearchMailboxes()](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.exchangeservice.searchmailboxes%28v=exchg.80%29.aspx) <br/> |Выполняет поиск элементов в определенных почтовых ящиков, которые соответствуют ключевые слова запроса.  <br/> |
|[Операция SetHoldOnMailboxes](http://msdn.microsoft.com/library/9015a0d8-3495-461b-aa79-797d23169585%28Office.15%29.aspx) <br/> |[ExchangeService.SetHoldOnMailboxes()](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.exchangeservice.setholdonmailboxes%28v=exchg.80%29.aspx) <br/> |Наборы на основе запроса содержат элементы.  <br/> |

<a name="arch"> </a>

## <a name="archiving-in-ews"></a>Архивация в веб-служб Exchange

Архивные почтовые ящики, дополнительного почтовые ящики, связанные с пользователем. Архивные почтовые ящики обычно используются для управления ограничениями на размер хранилища электронной почты. Например старые элементы электронной почты могут периодически перемещены из папки «Входящие» в архивный почтовый ящик. 
  
Exchange представлены два новых операций веб-служб Exchange, которые можно использовать для архивирования набор почтовых элементов от основного почтового ящика. Архивация элементов папки "Входящие" таким образом сохраняет иерархии папок, вложенных элементов. Кроме того архивные почтовые ящики можно хранить теперь локально на клиенте, либо удаленно, в результате которого большей части прозрачно для пользователей, используя путь к папке для указания на содержимого архива.
  
**В таблице 3. Операции веб-служб Exchange и управляемый API EWS методы для работы с архивами**

|**Имя операции**|**Метод управляемого API EWS**|**Описание**|
|:-----|:-----|:-----|
|[Операция ArchiveItem](http://msdn.microsoft.com/library/1af216b3-13ea-498e-b4fc-23513755d731%28Office.15%29.aspx) <br/> |[ExchangeService.ArchiveItems()](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.exchangeservice.archiveitems%28v=exchg.80%29.aspx) <br/> |Перемещает элемент из основного почтового ящика в архивный почтовый ящик.  <br/> |
|[Операция CreateFolderPath](http://msdn.microsoft.com/library/5a10aa5e-3f25-4ec3-a0b9-284c30918a1f%28Office.15%29.aspx) <br/> |Не реализован.  <br/> |Создание иерархии папок в основной или архивного почтового ящика.  <br/> |

<a name="personas"> </a>

## <a name="personas-in-ews"></a>Действующие лица в веб-служб Exchange

*Пользователя* — это набор данных, связанный с пользователем. Данные могут поступать из одного или нескольких источников и связанный с пользователя с помощью идентификатора общие ссылки Действующие лица в веб-служб Exchange позволяют ссылка, поиск, просмотр и получение сведений о сотруднике из нескольких источников и организовать их в одном логический объект. Действующие лица отличаются от контактов, что контакт — это набор данных из одного источника, связанный с пользователем; например личный контакт Outlook или запись в глобальном списке адресов (GAL). 
  
Управляемый API EWS не реализует эту функцию.
  
> [!NOTE]
> Единого хранилища контактов также предоставляет функциональные возможности пользователя с помощью операции, которые поддерживают эту функцию. 
  
**В таблице 4. Операции EWS для работы с пользователями**

|**Имя операции**|**Описание**|
|:-----|:-----|
|[Операция FindPeople](http://msdn.microsoft.com/library/446106b7-ff2d-4107-90c1-29f4d38ba128%28Office.15%29.aspx) <br/> |Возвращает все объекты пользователя из указанной папке контактов или получает все контакты, соответствующие указанному запросу строки.  <br/> |
|[Операция GetPersona](http://msdn.microsoft.com/library/e2146df0-53d0-4caf-9758-b600bbc14b6a%28Office.15%29.aspx) <br/> |Получает пользователя.  <br/> |

<a name="unified"> </a>

## <a name="unified-contact-store-in-ews"></a>Единое хранилище контактов в веб-служб Exchange

Единого хранилища контактов — это функция, которая обеспечивает согласованность контакта в разных продуктов Office и выступает в качестве точки интеграции для приложений сторонних производителей для использования в одном хранилище контактов. Это позволяет пользователям и приложениям для хранения, управления и доступ к контактной информации и сделать его доступным глобальный среди Lync, Exchange 2013, Outlook, Outlook Web App и любых других приложений, который реализует доступ к единого хранилища контактов. Exchange не хранилище контактов для взаимодействия единого хранилища контактов. 
  
Управляемый API EWS не реализует эту функцию.
  
**В таблице 5. Операции EWS для работы с единого хранилища контактов**

|**Имя операции**|**Описание**|
|:-----|:-----|
|[Операция AddNewImContactToGroup](http://msdn.microsoft.com/library/0cb5525f-faa3-48f1-9551-df55ffc26f46%28Office.15%29.aspx) <br/> |Добавление нового контакта обмена мгновенными Сообщениями в группу. Единого хранилища контактов может содержать не более 1000 контактов.  <br/> |
|[Операция AddImContactToGroup](http://msdn.microsoft.com/library/376acc42-2684-4596-aca1-82a4a10865c9%28Office.15%29.aspx) <br/> |Добавляет существующего контакта обмена мгновенными Сообщениями в группу. Единого хранилища контактов может содержать не более 1000 контактов.  <br/> |
|[Операция AddImGroup](http://msdn.microsoft.com/library/6df6e504-b7c8-4773-b10f-ffa5defac229%28Office.15%29.aspx) <br/> |Добавляет новую группу обмена мгновенными Сообщениями. Единого хранилища контактов может содержать до 64 групп.  <br/> |
|[Операция AddNewTelUriContactToGroup](http://msdn.microsoft.com/library/c9688ce8-2465-45bb-8bd2-94b32ed4885c%28Office.15%29.aspx) <br/> |Добавляет новый контакт в группу на основании номер телефона контакта.  <br/> |
|[Операция AddDistributionGroupToImList](http://msdn.microsoft.com/library/5aa9bec8-71cf-4a6e-8ec8-b4965b40fd4a%28Office.15%29.aspx) <br/> |Добавляет новую группу списка рассылки. Единого хранилища контактов может содержать до 64 групп.  <br/> |
|[Операция GetImItemList](http://msdn.microsoft.com/library/e31d14e1-0c1f-4b69-98b7-157d59c13698%28Office.15%29.aspx) <br/> |Получает список групп для IM и фиктивных пользователей, включающих контакты для IM.  <br/> |
|[Операция GetImItems](http://msdn.microsoft.com/library/51186691-46d2-4d5c-b8bc-4ee2bb20fbe7%28Office.15%29.aspx) <br/> |Извлекает сведения о указанными группами обмена мгновенными Сообщениями и обмена мгновенными Сообщениями контакта пользователей.  <br/> |
|[Операция RemoveContactFromImList](http://msdn.microsoft.com/library/28ec96c3-45af-48ff-9f17-718a527dc0ad%28Office.15%29.aspx) <br/> |Удаление указанного контакта из всех групп обмена мгновенными Сообщениями.  <br/> |
|[Операция RemoveImContactFromGroup](http://msdn.microsoft.com/library/a190bbec-c71b-4e6a-880b-55854c724d8c%28Office.15%29.aspx) <br/> |Удаляет для обмена мгновенными Сообщениями контакта из группы.  <br/> |
|[Операция RemoveDistributionGroupFromImList](http://msdn.microsoft.com/library/252bddf2-98b6-4824-b548-2fba2bda5384%28Office.15%29.aspx) <br/> |Удаляет указанную группу списка рассылки обмена мгновенными Сообщениями.  <br/> |
|[Операция RemoveImGroup](http://msdn.microsoft.com/library/5e788016-68e0-4a3f-9243-03f6b6c6b389%28Office.15%29.aspx) <br/> |Удаляет указанную группу обмена мгновенными Сообщениями.  <br/> |
|[Операция SetImGroup](http://msdn.microsoft.com/library/2d48aa07-8152-4c3d-a519-061253e80174%28Office.15%29.aspx) <br/> |Изменяется отображаемое имя группы.  <br/> |

<a name="retentionpolicy"> </a>
  
## <a name="retention-policies-in-ews"></a>Политики хранения в веб-служб Exchange

Политики хранения, политики, которые используются в Exchange для группы один или несколько тегов хранения, позволяют применять параметры хранения для папки или отдельных элементов, такие как сообщения электронной почты и голосовой почты, а также для применения параметров хранения для почтового ящика.
  
Exchange включает в себя три типа тегов хранения:
  
- Теги политики по умолчанию, которые применяются к элементов почтовых ящиков, которые имеют никакой другой тип тега хранения, примененного.
    
- Системные теги политики папки, которые применяются к папок по умолчанию, например папки «Входящие».
    
- Личные теги, которые пользователь может применить к папкам, которые они создают или для отдельных элементов.
    
Политика хранения только один можно назначить почтовому ящику, но политики может иметь один или несколько тегов хранения различных типов, связанных с ней. Теги хранения могут быть связаны для или несвязанные из политики хранения в любое время. ВЕБ-службах Exchange предоставляет новую операцию, [GetUserRetentionPolicyTags](http://msdn.microsoft.com/library/57c6ff23-5c2c-42ee-824b-5a1b6dafab8c%28Office.15%29.aspx)и управляемый API EWS реализует новый метод [ExchangeService.GetUserRetentionPolicyTags()](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.exchangeservice.getuserretentionpolicytags%28v=exchg.80%29.aspx), предоставляющий список всех тегов, связанные с политикой хранения. Можно задать и получить теги политики хранения для элементов и папок с помощью **CreateItem**, **CreateFolder**, **UpdateItem**, **UpdateFolder**, **GetItem**и **GetFolder** операций. 

<a name="userphoto"> </a>

## <a name="requesting-user-photos"></a>Разрешения на запрос фотографий

Можно запросить фотографии пользователя с сервера Exchange server с помощью одного из двух реализаций [GetUserPhoto операции](http://msdn.microsoft.com/library/f6e8143d-4235-428e-8f9c-ab6e9b1cfa6e%28Office.15%29.aspx): [REST](how-to-get-user-photos-by-using-ews-in-exchange.md) или SOAP. Конечная точка REST использует стандартные запроса HTTPS, **Получение** для получения фото пользователя. Служба либо возвращает фото пользователя, хранящиеся в Exchange или фотографию из доменных служб Active Directory (AD DS). 
  
Управляемый API EWS не реализует эту функцию. Тем не менее, можно использовать управляемый API EWS для возврата фотографии пользователя, которые хранятся в почтовом ящике, получив фотографий, подключенный к контакту.

<a name="blocksender"> </a>

## <a name="block-senders-and-mark-email-as-junk-in-ews"></a>Блокировать отправителей и отметить электронной почты как нежелательные сообщения в веб-служб Exchange

Теперь можно блокировать отправителей и пометка нежелательной электронной почты с помощью создания [операции MarkAsJunk](http://msdn.microsoft.com/library/1f71f04d-56a9-4fee-a4e7-d1034438329e%28Office.15%29.aspx) в веб- или с помощью метода [ExchangeService.MarkAsJunk()](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.exchangeservice.markasjunk%28v=exchg.80%29.aspx) в управляемый API веб-служб Exchange. 

<a name="ewsmailapps"> </a>

## <a name="mail-apps-for-outlook"></a>Почтовые приложения для Outlook

Веб-служб Exchange теперь включает поддержку управления почтовые приложения для Outlook. 
  
**В таблице 6. Операции веб-служб Exchange и управляемый API EWS методы для работы с почтовыми приложениями для Outlook**

|**Имя операции**|**Метод управляемого API EWS**|**Описание**|
|:-----|:-----|:-----|
|[Операция DisableApp](http://msdn.microsoft.com/library/211731a3-2470-49af-bda3-1ddfc15a8e46%28Office.15%29.aspx) <br/> |[ExchangeService.DisableApp()](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.exchangeservice.disableapp%28v=exchg.80%29.aspx) <br/> |Отключает установленного приложения.  <br/> |
|[Операция GetAppManifests](http://msdn.microsoft.com/library/21a4987c-c24d-4a6e-ace4-e81edcda6303%28Office.15%29.aspx) <br/> |[ExchangeService.GetAppManifests()](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.exchangeservice.getappmanifests%28v=exchg.80%29.aspx) <br/> |Получает манифестов приложений для почтового ящика.  <br/> |
|[Операция GetAppMarketplaceUrl](http://msdn.microsoft.com/library/2c016fc3-0e13-4624-9a5b-d3e84577a860%28Office.15%29.aspx) <br/> |[ExchangeService.GetAppMarketplaceUrl()](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.exchangeservice.getappmarketplaceurl%28v=exchg.80%29.aspx) <br/> |Получает URL-адрес приложения marketplace.  <br/> |
|[Операция GetClientAccessToken](http://msdn.microsoft.com/library/086876cc-e22c-4e89-89f9-19e78af51217%28Office.15%29.aspx) <br/> |[ExchangeService.GetClientAccessToken()](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.exchangeservice.getclientaccesstoken%28v=exchg.80%29.aspx) <br/> |Получает маркеры доступа клиентов.  <br/> |
|[Операция InstallApp](http://msdn.microsoft.com/library/596eae95-3e78-489a-8bb2-d2dd4a026405%28Office.15%29.aspx) <br/> |[ExchangeService.InstallApp()](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.exchangeservice.installapp%28v=exchg.80%29.aspx) <br/> |Устанавливает приложение для почтового ящика.  <br/> |
|[Операция UninstallApp](http://msdn.microsoft.com/library/7707aa6a-381d-43f7-a454-54f6343ed127%28Office.15%29.aspx) <br/> |[ExchangeService.UninstallApp](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.exchangeservice.uninstallapp%28v=exchg.80%29.aspx) <br/> |Удаление приложения из почтового ящика.  <br/> |

<a name="propose"> </a>

## <a name="propose-new-meeting-time"></a>Предложение нового времени проведения собрания

Новая функция время предложить была представлена в версии 15.00.0800.007 Exchange. Это позволяет участникам собрания возможность [предложение нового времени](how-to-propose-a-new-meeting-time-by-using-ews-in-exchange.md) для организатора собрания. 
  
Управляемый API EWS не реализует эту функцию.
  
## <a name="see-also"></a>См. также

- [Сведения об управляемом API EWS, EWS и веб-службах в Exchange](explore-the-ews-managed-api-ews-and-web-services-in-exchange.md)  
- [Общие сведения о разработке клиента EWS для Exchange](ews-client-design-overview-for-exchange.md)
- [Приложения электронной почты для Outlook и EWS в Exchange](mail-apps-for-outlook-and-ews-in-exchange.md)
- [Архивация в веб-служб Exchange в Exchange](archiving-in-ews-in-exchange.md)
- [обнаружение электронных данных в веб-службах Exchange](ediscovery-in-ews-in-exchange.md)
- [Пользователи и контакты в EWS для Exchange](people-and-contacts-in-ews-in-exchange.md)
    

