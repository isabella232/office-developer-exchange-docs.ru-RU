---
title: Удаление элементов с помощью веб-служб Exchange в Exchange
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
localization_priority: Normal
ms.assetid: c81e3160-e12b-47e0-b3d6-4be28537f301
description: Узнайте, как использовать управляемый API EWS или веб-службах Exchange для удаления элементов, либо при перемещении их в папку Удаленные или в корзину.
ms.openlocfilehash: a475ebc6677e5f5003cc790a2d4d2b83c513f309
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/11/2018
ms.locfileid: "19760962"
---
# <a name="deleting-items-by-using-ews-in-exchange"></a>Удаление элементов с помощью веб-служб Exchange в Exchange

Узнайте, как использовать управляемый API EWS или веб-службах Exchange для удаления элементов, либо при перемещении их в папку Удаленные или в корзину.
  
Вы когда-либо обратились самостоятельно является различие между перемещение элементов папки «Удаленные», а также сдвиг их в корзину? Может быть интересно различные варианты для обработки удаленных элементов и как реализовать эти параметры в приложении. Веб-служб Exchange (EWS) включает в себя три варианта для обработки удаленных элементов. В этой статье будет надеюсь снимите все путаницы, следует подумать о различиях между ними.
  
## <a name="deleting-items---what-are-my-options"></a>Удаление элементов - параметры?
<a name="bk_DeletingItemsOptions"> </a>

Прежде чем можно понять общий альбомная для удаления элементов, важно понять разницу между следующее:
  
- Папки «Удаленные» — при удалении элементов в почтовом ящике, это куда они.
    
- Корзина (также называемого папка элементов для восстановления) — при удалении элементов из почтового ящика, это куда они.
    
Рисунки 1 и 2 показано, как выглядит процесс удаления элементов и папок в почтовом ящике. 

**На рисунке 1. Процесс удаления элементов из почтового ящика**

![Иллюстрация, показывающая where элементов перейти, когда они будут удалены. Удаленные элементы перемещаются в папку «Удаленные» и перемещаются в папку элементов для восстановления в политику хранения, где они истечения срока действия и permantently удалены.](media/Ex_DeleteItems_Source.png)

<br/>

**На рисунке 2. Процесс удаления папки из почтового ящика**

![Иллюстрация, на которой показан способ перемещения удаленных папок в папку "Удаленные", откуда их можно окончательно удалить из почтового ящика.](media/Ex_.png)
   
Можно удалить элементов и папок тремя разными способами, в зависимости от того, как «постоянные», предоставляемых удаления быть.
  
**Таблица 1: Параметры для удаления элементов с помощью веб-служб Exchange**

