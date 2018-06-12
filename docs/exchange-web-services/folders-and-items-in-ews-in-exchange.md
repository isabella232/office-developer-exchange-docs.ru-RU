---
title: Папки и элементы в веб-службах Exchange
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
localization_priority: Normal
ms.assetid: 9d8cf6fa-85a4-45ac-8165-e4d3ab92594e
description: Сведения о папок и элементов почтового ящика и как управляемый API EWS или веб-служб Exchange client представляет их.
ms.openlocfilehash: a3358844f2317c9b0462456ff7d2f38442c98ee3
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/11/2018
ms.locfileid: "19760976"
---
# <a name="folders-and-items-in-ews-in-exchange"></a>Папки и элементы в веб-службах Exchange

Сведения о папок и элементов почтового ящика и как управляемый API EWS или веб-служб Exchange client представляет их.
  
Папки — упорядочения элемент почтовый ящик Exchange. Папки могут содержать элементы почтового ящика, такие как сообщения электронной почты, контактов, встреч, собраний и задач, или они могут содержать другие папки. Exchange включает различные типы папок, но типы папки похожи друг с другом. Основное различие между ними — это тип элемента, содержащихся в них.
  
Элементы, однако иметь уникальные типы. Каждый тип элемента имеет другой набор свойств или схемы для определения его. В этой статье обсуждаются типы папок и элементов, доступных и различия между ними.

<a name="bk_folders"> </a>

## <a name="folders"></a>Папки

