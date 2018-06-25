---
title: Общедоступная папка доступ с помощью веб-служб Exchange в Exchange
manager: sethgros
ms.date: 7/17/2015
ms.audience: Developer
localization_priority: Normal
ms.assetid: d9372057-1deb-45de-8f98-b9149604429a
description: Сведения о том, как использовать управляемый API EWS и веб-служб Exchange для доступа к общим папкам и маршрутизации запросов общих папок в Exchange.
ms.openlocfilehash: cfa089ba617dc760ed12883590e141debb5ecd9b
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/25/2018
ms.locfileid: "19761242"
---
# <a name="public-folder-access-with-ews-in-exchange"></a>Общедоступная папка доступ с помощью веб-служб Exchange в Exchange

Сведения о том, как использовать управляемый API EWS и веб-служб Exchange для доступа к общим папкам и маршрутизации запросов общих папок в Exchange.
  
Общие папки обеспечивают общее хранилище элементов, которые могут получить доступ к пользователям в вашей организации. Office 365, Exchange Online и локальной версии Exchange, начиная с Exchange 2013 представлена новая архитектура для общих папок. Общие папки в Exchange используйте разработки специализированных почтового ящика (вместо базы данных общих папок) для хранения иерархии общих папок и содержимого общей папки. Управление разрешениями для общих папок выполняется через роль на основе Access элемента управления (RBAC).
  
Технологии доступа к клиента, таких как веб-служб Exchange (EWS) и управляемый API веб-служб Exchange, предоставляют программный доступ к иерархии общих папок и элементов контента в базу данных общих папок. В этой статье представлены сведения об использовании веб-служб Exchange и управляемый API веб-служб Exchange для доступа к общих папок и общих папок и общих папок. 
  
## <a name="ews-operations-and-ews-managed-api-methods-for-public-folder-access"></a>Операции EWS и управляемый API EWS методы для доступа к общей папке
<a name="bk_functionality"> </a>

Большая часть основных операций веб-служб Exchange поддерживает доступ к общим папкам. Операции, папок и элементов и управляемый API EWS методы, перечисленные в следующей таблице можно использовать для работы с общедоступными папками.
  