|**Возможные варианты**|**Что происходит**|
|:-----|:-----|
|Перемещение папки "Удаленные"  <br/> |Этот способ наименее постоянная удалять элементы.<br/><br/>Это как выравнивание часть документ в корзины с на рабочем месте. Можно легко отобразить его, если это необходимо.<br/><br/>Можно использовать любые [операции удаления](deleting-items-by-using-ews-in-exchange.md#bk_howdoIdeleteitems) , который реализует переход на параметр папку Deleted Items для выполнения этого действия.<br/><br/>Также можно использовать [операцию MoveFolder](http://msdn.microsoft.com/library/c7233966-6c87-4a14-8156-b1610760176d%28Office.15%29.aspx) ( [Folder.Move()](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.folder.move%28v=exchg.80%29.aspx)) или [MoveItem операции](http://msdn.microsoft.com/library/dcf40fa7-7796-4a5c-bf5b-7a509a18d208%28Office.15%29.aspx) ( [Item.Move()](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.item.move%28v=exchg.80%29.aspx)) для перемещения элемента или папки для папки «Удаленные».  <br/> |
|Обратимым удалением  <br/> |Перемещено в папку Удаленные элементы в корзине.<br/><br/>Это как очистите корзину в curbside контейнер. Можно получить доступ элемент, если требуется, это лишь немного сложнее.  <br/><br/>Дополнительные сведения о корзины (также называемая папки элементов для восстановления) и сценарии, такие как обнаружение электронных данных или судебного удержания, ознакомьтесь с разделом [Папки восстанавливаемых элементов](http://technet.microsoft.com/en-us/library/ee364755%28v=exchg.150%29.aspx) на сайте TechNet.<br/><br/>Программных удалений не рекомендуется для приложений, предназначенных для Exchange 2007. В Exchange 2007, использования программных удалений обрабатываются параметр немного на элемент, чтобы указать, что он перемещается в корзину на неопределенное время.<br/><br/>Обходы обратимым удалением или поиск элементов, которые были программных удален с помощью [операции FindItem](http://msdn.microsoft.com/library/ebad6aae-16e7-44de-ae63-a95b24539729%28Office.15%29.aspx), не поддерживается в Exchange Online, Exchange Online как часть Office 365 и версии Exchange, начиная с Exchange 2010.  <br/><br/>**Примечание**: папок Мягкая удалить невозможно.           |
|Окончательного удаления  <br/> |Окончательно удалить элемент или папку.<br/><br/>Удаленные элементы помещаются в папку удаляет из корзины. Это, как и когда утилизации грузовик приводит к очистке curbside recycle контейнера. Элементы, которые не были доступны из клиента электронной почты как Outlook или Outlook Web App и при отсутствии удержания установленный для почтового ящика элементы будут окончательно удалены после определенного периода времени.<br/><br/>Можно получить дополнительные о хранение объектов в статье [Настройка параметре хранение удаленных записей и восстанавливаемых элементов квот](http://technet.microsoft.com/en-us/library/ee364752%28v=exchg.150%29.aspx).<br/><br/>**Примечание**: папки не размещаются в папке удаляет при серьезный удаляются. Удаленных папок, удаляются из почтового ящика.  |
   
Перемещение папки «Удаленные» и параметры окончательного удаления транзакций, что означает, что время завершения вызова веб-службы, элемент был перемещен для папки «Удаленные» или корзины.
  
Помогут вам лучше понять экосистеме папки, которые используются для хранения удаленных элементов на следующем рисунке показана что иерархии папок, которые могут содержать удаленных элементов. Имена папок, как они отображаются в тип схемы **DistinguishedFolderIdNameType** или перечисление **WellKnownFolderName** в управляемый API веб-служб Exchange. 
  
**На рисунке 3. Иерархия папок, содержащих "Удаленные"**

![Изображение иерархии папок для удаленных элементов в основном и архивном почтовых ящиках. Каждая папка на рисунке представлена ее уникальным именем.](media/Ex_FolderHierarchyDeletedItems.png)
  
**В таблице 2: Папок, содержащих удаленных элементов**

|**Имя папки**|**Представлены в**|**Описание**|
|:-----|:-----|:-----|
|deleteditems  <br/> |Exchange 2007  <br/> |По умолчанию папки "Удаленные". Элементы остаются в этой папке до их или жестко удаленные или пока период хранения превышена. Затем они перемещаются в папку в корзину. Удаленные папки помещаются в папку «Удаленные», и время, когда он или жестко удаленные, они будут окончательно удалены из почтового ящика и, восстановить невозможно.  <br/> |
|recoverableitemsroot  <br/> |Exchange 2010  <br/> |В корневой каталог корзины, или папки элементов для восстановления. Корзины доступ был реализован в веб-службах Exchange 2010. Отображаемое имя для этой папки — «Элементов для восстановления».  <br/> |
|recoverableitemsdeletions  <br/> |Exchange 2010  <br/> |Основной корзины папок для почтового ящика. Удаленные элементы и элементы перемещаются из папки "Удаленные" политикой хранения помещаются в этой папке. Отображаемое имя для этой папки — «Удаление».  <br/> |
|recoverableitemsversions  <br/> |Exchange 2010  <br/> |Где хранятся старые версии элемента. Старые версии элемента создаются при обновлении элемента. Черновых версий элемента не сохраняются в этой папке. Отображаемое имя этой папки — «Версии».  <br/> |
|recoverableitemspurges  <br/> |Exchange 2010  <br/> |Где хранятся элементы, удаленные из папки "Удаленные элементы". Все элементы хранения удаленных перемещаются в эту папку. Отображаемое имя для этой папки — «Удаление».  <br/> |
|archiveddeletedtitems  <br/> |Exchange 2010  <br/> |По умолчанию папки "Удаленные" для архивного почтового ящика.  <br/> |
|archiverecoverablesitemsroot  <br/> |Exchange 2010  <br/> |Корневой корзины папок для архивного почтового ящика. Архивные элементы, удаленные перемещаются в папке в этой папке.  <br/> |
|archiverecoverableitemsdeletions  <br/> |Exchange 2010  <br/> |Основной корзины папок для архивного почтового ящика. Архивируются элементы помещаются в корзину помещаются здесь.  <br/> |
|archiverecoverableitemsversions  <br/> |Exchange 2010  <br/> |Где хранятся старые версии архивных элементов.  <br/> |
|archiverecoverableitemspurges  <br/> |Exchange 2010  <br/> |Где элементов, которые удаляется из архива удалений папки в корзине хранятся. Все элементы-удаления хранилища архивации перемещаются в эту папку.  <br/> |
   
## <a name="how-do-i-delete-items"></a>Удаление элементов
<a name="bk_howdoIdeleteitems"> </a>

Удалить, выполните одну из следующих значений, чтобы указать, следует ли переместить элемент папки «Удаленные» или выполнить мягкое или жестко:
  
- **DisposalType** простой тип, при использовании веб-служб Exchange для доступа к Exchange. 
    
- [Перечисление DeleteMode](http://msdn.microsoft.com/en-us/library/exchange/microsoft.exchange.webservices.data.deletemode%28v=exchg.80%29.aspx), если используется управляемый API веб-служб Exchange.
    
Количество различных операций веб-служб Exchange или управляемый API EWS методы можно использовать для удаления элементов и папок из почтового ящика.
  
**В таблице 3: Операции веб-служб Exchange и методы управляемый API веб-служб Exchange для удаления элементов**

|**Операция служб EWS**|**Метод управляемого API EWS**|**Представлены в**|**Назначение**|
|:-----|:-----|:-----|:-----|
|[Операция DeleteFolder](http://msdn.microsoft.com/library/b0f92682-4895-4bcf-a4a1-e4c2e8403979%28Office.15%29.aspx) <br/> |[Метод Folder.Delete](http://msdn.microsoft.com/en-us/library/exchange/microsoft.exchange.webservices.data.folder.delete%28v=exchg.80%29.aspx) <br/> |Exchange 2007  <br/> |Удаление папки из почтового ящика. С помощью веб-служб Exchange можно пакетного удаление папок. С помощью управляемый API веб-служб Exchange можно удалить только одной папке на вызов.  <br/> |
|[Операция DeleteItem](http://msdn.microsoft.com/library/3e26c416-fa12-476e-bfd2-5c1f4bb7b348%28Office.15%29.aspx) <br/> |[Метод Item.Delete](http://msdn.microsoft.com/en-us/library/exchange/microsoft.exchange.webservices.data.item.delete%28v=exchg.80%29.aspx)<br/><br/>[Метод ExchangeService.DeleteItems](http://msdn.microsoft.com/en-us/library/exchange/microsoft.exchange.webservices.data.exchangeservice.deleteitems%28v=exchg.80%29.aspx) <br/> |Exchange 2007  <br/> |Удаление элементов из почтового ящика.  <br/> |
|[Операция EmptyFolder](http://msdn.microsoft.com/library/98161486-e2f2-480f-8d5d-708ba81b208a%28Office.15%29.aspx) <br/> |[Метод Folder.Empty](http://msdn.microsoft.com/en-us/library/exchange/microsoft.exchange.webservices.data.folder.empty%28v=exchg.80%29.aspx) <br/> |Exchange 2010  <br/> |Удаляет все элементы в папке, а при необходимости, удаляет все вложенные папки в папке.  <br/> |
|[Операция ApplyConversationAction](http://msdn.microsoft.com/library/73d7943d-d361-4f8b-9948-d85f886efa1a%28Office.15%29.aspx) <br/> |[Метод Conversation.EnableAlwaysDeleteItems](http://msdn.microsoft.com/en-us/library/exchange/microsoft.exchange.webservices.data.conversation.enablealwaysdeleteitems%28v=exchg.80%29.aspx)<br/><br/>[Метод Conversation.DeleteItems](http://msdn.microsoft.com/en-us/library/exchange/microsoft.exchange.webservices.data.conversation.deleteitems%28v=exchg.80%29.aspx) <br/> |Exchange 2010  <br/> |Задание удаления обработки действий в сообщениях электронной почты в беседе, чтобы они будут удалены.  <br/> |
|[Операция DeleteUserConfiguration](http://msdn.microsoft.com/library/93e44690-be2d-4fdb-96a8-4ded3c193aed%28Office.15%29.aspx) <br/> |[Метод UserConfiguration.Delete](http://msdn.microsoft.com/en-us/library/exchange/microsoft.exchange.webservices.data.userconfiguration.delete%28v=exchg.80%29.aspx) <br/> |Exchange 2010  <br/> |Удаляет папку связанных элементов и переводит его в корзину.  <br/> |
|[CreateItem Operation](http://msdn.microsoft.com/library/78a52120-f1d0-4ed7-8748-436e554f75b6%28Office.15%29.aspx) <br/> |[Метод Appointment.Accept](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.appointment.accept%28v=exchg.80%29.aspx) <br/><br/>[Метод Appointment.AcceptTentatively](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.appointment.accepttentatively%28v=exchg.80%29.aspx)<br/><br/>[Метод Appointment.CancelMeeting](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.appointment.cancelmeeting%28v=exchg.80%29.aspx)<br/><br/>[Appointment.Decline](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.appointment.decline%28v=exchg.80%29.aspx)<br/><br/>[Метод MeetingRequest.Accept](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.meetingrequest.accept%28v=exchg.80%29.aspx)<br/><br/>[Метод MeetingRequest.AcceptTentatively](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.meetingrequest.accepttentatively%28v=exchg.80%29.aspx)<br/><br/>[Метод MeetingRequest.Decline](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.meetingrequest.decline%28v=exchg.80%29.aspx) <br/> |Exchange 2007  <br/> |Косвенно перемещает элемент папки «Удаленные» каждый раз, когда отправляется ответ на приглашения на собрание или установлено ответ для встречи.<br/><br/>Тип удаления установлено на этой операции. Сообщения собрания перемещаются папки "Удаленные", когда объект ответа успешно обработан службой.  <br/> |
   
Перемещение элементов папки «Удаленные» можно также с помощью правила папки «Входящие». Например можно [создавать правила](inbox-management-and-ews-in-exchange.md) , для которого действие удаления. 
  
Некоторые замечания об удалении элементов:
  
- Удаление вхождения повторяющегося элемента не вызывает переход в папку «Удаленные» или корзины. В результате обновление для повторяющегося элемента главных ряда повторяющейся.
    
- Папки по умолчанию нельзя удалить из почтового ящика.
    
- Отменить удаление встречи или сообщения о собраниях, например, приглашений на собрания, а или обновлений встреч. Вместо этого ответ на эти элементы с помощью объектов ответа. Таким образом, элементы календаря связанного обновляются в соответствии с действиями пользователя ответчика или организатора.
    
- Ключ изменения элемента не обновляются при перемещении элемента в папку Deleted Items или удалять.
    
- При выполнении жестко удаления элемента и затем вызвать [SyncFolderHierarchy операции](http://msdn.microsoft.com/library/b31916b1-bc6c-4451-a475-b7c5417f752d%28Office.15%29.aspx) или метод управляемый API EWS [SyncFolderHierarchy](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.exchangeservice.syncfolderhierarchy%28v=exchg.80%29.aspx) или [SyncFolderItems операции](http://msdn.microsoft.com/library/7f0de089-8876-47ec-a871-df118ceae75d%28Office.15%29.aspx) или [SyncFolderItems](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.exchangeservice.syncfolderitems%28v=exchg.80%29.aspx) метода, изменение, **Удаление** будут возвращены запись. При перемещении элемента в папку Deleted Items возвращается записи изменений **обновления** . Это, так как элемент или папку, будут иметь новое значение свойства [ParentFolderId](http://msdn.microsoft.com/library/258f4b1f-367e-4c7d-9c29-eb775a2398c7%28Office.15%29.aspx) . [Более подробные сведения о синхронизации](mailbox-synchronization-and-ews-in-exchange.md) при синхронизации удаленных элементов является частью сценария. 
    
## <a name="find-out-more-about-deleting-items"></a>Дополнительные сведения о удаление элементов
<a name="findoutmore"> </a>

- [По запросу уведомления для событий, связанных с удаления почтового ящика веб-служб Exchange в Exchange](pull-notifications-for-ews-deletion-related-mailbox-events-in-exchange.md)
    
- [Обработка ошибок, связанных с удаления в веб-служб Exchange в Exchange](handling-deletion-related-errors-in-ews-in-exchange.md)
    
## <a name="see-also"></a>См. также

- [Папки и элементы в веб-службах Exchange](folders-and-items-in-ews-in-exchange.md)    
- [Разработка клиентов веб-служб для Exchange](develop-web-service-clients-for-exchange.md)    
- [Папка элементов для восстановления](http://technet.microsoft.com/en-us/library/ee364755.aspx)    
- [Функцию восстановления отдельных элементов в Exchange Server 2010](http://blogs.technet.com/b/exchange/archive/2009/09/25/3408389.aspx#_Single_Item_Recovery)    
- [Exchange 2013: Удаление повторяющихся серии программными средствами с серверов Exchange](http://code.msdn.microsoft.com/exchange/Exchange-2013-Delete-a-e1c7b89d)    
- [Exchange 2013: Удаление задачи из учетной записи на серверах Exchange программным путем](http://code.msdn.microsoft.com/exchange/Exchange-2013-Delete-tasks-13824637)    
- [Exchange 2013: Очистите папки на серверах Exchange программным путем](http://code.msdn.microsoft.com/exchange/Exchange-2013-Empty-6487df37)    
- [Exchange 2013: Удаление папок программными средствами с серверов Exchange](http://code.msdn.microsoft.com/exchange/Exchange-2013-Delete-aa1a5823)    
- [Exchange 2013: Удаление много элементов программными средствами с серверов Exchange](http://code.msdn.microsoft.com/exchange/Exchange-2013-Delete-many-064f8760)    
- [Exchange 2013: Удаление контактов программными средствами с серверов Exchange](http://code.msdn.microsoft.com/exchange/Exchange-2013-Delete-3b8b0640)    
- [Удаление встреч и отмены собраний с помощью веб-служб Exchange в Exchange](how-to-delete-appointments-and-cancel-meetings-by-using-ews-in-exchange.md)    
- [Управление параметрами сохраняемого приложения с помощью веб-служб Exchange в Exchange](how-to-manage-persistent-application-settings-by-using-ews-in-exchange.md)
    