Все папках являются производными от одного базового класса или базового типа, [класс в управляемый API EWS](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.folder%28v=EXCHG.80%29.aspx) или типа [папки](http://msdn.microsoft.com/library/812948d8-c7db-45ce-bb3a-77233a53a974%28Office.15%29.aspx) в веб-служб Exchange. На следующем рисунке показана управляемый API EWS классы и типы веб-служб Exchange. 
  
**На рисунке 1. Управляемый API EWS папки классы и типы папки веб-служб Exchange**

![Иллюстрация, показывающая классы, получаемые из класса управляемого API EWS Folder, и типы, получаемые из типа EWS Folder, именуемые CalendarFolder, ContactsFolder, SearchFolder и TasksFolder.](media/Ex2013_Folder_OverviewTypes.png)
  
Основное различие между каждым из классов папки и типы папки — это, что тип элемента можно создать только в каждый тип папки. Единственное отличие находится в отображения информации в папке клиента. Например Exchange позволяет создавать встреч в папке календаря. Можно переместить других типов элементов в папке календаря после их создания, но они не отображаются Outlook. Outlook отображаются только элементы календаря, например, встречи и собрания в папке календаря, [даже в том случае, если существует другой тип элемента в папке](folders-and-items-in-ews-in-exchange.md#bk_item). 
  
**В таблице 1. Управляемый API EWS папки классы и типы папки веб-служб Exchange**

|**Управляемый API EWS класс**|**Тип веб-служб Exchange**|**Значение FolderClass**|**Contains**|**Примечания**|
|:-----|:-----|:-----|:-----|:-----|
|[Folder](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.folder%28v=exchg.80%29.aspx) <br/> |[Folder](http://msdn.microsoft.com/library/812948d8-c7db-45ce-bb3a-77233a53a974%28Office.15%29.aspx) <br/> |IPF. Примечание  <br/> |Сообщения электронной почты или папки.  <br/> | Это общая папка класса или тип для следующих управляемый API EWS [WellKnownFolderName](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.wellknownfoldername%28v=exchg.80%29.aspx) и веб-служб Exchange [DistinguishedFolderId](http://msdn.microsoft.com/library/50018162-2941-4227-8a5b-d6b4686bb32f%28Office.15%29.aspx) папки: <ul><li>  Корневой (IPM поддерево)</li><li>NonIpmSubtree</li><li>Inbox</li><li>"Удаленные"</li><li>���������</li><li>������</li><li>����������  </li><li>Исходящие</li><li>Отправленные элементы</li><li>Папка сообщений</li><li>Нежелательной почты</li><li>Голосовая почта</li></ul> |
|[CalendarFolder](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.calendarfolder%28v=exchg.80%29.aspx) <br/> |[CalendarFolder](http://msdn.microsoft.com/library/48687a78-e757-4c04-9641-bf4302c6b565%28Office.15%29.aspx) <br/> |IPF. Встречи  <br/> |Встречи и собрания.  <br/> |Когда пользователь отвечает на приглашения на собрание, управляемый API EWS [WellKnownFolderName.Calendar](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.wellknownfoldername%28v=exchg.80%29.aspx) или веб-служб Exchange [DistinguishedFolderId.CalendarFolder](http://msdn.microsoft.com/library/50018162-2941-4227-8a5b-d6b4686bb32f%28Office.15%29.aspx) только добавляется встречи. Далее представлены только папки, которые поддерживают автоматического взаимодействия с приглашений на собрания и ответы.  <br/><br/>Этот класс папки или папки тип поддерживает использование представления календаря для возврата встречи и собрания на основе Дата начала и Дата завершения с помощью метода управляемый API EWS [Folder.FindItem](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.folder.finditems%28v=EXCHG.80%29.aspx) и класс [представления календаря](http://msdn.microsoft.com/EN-US/library/microsoft.exchange.webservices.data.calendarview%28v=exchg.80%29.aspx) или веб-служб Exchange [FindItem ](http://msdn.microsoft.com/library/ebad6aae-16e7-44de-ae63-a95b24539729%28Office.15%29.aspx)операции и элемент [представления календаря](http://msdn.microsoft.com/library/a4a953b8-0710-416c-95ef-59e51eba9982%28Office.15%29.aspx) .  <br/> |
|[ContactsFolder](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.contactsfolder%28v=exchg.80%29.aspx) <br/> |[ContactsFolder](http://msdn.microsoft.com/library/6c299de8-2087-4aeb-8e66-2bc7586509a6%28Office.15%29.aspx) <br/> |IPF. Контакт  <br/> |Контакты и списки рассылки.  <br/> |Нет.  <br/> |
|[SearchFolder](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.searchfolder%28v=exchg.80%29.aspx) <br/> |[SearchFolder](http://msdn.microsoft.com/library/1a7d408b-2e98-4391-8834-085ed6d5757c%28Office.15%29.aspx) <br/> |IPF. Примечание  <br/> |Содержимое, определяются ограничения или фильтра. Папки поиска нет вложенных папок.  <br/> |Элементы, которые соответствуют критериям поиска фактически не содержатся в папке поиска; Вместо этого они находятся в другом месте в почтовый ящик.  <br/> Убедитесь, что в папках поиска доступны в Outlook, создайте их в папку поиска.  <br/> |
|[TasksFolder](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.tasksfolder%28v=exchg.80%29.aspx) <br/> |[TasksFolder](http://msdn.microsoft.com/library/5a9a4612-8064-4986-b467-c44f268c64df%28Office.15%29.aspx) <br/> |IPF. Задача  <br/> |Содержит рабочих элементов для выполнения.  <br/> |Нет.  <br/> |
   
### <a name="folder-structure"></a>Структура папок

Папки обеспечивают структуру почтового ящика. Этот компонент включает поддерева IPM, известных как хранилища в веб-служб Exchange, когда большинство пользователей взаимодействуют с почтовым ящиком, а также папок системы, большинство пользователей не отображается, которые хранятся в поддерева IPM не или корневой в веб. На следующем рисунке показана структура папки для пользователя и указывает папок — для пользователя элементов, а какие — системных папок.
  
**На рисунке 2. Элемент и система папок в почтовом ящике**

![Иллюстрация, показывающая системные папки в Root, включая Favorites, Finder, FreeBusy Data, Top of Information Store и другие. Папка Top of Information Store содержит пользовательские папки, включая календарь, контакты и пр.](media/Ex2013_Folder_OverviewSampleHierarchy.png)
  
### <a name="well-known-folders"></a>Хорошо известные папки

Папок в почтовом ящике указаны некоторые специальные папки. Они соответствуют известных папок в управляемый API веб-служб Exchange и различающееся папок в веб-служб Exchange. Некоторые из этих папок имеют ограничения на имя папки, где они находятся в структуре папок, а также ли они могут быть удалены. Другие «общих» папки (без специальных) не имеют те же ограничения. Важно быть знакомы с следующие папки известных или различающееся, так как они корневой системы, пользователей и папок поиска и могут быть применены большинство реализаций. 
  
**В таблице 2. Основной известный и различающееся папок**

|**Понятное имя**|**Управляемый API EWS **WellKnownFolderName** значения**|**Значения **DistinguishedFolderId** веб-служб Exchange**|**Описание**|
|:-----|:-----|:-----|:-----|
|Корневой (не являющиеся IPM поддерево)  <br/> |WellKnownFolderName.Root  <br/> |DistinguishedFolderId.root  <br/> |Содержит корневую папку почтового ящика, также известной как поддерева IPM без поддержки. Эта папка не имеет родительского и нельзя переместить, скопируйте, переименуйте или удалите его. Хранилище каждого сообщения содержит только один корневой папки.  <br/> |
|Верхняя часть информационного хранилища (IPM поддерево)  <br/> |WellKnownFolderName.MsgFolderRoot  <br/> |DistinguishedFolderId.msgfolderroot  <br/> |Содержит папки «Входящие» и других пользовательских папках.  <br/> |
|Finder (папки поиска)  <br/> |WellKnownFolderName.SearchFolders  <br/> |DistinguishedFolderId.searchfolders.  <br/> |Содержит папки поиска, которые отображаются в Outlook.  <br/> |
   
Полный список значений свойств управляемый API EWS [WellKnownFolderName](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.folder.wellknownfoldername%28v=exchg.80%29.aspx) [WellKnownFolderName](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.wellknownfoldername%28v=EXCHG.80%29.aspx) см. Полный список значений веб-служб Exchange **DistinguishedFolderId** в разделе [DistinguishedFolderId](http://msdn.microsoft.com/library/50018162-2941-4227-8a5b-d6b4686bb32f%28Office.15%29.aspx).
  
### <a name="folder-properties"></a>Свойства Folder

Управляемый API веб-служб Exchange, в [Свойства папки](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.folder_properties%28v=exchg.80%29.aspx) являются производными от базового класса [папки](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.folder%28v=EXCHG.80%29.aspx) . И в веб-служб Exchange, используйте элементы папки, доступные для типа [папки](http://msdn.microsoft.com/library/812948d8-c7db-45ce-bb3a-77233a53a974%28Office.15%29.aspx) всех папок. Большая часть свойств, связанных с папки и элементы являются просто (идентификатор родительской папки, отображаемое имя и т. д.), но некоторые требуют остановиться более подробно. 
  
К управляемый API EWS [Folder.FolderClass](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.folder.folderclass%28v=EXCHG.80%29.aspx) свойство или элемент веб-служб Exchange [FolderClass](http://msdn.microsoft.com/library/0041d135-2869-4612-89a5-d1aa86aa1093%28Office.15%29.aspx) применяются следующие факторы. 
  
- Если установлен, значение свойства или элемента должно соответствовать производного класса или тип папки. К примеру **FolderClass** свойство или элемент не может указать, что папки Контакты при класса или тип папки указывает, что папки календаря. 
    
- Можно либо [Создать папок](how-to-work-with-folders-by-using-ews-in-exchange.md#bk_createfolderewsma) определенного типа без указания **FolderClass** свойство или элемент, или можно создать папку с папкой стандартного типа и укажите **FolderClass** свойства или элемента. Оба параметра создание тем же. 
    
- После установки значения **FolderClass** путем создания определенного типа папки или путем установки свойства **FolderClass** или сам элемент, изменить его нельзя. Например нельзя изменить IPF. Папка Примечание к IPF. Обратитесь в папке. Тем не менее, его можно изменить для IPF. Папка Note.Contoso. 
    
- Любое значение **FolderClass** , который не используется ни один из предварительно заданных префиксов обрабатывается как IPF. Папка заметок. Например значение **FolderClass** IAmAFolderClass обрабатывается как IPF. Папка заметок. 
    
Значение класса папка является расширяемым. Это означает, что **FolderClass** значения по умолчанию, указанные в таблице 1 обрабатывается как префиксы и можно добавить пользовательские значения. Например можно создать папку со значением **FolderClass** IPF. Contact.Contoso и он обрабатывается как папку Контакты. 
  
Можно определить, какие разрешения, которые клиент имеет для папок, например, удаление, чтения и изменения, с помощью свойства управляемый API EWS [Folder.EffectiveRights](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.folder.effectiverights%28v=EXCHG.80%29.aspx) или веб-служб Exchange [EffectiveRights](http://msdn.microsoft.com/library/bf5278eb-3a1a-4d27-9d16-b8be043bb023%28Office.15%29.aspx) элемент. 
  
### <a name="public-folders"></a>Общие папки

Общие папки предназначены для общего доступа и предоставляют простой и эффективный способ сбора, организации и обмениваться информацией с другими пользователями в рабочей группе или организации. Также можно использовать общие папки для архивирования содержимого группы рассылки. Подробные сведения об общих папках содержатся в разделе [общих папок в Exchange доступ с помощью веб-служб Exchange](public-folder-access-with-ews-in-exchange.md).

<a name="bk_hiddenfolders"> </a>

### <a name="hidden-folders"></a>Скрытые папки

Все папки, создаваемые в корне почтовый ящик Exchange скрыты, и можно использовать управляемый API EWS или веб-служб Exchange для скрытия дополнительных папок в хранилища. Дополнительные сведения о скрытых папок [скрытые папки с помощью веб-служб Exchange в Exchange](how-to-work-with-hidden-folders-by-using-ews-in-exchange.md)см. 

<a name="bk_hiddenfolders"> </a>

### <a name="search-folders"></a>Папки поиска

Папки поиска — так же, как обычные папки, за исключением того, что у них есть свойство или элемент, который определяет поисковый фильтр. Папки поиска можно создать в любой папке в почтовый ящик Exchange, и их создания так же, как создавать любую другую папку. Тем не менее для папки поиска в Outlook, Outlook Web App или Outlook Live, [SearchFolder](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.searchfolder%28v=exchg.80%29.aspx) объекты, созданные с помощью управляемого интерфейса API веб-служб Exchange должны быть расположены в папке [WellKnownFolderName.SearchFolders](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.wellknownfoldername%28v=exchg.80%29.aspx) и [SearchFolder](http://msdn.microsoft.com/library/1a7d408b-2e98-4391-8834-085ed6d5757c%28Office.15%29.aspx) типы, которые создаются с помощью веб-служб Exchange должны быть расположены в папке [DistinguishedFolderId.SearchFolders](http://msdn.microsoft.com/library/50018162-2941-4227-8a5b-d6b4686bb32f%28Office.15%29.aspx) . Если папка поиска создается в другом месте, по-прежнему доступен, и его можно просмотреть в пользовательских клиентских приложений. 

<a name="bk_item"> </a>

## <a name="items"></a>Элементы

**Элементы** используются веб-службах Exchange для представления отдельные сообщения электронной почты, встреч, собраний, контакты, списки рассылки, задачи, записи и других элементов в почтовом ящике. Элементы, либо строго типизированных, что означает, что они имеют конкретного связанного класса или схема или не строго типизированные, также известной как универсальный элементов. Универсальный элементы являются объекты [элементов](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.item%28v=exchg.80%29.aspx) в типах управляемый API EWS и [элементов](http://msdn.microsoft.com/library/4dfe8f48-e7b4-444d-bdf9-a34e180f598b%28Office.15%29.aspx) в веб-служб Exchange. Общие элементы, такие как сообщения электронной почты, контакты, списки рассылки, публикации, и строго типизированных задачи можно задать Схематизированный свойств или элементов на них. 
  
**В таблице 3. Строго типизированные элементы**

|**Управляемый API EWS тип элемента**|**Элемент веб-служб Exchange**|
|:-----|:-----|
|[Встреча](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.appointment%28v=exchg.80%29.aspx) <br/> |[Элемента календаря, имеющего](http://msdn.microsoft.com/library/b0c1fd27-b6da-46e5-88b8-88f00c71ba80%28Office.15%29.aspx) <br/> |
|[Контакт](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.contact%28v=exchg.80%29.aspx) <br/> |[Контакт](http://msdn.microsoft.com/library/66bfff50-7a91-4d81-b6a0-610b9962f677%28Office.15%29.aspx) <br/> |
|[ContactGroup](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.contactgroup%28v=exchg.80%29.aspx) <br/> |[DistributionList](http://msdn.microsoft.com/library/f65aea01-e870-44a2-8571-fa6c001341cc%28Office.15%29.aspx) <br/> |
|[EmailMessage](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.emailmessage%28v=exchg.80%29.aspx) <br/> |[Message](http://msdn.microsoft.com/library/2400b33c-43b2-4fc2-b6fb-275a99e0e810%28Office.15%29.aspx) <br/> |
|[PostItem](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.postitem%28v=exchg.80%29.aspx) <br/> |[PostItem](http://msdn.microsoft.com/library/7727ed84-9591-4a1c-bb04-12129926499b%28Office.15%29.aspx) <br/> |
|[Задача](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.task%28v=exchg.80%29.aspx) <br/> |[Задача](http://msdn.microsoft.com/library/7c84927e-db28-4c5d-b0b5-cbcc2b88d869%28Office.15%29.aspx) <br/> |
   
Управляемый API EWS строго типизированных элементы являются производными от базового класса [элемента](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.item%28v=EXCHG.80%29.aspx) . Тем не менее вы обычно работают с одним из производных типов, перечисленных в таблице 3, а не с **класс** непосредственно. При работе с классом [ItemCollection](http://msdn.microsoft.com/en-us/library/dd634001%28v=EXCHG.80%29.aspx) , тем не менее, можно работать непосредственно с экземпляры класса **элемента** . В этом случае следует применить логику, которая определяет тип элемента в хранилище, представляющий экземпляр класса **элемента** . Для работы с этого элемента следует привязать к элементу с помощью экземпляра класса, который представляет элемент. 
  
### <a name="items-in-folders"></a>Элементы в папках

Некоторые папки имеют ограничения на типы элементов, которые могут содержать. Это ограничения, которые базы данных почтовых ящиков Exchange применяется к папкам, не ограничения представления клиента. 
  
**В таблице 4. Элемент ограничения для папок**

|**Класс управляемой папки API веб-служб Exchange**|**Тип папки веб-служб Exchange**|**Ограничения**|
|:-----|:-----|:-----|
|[Базовый класс папки](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.folder%28v=exchg.80%29.aspx) <br/> |[Folder](http://msdn.microsoft.com/library/812948d8-c7db-45ce-bb3a-77233a53a974%28Office.15%29.aspx) <br/> |Новые объекты управляемый API EWS [EmailMessage](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.emailmessage%28v=exchg.80%29.aspx) и [PostItem](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.postitem%28v=exchg.80%29.aspx) объекты или типы веб-служб Exchange [сообщение](http://msdn.microsoft.com/library/2400b33c-43b2-4fc2-b6fb-275a99e0e810%28Office.15%29.aspx) или **PostItem** типов, можно создать только в универсальный папок. Можно перемещать других типов элементов на универсальный папок, но клиент может не отображаются.  <br/> |
|[CalendarFolder](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.calendarfolder%28v=exchg.80%29.aspx) <br/> |[CalendarFolder](http://msdn.microsoft.com/library/48687a78-e757-4c04-9641-bf4302c6b565%28Office.15%29.aspx) <br/> |Новые объекты управляемый API EWS [встречи](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.appointment%28v=exchg.80%29.aspx) и типы веб-служб Exchange [элемента календаря, имеющего](http://msdn.microsoft.com/library/b0c1fd27-b6da-46e5-88b8-88f00c71ba80%28Office.15%29.aspx) создаются только в папке календаря. Можно переместить других типов элементов в папке календаря, но клиент может не отображаются.  <br/> |
|[ContactsFolder](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.contactsfolder%28v=exchg.80%29.aspx) <br/> |[ContactsFolder](http://msdn.microsoft.com/library/6c299de8-2087-4aeb-8e66-2bc7586509a6%28Office.15%29.aspx) <br/> |Новый управляемый API EWS [контакта](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.contact%28v=exchg.80%29.aspx) и [ContactGroup](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.contactgroup%28v=exchg.80%29.aspx) объектов или веб-служб Exchange [контакт](http://msdn.microsoft.com/library/66bfff50-7a91-4d81-b6a0-610b9962f677%28Office.15%29.aspx) или [DistributionList](http://msdn.microsoft.com/library/f65aea01-e870-44a2-8571-fa6c001341cc%28Office.15%29.aspx) типы создаются только в папке «Контакты». Можно переместить других типов элементов в папке «Контакты», но клиент может не отображаться их  <br/> |
|[SearchFolder](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.searchfolder%28v=exchg.80%29.aspx) <br/> |[SearchFolder](http://msdn.microsoft.com/library/1a7d408b-2e98-4391-8834-085ed6d5757c%28Office.15%29.aspx) <br/> |Без ограничений. Элементы самом деле не располагаются в папке поиска; они находятся в другом месте в почтовый ящик.  <br/> |
|[TasksFolder](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.tasksfolder%28v=exchg.80%29.aspx) <br/> |[TasksFolder](http://msdn.microsoft.com/library/5a9a4612-8064-4986-b467-c44f268c64df%28Office.15%29.aspx) <br/> |Новые объекты управляемый API EWS [задач](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.task%28v=exchg.80%29.aspx) или типы веб-служб Exchange [задач](http://msdn.microsoft.com/library/7c84927e-db28-4c5d-b0b5-cbcc2b88d869%28Office.15%29.aspx) создаются только в папке заданий. Можно переместить других типов элементов в папке задач, но клиент может не отображаться их  <br/> |

<a name="bk_upgrading"> </a>

## <a name="upgrading-from-earlier-product-versions"></a>Обновление с более ранних версий

Папки в большинстве случаев, оставшихся без изменений в текущей и более ранних версиях. Обратите внимание, что более ранних версий Exchange использовать управляемые папки для выполнения управление записями сообщений (MRM). Exchange Online, Exchange Online как часть Office 365 и версии Exchange, начиная с Exchange 2013 использовать политики хранения для управления записями сообщений. Можно выполнить [обновление управляемых папок, которые следует использовать политики хранения](http://technet.microsoft.com/en-us/library/dd298032%28v=exchg.150%29.aspx). 
  
Элементы не были изменены в текущей и более ранних версиях.

<a name="bk_inthissection"> </a>

## <a name="in-this-section"></a>В этом разделе

- [Работа с папками с помощью веб-служб Exchange в Exchange](how-to-work-with-folders-by-using-ews-in-exchange.md)
    
- [Работа с скрытые папки с помощью веб-служб Exchange в Exchange](how-to-work-with-hidden-folders-by-using-ews-in-exchange.md)
    
- [Работа с элементами почтового ящика Exchange с помощью веб-служб Exchange в Exchange](how-to-work-with-exchange-mailbox-items-by-using-ews-in-exchange.md)
    
- [Удаление элементов с помощью веб-служб Exchange в Exchange](deleting-items-by-using-ews-in-exchange.md)
    
- [Экспорт и импорт элементов с помощью веб-служб Exchange в Exchange](exporting-and-importing-items-by-using-ews-in-exchange.md)
    
## <a name="see-also"></a>См. также

- [Разработка клиентов веб-служб для Exchange](develop-web-service-clients-for-exchange.md)   
- [Начать работу с использованием веб-служб Exchange](start-using-web-services-in-exchange.md)   
- [Общие сведения о разработке клиента EWS для Exchange](ews-client-design-overview-for-exchange.md)
    

