---
title: Общих папок в Exchange доступ с EWS
manager: sethgros
ms.date: 7/17/2015
ms.audience: Developer
ms.assetid: d9372057-1deb-45de-8f98-b9149604429a
description: Узнайте, как использовать веб-службы EWS и управляемый API EWS для доступа к общедоступным папкам и запросам общедоступных папок в Exchange.
localization_priority: Priority
ms.openlocfilehash: e921a77b250e11e974b0c47b1d28a8e020837d44
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/03/2020
ms.locfileid: "44460213"
---
# <a name="public-folder-access-with-ews-in-exchange"></a>Общих папок в Exchange доступ с EWS

Узнайте, как использовать веб-службы EWS и управляемый API EWS для доступа к общедоступным папкам и запросам общедоступных папок в Exchange.
  
Общедоступные папки предоставляют общий репозиторий элементов, к которым пользователи в вашей организации могут получать доступ. Office 365, Exchange Online и локальная версия Exchange, начиная с Exchange 2013, вводят новую архитектуру для общедоступных папок. Общедоступные папки в Exchange используют специализированный дизайн почтовых ящиков (вместо базы данных общедоступных папок) для хранения иерархии общедоступных папок и содержимого общедоступных папок. Разрешения для общедоступных папок управляются с помощью управления доступом на основе ролей (RBAC).
  
Клиентские технологии клиентского доступа, например веб-службы Exchange (EWS) и управляемый API EWS, предоставляют программный доступ к иерархии общедоступных папок и элементам содержимого в базе данных общедоступных папок. В этой статье приводятся сведения о том, как использовать EWS и управляемый API EWS для доступа к общедоступным папкам и общедоступным папкам и данным общедоступных папок. 
  
## <a name="ews-operations-and-ews-managed-api-methods-for-public-folder-access"></a>Операции служб EWS и методы управляемого API EWS для доступа к общедоступным папкам
<a name="bk_functionality"> </a>

Большинство основных операций EWS поддерживают доступ к общедоступным папкам. Для работы с общедоступными папками можно использовать операции с папками и элементами, а также методы управляемого API EWS, приведенные в следующей таблице.
  