Сведения о методах управляемый API EWS [Управляемый API EWS](http://msdn.microsoft.com/en-us/library/jj220535%28v=exchg.80%29.aspx)см.
  
|**Операция служб EWS**|**Метод управляемого API EWS**|
|:-----|:-----|
|[CreateFolder Operation](http://msdn.microsoft.com/library/6f6c334c-b190-4e55-8f0a-38f2a018d1b3%28Office.15%29.aspx) <br/> |**Folder.Save()** <br/> |
|[Операцию UpdateFolder](http://msdn.microsoft.com/library/3494c996-b834-4813-b1ca-d99642d8b4e7%28Office.15%29.aspx) <br/> |**Folder.Update()** <br/> |
|[Операция DeleteFolder](http://msdn.microsoft.com/library/b0f92682-4895-4bcf-a4a1-e4c2e8403979%28Office.15%29.aspx) <br/> |**Folder.Delete()** <br/> |
|[Операция MoveFolder](http://msdn.microsoft.com/library/c7233966-6c87-4a14-8156-b1610760176d%28Office.15%29.aspx) <sup>1</sup> <br/> |**Folder.Move()** <br/> |
|[Операция CopyFolder](http://msdn.microsoft.com/library/c7ea0d68-9793-4144-b378-d99536776db9%28Office.15%29.aspx) <sup>2</sup> <br/> |**Folder.Copy()** <br/> |
|[GetFolder Operation](http://msdn.microsoft.com/library/355bcf93-dc71-4493-b177-622afac5fdb9%28Office.15%29.aspx) <br/> |**Folder.Bind()** <br/> |
|[Операция EmptyFolder](http://msdn.microsoft.com/library/98161486-e2f2-480f-8d5d-708ba81b208a%28Office.15%29.aspx) <sup>3</sup> <br/> |**Folder.Empty()** <br/> |
|[FindFolder Operation](http://msdn.microsoft.com/library/7a9855aa-06cc-45ba-ad2a-645c15b7d031%28Office.15%29.aspx) <br/> |**ExchangeService.FindFolders()** <br/> **Folder.FindFolders()** <br/> |
|[CreateItem Operation](http://msdn.microsoft.com/library/78a52120-f1d0-4ed7-8748-436e554f75b6%28Office.15%29.aspx) <br/> |**Item.Save()** <br/> |
|[MoveItem Operation](http://msdn.microsoft.com/library/dcf40fa7-7796-4a5c-bf5b-7a509a18d208%28Office.15%29.aspx) <br/> |**Item.Move()** <br/> |
|[CopyItem Operation](http://msdn.microsoft.com/library/bcc68f9e-d511-4c29-bba6-ed535524624a%28Office.15%29.aspx) <br/> |**Item.Copy()** <br/> |
|[UpdateItem Operation](http://msdn.microsoft.com/library/5d027523-e0bc-4da2-b60b-0cb9fc1fdfe4%28Office.15%29.aspx) <br/> |**Item.Update()** <br/> |
|[Операция DeleteItem](http://msdn.microsoft.com/library/3e26c416-fa12-476e-bfd2-5c1f4bb7b348%28Office.15%29.aspx) <br/> |**Item.Delete()** <br/> |
|[Операция FindItem](http://msdn.microsoft.com/library/ebad6aae-16e7-44de-ae63-a95b24539729%28Office.15%29.aspx) <sup>4</sup> <br/> |**ExchangeService.FindItems()** <br/> **Folder.FindItems()** <br/> |
|[GetItem Operation](http://msdn.microsoft.com/library/e3590b8b-c2a7-4dad-a014-6360197b68e4%28Office.15%29.aspx) <br/> |**Item.Bind()** <br/> |
|[Операция ConvertId](http://msdn.microsoft.com/library/47d96cf6-9e2f-4fc0-9682-7258d3fbf918%28Office.15%29.aspx) <sup>5</sup> <br/> |**ExchangeService.ConvertId()** <br/> **ExchangeService.ConvertIds()** <br/> |
   
<sup>1</sup> перемещать папки между общих папок и личной папки недоступен в версиях Exchange, начиная с Exchange 2013. 
  
<sup>2</sup> эта операция применима только общие папки в Exchange Server 2007 и Exchange Server 2010. 
  
<sup>3</sup> эта операция применима только для общих папок в Exchange 2010. 
  
<sup>4</sup> индексированных полнотекстовый поиск в рамках одной общей папки с помощью параметра строки запроса поиска поддерживается в версиях Exchange, начиная с Exchange 2013. 
  
<sup>5</sup> ConvertId операция не преобразует правильно идентификаторы общедоступных папок из идентификатора веб-служб Exchange на идентификатор хранилища. Идентификатор, который возвращается в качестве [обходной путь](http://msdn.microsoft.com/library/47d96cf6-9e2f-4fc0-9682-7258d3fbf918%28Office.15%29.aspx#bk_usingConvertId)можно обновлять вручную.
  
Следующие операции не поддерживаются или частично поддерживаются, для общих папок в версиях Exchange, начиная с Exchange 2013:
  
- **CopyFolder** (не поддерживается). **CreateFolder** с операцией **CopyItems** можно использовать для реализации функций **CopyFolder** операции. 
    
- **EmptyFolder** (не поддерживается). **FindItem** с операцией **DeleteItem** можно использовать для реализации функций **EmptyFolder** операции. 
    
- **MoveFolder** (частично поддерживаемая функция). Нельзя перемещать папки между частных и общих папок. Можно перемещать папки между частных и общих папок в Exchange 2007 и Exchange 2010. Вы можете переместить папок в общедоступной папке во всех версиях Exchange. 
    
Веб-служб Exchange и управляемый API EWS не поддерживают следующие функциональные возможности для общих папок:
  
- С помощью **SyncFolderHierarchy**. Использование операций **FindFolder**, **GetFolder** и **SyncFolderItems** для синхронизации элементов и папок в почтовом ящике общих папок. 
    
- Выполняет обход глубокое иерархии общедоступных папок. Использование рекурсивный **FindFolder** вызовы операции для всей иерархии общедоступных папок. 
    
- Создание иерархии папок для общих папок с помощью операции **CreateFolderPath** . Необходимо будет использовать операцию **CreateFolder** для каждого уровня папки в иерархии отдельных папок при разработке почтового ящика общедоступных папок. 
    
- С помощью операции **CreateItem** для сохранения копии сообщений, отправленных по электронной почте. Вместо этого используйте операцию **MoveItem** Перемещение копии сообщения в общую папку. 
    
## <a name="scenarios-for-using-ews-and-the-ews-managed-api-to-work-with-public-folders"></a>Сценарии для использования веб-служб Exchange и управляемый API EWS для работы с общими папками
<a name="bk_scenarios"> </a>

Общие папки включите самые разные сценарии важные для почтовых ящиков пользователей Exchange. Пользователи могут взаимодействовать с помощью веб-служб Exchange и управляемый API EWS для реализации пользовательских решений на доступ и использование общих папок и их содержимое. 
  
### <a name="programmatically-access-email-messages-that-have-been-sent-to-distribution-lists"></a>Программного доступа сообщения электронной почты, отправленных в списки рассылки

Пользователи почтовых ящиков Exchange можно использовать общие папки для хранения сообщений электронной почты, отправленных в списки рассылки. Это удобный способ сохранения истории списка рассылки. Можно использовать [операцию FindItem](http://msdn.microsoft.com/library/ebad6aae-16e7-44de-ae63-a95b24539729%28Office.15%29.aspx) в веб- или методы **ExchangeService.FindItems()** и **Folder.FindItems()** в управляемый API веб-служб Exchange для доступа к сообщениям электронной почты списка сохраненных рассылки. 
  
### <a name="share-important-email-messages-and-other-mailbox-items"></a>Обмен сообщениями важные электронной почты и другие элементы почтового ящика

Пользователи почтовых ящиков можно использовать общедоступные папки как общее хранилище для элементов почтового ящика. Различных пользователей в организации может совместно использовать важные сообщения и контакты, с помощью общих папок. Веб-служб Exchange можно предоставить доступ к этим элементам общего почтового ящика. [Операция MoveItem](http://msdn.microsoft.com/library/dcf40fa7-7796-4a5c-bf5b-7a509a18d208%28Office.15%29.aspx) в веб-служб Exchange или с помощью метода **Item.Move()** в управляемый API веб-служб Exchange можно использовать для перемещения сообщений электронной почты, контакты и другие элементы почтового ящика в и из общей папки. 
  
### <a name="public-discussions-with-post-items"></a>Открытые обсуждения с элементами post

Общие папки — это удобный контейнер для элементов, post. Элементы предусмотрена возможность использовать потоки, не создавая отправлять сообщения электронной почты между пользователями. Пользователи могут использовать общедоступные папки и публиковать элементы для размещения и обслуживания цепочек обсуждений между разных почтовых ящиков пользователей в организации. Таким образом, пользователей почтовых ящиков можно получить доступ к общей журнал беседы, что использует публиковать элементы, даже в том случае, если они не были частью беседы. Как создать и отвечать на публиковать элементы, хранящиеся в общей папке можно использовать [операции CreateItem](http://msdn.microsoft.com/library/78a52120-f1d0-4ed7-8748-436e554f75b6%28Office.15%29.aspx) в веб-служб Exchange или с помощью метода **Item.Save()** в управляемый API веб-служб Exchange. 
  
## <a name="routing-public-folder-requests"></a>Маршрутизация запросов общих папок
<a name="bk_routing"> </a>

Содержимое общих папок могут храниться на нескольких серверах почтовых ящиков. Иерархия общедоступных папок могут храниться на один почтовый ящик во время хранения контента для общих папок на другой. И каждый из этих серверов может отличаться от сервера почтовых ящиков для пользователя, запрашивающего сведения. В этих случаях важно включить дополнительные заголовки X AnchorMailbox и X-PublicFolderMailbox в общей папки запросы на получение точная информация об общих папках.
  
Значение X-AnchorMailbox и X-PublicFolderMailbox может отличаться в зависимости от того, является ли для выполнения запроса, связанные с иерархии папок или содержимого папки. В следующей таблице указываются какие процедуру необходимо выполнить для каждого метода управляемый API EWS или операции веб-служб Exchange.
  
**Управляемый API EWS методы и операции веб-служб Exchange для маршрутизации запросов общих папок**

|**При вызове этих методов**|**При вызове этих операций**|**Используйте эту процедуру**|
|:-----|:-----|:-----|
|[Folder.FindFolders](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.folder.findfolders%28v=exchg.80%29.aspx) <br/> [Folder.Delete](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.folder.delete%28v=exchg.80%29.aspx) <br/> [Folder.Update](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.folder.update%28v=exchg.80%29.aspx) <br/> [Folder.Move](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.folder.move%28v=exchg.80%29.aspx) <br/> |[CreateFolder](http://msdn.microsoft.com/library/6f6c334c-b190-4e55-8f0a-38f2a018d1b3%28Office.15%29.aspx) <br/> [FindFolder](http://msdn.microsoft.com/library/7a9855aa-06cc-45ba-ad2a-645c15b7d031%28Office.15%29.aspx) <br/> [DeleteFolder](http://msdn.microsoft.com/library/b0f92682-4895-4bcf-a4a1-e4c2e8403979%28Office.15%29.aspx) <br/> [UpdateFolder](http://msdn.microsoft.com/library/3494c996-b834-4813-b1ca-d99642d8b4e7%28Office.15%29.aspx) <br/> [MoveFolder](http://msdn.microsoft.com/library/c7233966-6c87-4a14-8156-b1610760176d%28Office.15%29.aspx) <br/> |Маршрутизация запросов иерархии общедоступных папок  <br/> |
|[Item.Bind](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.item.bind%28v=exchg.80%29.aspx) <br/> [Item.Update](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.item.update%28v=exchg.80%29.aspx) <br/> [Item.Copy](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.item.copy%28v=exchg.80%29.aspx) <br/> [Item.Move](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.item.move%28v=exchg.80%29.aspx) <br/> [Item.Delete](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.item.delete%28v=exchg.80%29.aspx) <br/> [Folder.Bind](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.folder.bind%28v=exchg.80%29.aspx) <br/> [Folder.FindItems](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.folder.finditems%28v=exchg.80%29.aspx) <br/> |[CreateItem](http://msdn.microsoft.com/library/78a52120-f1d0-4ed7-8748-436e554f75b6%28Office.15%29.aspx) <br/> [GetItem](http://msdn.microsoft.com/library/e3590b8b-c2a7-4dad-a014-6360197b68e4%28Office.15%29.aspx) <br/> [UpdateItem](http://msdn.microsoft.com/library/5d027523-e0bc-4da2-b60b-0cb9fc1fdfe4%28Office.15%29.aspx) <br/> [CopyItem](http://msdn.microsoft.com/library/bcc68f9e-d511-4c29-bba6-ed535524624a%28Office.15%29.aspx) <br/> [MoveItem](http://msdn.microsoft.com/library/dcf40fa7-7796-4a5c-bf5b-7a509a18d208%28Office.15%29.aspx) <br/> [DeleteItem](http://msdn.microsoft.com/library/3e26c416-fa12-476e-bfd2-5c1f4bb7b348%28Office.15%29.aspx) <br/> [GetFolder](http://msdn.microsoft.com/library/355bcf93-dc71-4493-b177-622afac5fdb9%28Office.15%29.aspx) <br/> [FindItem](http://msdn.microsoft.com/library/ebad6aae-16e7-44de-ae63-a95b24539729%28Office.15%29.aspx) <br/> |Маршрутизация запросов контента общей папки  <br/> |
   
## <a name="version-differences"></a>Различия версий
<a name="VersionDifferences"> </a>

В Exchange 2007 и Exchange 2010 операция **ConvertId** работу при преобразовании идентификаторы общедоступных папок из идентификатора веб-служб Exchange на идентификатор хранилища. 
  
## <a name="see-also"></a>См. также


- [Разработка клиентов веб-служб для Exchange](develop-web-service-clients-for-exchange.md)
    
- [Начать работу с использованием веб-служб Exchange](start-using-web-services-in-exchange.md)
    
- [Ограничения для общих папок](http://technet.microsoft.com/en-us/library/dn594582%28v=exchg.150%29.aspx)
    
- [Вопросы и ответы: Общедоступные папки](http://technet.microsoft.com/en-us/library/jj552408.aspx)
    
- [Процедуры общих папок](http://technet.microsoft.com/en-us/library/jj657481.aspx)
    