Дополнительные сведения о методах управляемого API EWS приведены в статье [пространства имен управляемого API EWS](https://msdn.microsoft.com/library/jj220535%28v=exchg.80%29.aspx).
  
|**Операция служб EWS**|**Метод управляемого API EWS**|
|:-----|:-----|
|[Операция CreateFolder](https://msdn.microsoft.com/library/6f6c334c-b190-4e55-8f0a-38f2a018d1b3%28Office.15%29.aspx) <br/> |**Folder. Save ()** <br/> |
|[Операция UpdateFolder](https://msdn.microsoft.com/library/3494c996-b834-4813-b1ca-d99642d8b4e7%28Office.15%29.aspx) <br/> |**Folder. Update ()** <br/> |
|[Операция DeleteFolder](https://msdn.microsoft.com/library/b0f92682-4895-4bcf-a4a1-e4c2e8403979%28Office.15%29.aspx) <br/> |**Folder. Delete ()** <br/> |
|[Операция MoveFolder](https://msdn.microsoft.com/library/c7233966-6c87-4a14-8156-b1610760176d%28Office.15%29.aspx)<sup>1</sup> <br/> |**Folder. Move ()** <br/> |
|[Операция CopyFolder](https://msdn.microsoft.com/library/c7ea0d68-9793-4144-b378-d99536776db9%28Office.15%29.aspx)<sup>2</sup> <br/> |**Folder. Copy ()** <br/> |
|[Операция GetFolder](https://msdn.microsoft.com/library/355bcf93-dc71-4493-b177-622afac5fdb9%28Office.15%29.aspx) <br/> |**Folder. bind ()** <br/> |
|[Операция EmptyFolder](https://msdn.microsoft.com/library/98161486-e2f2-480f-8d5d-708ba81b208a%28Office.15%29.aspx)<sup>3</sup> <br/> |**Folder. Empty ()** <br/> |
|[Операция FindFolder](https://msdn.microsoft.com/library/7a9855aa-06cc-45ba-ad2a-645c15b7d031%28Office.15%29.aspx) <br/> |**ExchangeService. Финдфолдерс ()** <br/> **Folder. Финдфолдерс ()** <br/> |
|[Операция CreateItem](https://msdn.microsoft.com/library/78a52120-f1d0-4ed7-8748-436e554f75b6%28Office.15%29.aspx) <br/> |**Item. Save ()** <br/> |
|[Операция MoveItem](https://msdn.microsoft.com/library/dcf40fa7-7796-4a5c-bf5b-7a509a18d208%28Office.15%29.aspx) <br/> |**Item. Move ()** <br/> |
|[Операция CopyItem](https://msdn.microsoft.com/library/bcc68f9e-d511-4c29-bba6-ed535524624a%28Office.15%29.aspx) <br/> |**Item. Copy ()** <br/> |
|[Операция UpdateItem](https://msdn.microsoft.com/library/5d027523-e0bc-4da2-b60b-0cb9fc1fdfe4%28Office.15%29.aspx) <br/> |**Item. Update ()** <br/> |
|[Операция DeleteItem](https://msdn.microsoft.com/library/3e26c416-fa12-476e-bfd2-5c1f4bb7b348%28Office.15%29.aspx) <br/> |**Item. Delete ()** <br/> |
|[Операция FindItem](https://msdn.microsoft.com/library/ebad6aae-16e7-44de-ae63-a95b24539729%28Office.15%29.aspx)<sup>4</sup> <br/> |**ExchangeService. FindItems ()** <br/> **Folder. FindItems ()** <br/> |
|[Операция GetItem](https://msdn.microsoft.com/library/e3590b8b-c2a7-4dad-a014-6360197b68e4%28Office.15%29.aspx) <br/> |**Item. bind ()** <br/> |
|[Операция ConvertId](https://msdn.microsoft.com/library/47d96cf6-9e2f-4fc0-9682-7258d3fbf918%28Office.15%29.aspx)<sup>5</sup> <br/> |**ExchangeService. ConvertId ()** <br/> **ExchangeService. Конвертидс ()** <br/> |
   
<sup>1</sup> перемещение папок между общедоступной папкой и частной папкой недоступно в версиях Exchange, начиная с Exchange 2013. 
  
<sup>2</sup> эта операция применяется только к общедоступным папкам в exchange Server 2007 и exchange Server 2010. 
  
<sup>3</sup> эта операция применяется только к общедоступным папкам в Exchange 2010. 
  
<sup>4</sup> полнотекстовый индексированный поиск в одной общедоступной папке с помощью параметра поиска QueryString поддерживается в версиях Exchange, начиная с Exchange 2013. 
  
<sup>5</sup> операция ConvertId неправильно преобразует идентификаторы общедоступных папок из идентификатора EWS в идентификатор хранилища. Вы можете вручную обновить идентификатор, возвращаемый в качестве [обходного пути](https://msdn.microsoft.com/library/47d96cf6-9e2f-4fc0-9682-7258d3fbf918%28Office.15%29.aspx#bk_usingConvertId).
  
Следующие операции не поддерживаются или частично поддерживаются, для общедоступных папок в версиях Exchange, начиная с Exchange 2013:
  
- **CopyFolder** (не поддерживается). Вы можете использовать **CreateFolder** с операцией **копитемс** , чтобы реализовать функциональные возможности операции **CopyFolder** . 
    
- **EmptyFolder** (не поддерживается). Для реализации функции операции **EmptyFolder** можно использовать **FindItem** с операцией **DeleteItem** . 
    
- **MoveFolder** (частично поддерживается). Папки нельзя перемещать между личными и общедоступными папками. Папки можно перемещать между частными и общедоступными папками в Exchange 2007 и Exchange 2010. Папки в общедоступных папках можно перемещать во всех версиях Exchange. 
    
Веб-интерфейс EWS и управляемый API EWS не поддерживают следующие функции для общедоступных папок:
  
- С помощью **SyncFolderHierarchy**. Используйте операции **FindFolder**, **SyncFolderItems** и **SyncFolderItems** для синхронизации элементов и папок в почтовом ящике общедоступных папок. 
    
- Поиск в иерархии общедоступных папок с глубоким обходом. Использование рекурсивных вызовов операций **FindFolder** для обхода иерархии общедоступных папок. 
    
- Использование операции **CreateFolderPath** для создания иерархии папок для общедоступных папок. При использовании почтового ящика общедоступных папок вам потребуется выполнить операцию **CreateFolder** для каждого уровня папки в иерархии различных папок. 
    
- Использование операции **CreateItem** для сохранения копий отправленных сообщений электронной почты. Вместо этого используйте операцию **MoveItem** , чтобы переместить копию сообщения в общедоступную папку. 
    
## <a name="scenarios-for-using-ews-and-the-ews-managed-api-to-work-with-public-folders"></a>Сценарии использования EWS и управляемого API EWS для работы с общедоступными папками
<a name="bk_scenarios"> </a>

В общедоступных папках для пользователей почтовых ящиков Exchange существует множество важных сценариев. Для реализации пользовательских решений для доступа к общедоступным папкам и их содержимым можно использовать службы EWS и управляемый API EWS. 
  
### <a name="programmatically-access-email-messages-that-have-been-sent-to-distribution-lists"></a>Программный доступ к сообщениям электронной почты, отправленным в списки рассылки

Пользователи почтовых ящиков Exchange могут использовать общедоступные папки для хранения сообщений электронной почты, отправляемых в списки рассылки. Это удобный способ сохранения истории списка рассылки. Для доступа к сохраненным электронным сообщениям списка рассылки можно использовать [операцию FindItem](https://msdn.microsoft.com/library/ebad6aae-16e7-44de-ae63-a95b24539729%28Office.15%29.aspx) или методы **ExchangeService. FindItems ()** и **Folder. FindItems ()** в управляемом API EWS. 
  
### <a name="share-important-email-messages-and-other-mailbox-items"></a>Совместное использование важных сообщений электронной почты и других элементов почтового ящика

Пользователи почтовых ящиков могут использовать общедоступные папки в качестве общего репозитория для элементов почтового ящика. Разные пользователи в организации могут обмениваться важными сообщениями электронной почты или контактами с помощью общедоступных папок. Службы EWS могут предоставлять доступ к этим общим почтовым ящикам. Для перемещения сообщений электронной почты, контактов и других элементов почтовых ящиков в общедоступную папку и из нее можно использовать [операцию MoveItem](https://msdn.microsoft.com/library/dcf40fa7-7796-4a5c-bf5b-7a509a18d208%28Office.15%29.aspx) в EWS или метод **Item. Move ()** в управляемом API EWS. 
  
### <a name="public-discussions-with-post-items"></a>Общедоступные обсуждения с элементами POST

Общедоступные папки — это удобный контейнер для размещения элементов. POST Items предоставляют способ использования потоковых бесед без необходимости отправлять сообщения электронной почты между пользователями. Пользователи могут использовать общедоступные папки и размещать элементы для размещения и обслуживания связанных обсуждений между различными пользователями почтовых ящиков в Организации. Таким образом, пользователи почтовых ящиков могут получить доступ к общему журналу беседы, использующего элементы POST, даже если они не были частью беседы. Можно использовать [операцию CreateItem](https://msdn.microsoft.com/library/78a52120-f1d0-4ed7-8748-436e554f75b6%28Office.15%29.aspx) в EWS или метод **Item. Save ()** в управляемом API EWS для создания элементов и реагирования на них, хранящихся в общедоступной папке. 
  
## <a name="routing-public-folder-requests"></a>Маршрутизация запросов к общедоступным папкам
<a name="bk_routing"> </a>

Содержимое общедоступных папок можно хранить на нескольких серверах почтовых ящиков. Иерархия общедоступных папок может храниться в одном почтовом ящике, а содержимое для общедоступной папки — на другом. Каждый из этих серверов может отличаться от сервера почтовых ящиков для пользователя, запрашивающего информацию. В этом случае важно добавить в общедоступную папку дополнительные заголовки X – AnchorMailbox и X – Публикфолдермаилбокс, чтобы получить точную информацию об общедоступных папках.
  
Значения X – AnchorMailbox и X Публикфолдермаилбокс могут различаться в зависимости от того, выполняется ли запрос, связанный с иерархией папок или содержимым папки. В следующей таблице указана процедура, которую необходимо выполнить для каждого метода управляемого API EWS или операции EWS.
  
**Методы управляемого API EWS и операции EWS для запросов общедоступных папок маршрутизации**

|**При вызове этих методов**|**При вызове этих операций**|**Используйте эту процедуру**|
|:-----|:-----|:-----|
|[Folder. Финдфолдерс](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.folder.findfolders%28v=exchg.80%29.aspx) <br/> [Folder. Delete](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.folder.delete%28v=exchg.80%29.aspx) <br/> [Folder. Update](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.folder.update%28v=exchg.80%29.aspx) <br/> [Папка. Move](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.folder.move%28v=exchg.80%29.aspx) <br/> |[CreateFolder](https://msdn.microsoft.com/library/6f6c334c-b190-4e55-8f0a-38f2a018d1b3%28Office.15%29.aspx) <br/> [FindFolder](https://msdn.microsoft.com/library/7a9855aa-06cc-45ba-ad2a-645c15b7d031%28Office.15%29.aspx) <br/> [DeleteFolder](https://msdn.microsoft.com/library/b0f92682-4895-4bcf-a4a1-e4c2e8403979%28Office.15%29.aspx) <br/> [UpdateFolder](https://msdn.microsoft.com/library/3494c996-b834-4813-b1ca-d99642d8b4e7%28Office.15%29.aspx) <br/> [MoveFolder](https://msdn.microsoft.com/library/c7233966-6c87-4a14-8156-b1610760176d%28Office.15%29.aspx) <br/> |Маршрутизация запросов иерархии общедоступных папок  <br/> |
|[Item.Bind](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.item.bind%28v=exchg.80%29.aspx) <br/> [Item.Update](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.item.update%28v=exchg.80%29.aspx) <br/> [Item. Copy](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.item.copy%28v=exchg.80%29.aspx) <br/> [Элемент. Move](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.item.move%28v=exchg.80%29.aspx) <br/> [Item.Delete](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.item.delete%28v=exchg.80%29.aspx) <br/> [Folder. Bind](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.folder.bind%28v=exchg.80%29.aspx) <br/> [Folder. FindItems](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.folder.finditems%28v=exchg.80%29.aspx) <br/> |[CreateItem](https://msdn.microsoft.com/library/78a52120-f1d0-4ed7-8748-436e554f75b6%28Office.15%29.aspx) <br/> [GetItem](https://msdn.microsoft.com/library/e3590b8b-c2a7-4dad-a014-6360197b68e4%28Office.15%29.aspx) <br/> [UpdateItem](https://msdn.microsoft.com/library/5d027523-e0bc-4da2-b60b-0cb9fc1fdfe4%28Office.15%29.aspx) <br/> [CopyItem](https://msdn.microsoft.com/library/bcc68f9e-d511-4c29-bba6-ed535524624a%28Office.15%29.aspx) <br/> [MoveItem](https://msdn.microsoft.com/library/dcf40fa7-7796-4a5c-bf5b-7a509a18d208%28Office.15%29.aspx) <br/> [DeleteItem](../web-service-reference/deleteitem-operation.md) <br/> [GetFolder](https://msdn.microsoft.com/library/355bcf93-dc71-4493-b177-622afac5fdb9%28Office.15%29.aspx) <br/> [FindItem](https://msdn.microsoft.com/library/ebad6aae-16e7-44de-ae63-a95b24539729%28Office.15%29.aspx) <br/> |Маршрутизация запросов содержимого общедоступных папок  <br/> |
   
## <a name="version-differences"></a>Различия версий
<a name="VersionDifferences"> </a>

В Exchange 2007 и Exchange 2010 операция **ConvertId** работает должным образом при преобразовании идентификаторов общедоступных папок из идентификатора EWS в идентификатор хранилища. 
  
## <a name="see-also"></a>См. также


- [Разработка клиентов веб-служб для Exchange](develop-web-service-clients-for-exchange.md)
    
- [Начало работы с веб-службами Exchange](start-using-web-services-in-exchange.md)
    
- [Пределы для общедоступных папок](https://technet.microsoft.com/library/dn594582%28v=exchg.150%29.aspx)
    
- [Вопросы и ответы: общедоступные папки](https://technet.microsoft.com/library/jj552408.aspx)
    
- [Процедуры для общедоступных папок](https://technet.microsoft.com/library/jj657481.aspx)
    

