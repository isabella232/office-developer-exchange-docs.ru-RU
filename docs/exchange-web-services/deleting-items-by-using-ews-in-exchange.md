---
title: Удаление элементов с помощью EWS в Exchange
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
localization_priority: Normal
ms.assetid: c81e3160-e12b-47e0-b3d6-4be28537f301
description: Сведения о том, как можно использовать управляемый API EWS или EWS в Exchange для удаления элементов, перемещая их в папку "Удаленные" или в корзину.
ms.openlocfilehash: a475ebc6677e5f5003cc790a2d4d2b83c513f309
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/25/2018
ms.locfileid: "19760962"
---
# <a name="deleting-items-by-using-ews-in-exchange"></a>Удаление элементов с помощью EWS в Exchange

Сведения о том, как можно использовать управляемый API EWS или EWS в Exchange для удаления элементов, перемещая их в папку "Удаленные" или в корзину.
  
Вы когда-нибудь запросили разницу между перемещением элементов в папку "Удаленные" и перемещением их в корзину? Возможно, вы хотите узнать о различных вариантах обработки удаленных элементов и о том, как реализовать эти параметры в приложении. Веб-службы Exchange (EWS) включают три варианта обработки удаленных элементов. В этой статье мы будем удалять все различия между ними.
  
## <a name="deleting-items---what-are-my-options"></a>Удаление элементов: что такое "Мои параметры"?
<a name="bk_DeletingItemsOptions"> </a>

Прежде чем вы сможете понять общую ориентацию по удалению элементов, важно понять разницу между следующими особенностями.
  
- Папка "Удаленные" — при удалении элементов в почтовом ящике это место.
    
- Корзина (как и папка "элементы с возможностью восстановления") — при удалении элементов из почтового ящика это место, где они находятся.
    
На рисунках 1 и 2 показано, как выглядит процесс удаления для элементов и папок в почтовом ящике. 

**Рис. 1. Процесс удаления элементов из почтового ящика**

![Иллюстрация, на которой показано, куда попадают удаленные элементы. Удаленные элементы перемещаются в папку "Удаленные", а затем перемещаются в папку "элементы с возможностью восстановления" для каждой политики хранения, срок действия которых истечет и они пермантентли удаляются.](media/Ex_DeleteItems_Source.png)

<br/>

**Рис. 2. Процесс удаления папок из почтового ящика**

![Иллюстрация, на которой показан способ перемещения удаленных папок в папку "Удаленные", откуда их можно окончательно удалить из почтового ящика.](media/Ex_.png)
   
Вы можете удалять элементы и папки тремя различными способами, в зависимости от того, как "постоянное" нужно удалить.
  
**Таблица 1: параметры удаления элементов с помощью EWS**

|**Option**|**Что происходит**|
|:-----|:-----|
|Перемещение в папку удаленных элементов  <br/> |Это наименее постоянный способ удаления элементов.<br/><br/>Это аналогично размещению бумажной бумаги в корзине на рабочем месте. Его можно легко захватить, если это необходимо.<br/><br/>Для выполнения этого действия можно использовать любую [операцию удаления](deleting-items-by-using-ews-in-exchange.md#bk_howdoIdeleteitems) , которая реализует параметр переместить в папку "Удаленные".<br/><br/>Вы также можете использовать [операцию MoveItem](http://msdn.microsoft.com/library/dcf40fa7-7796-4a5c-bf5b-7a509a18d208%28Office.15%29.aspx) ( [Item. Move ()](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.item.move%28v=exchg.80%29.aspx)) или [операцию MoveFolder](http://msdn.microsoft.com/library/c7233966-6c87-4a14-8156-b1610760176d%28Office.15%29.aspx) ( [Folder. Move ()](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.folder.move%28v=exchg.80%29.aspx)), чтобы переместить элемент или папку в папку "Удаленные".  <br/> |
|Обратимое удаление  <br/> |Элемент перемещается в папку "удаления" в корзине.<br/><br/>Это аналогично очистке корзины в контейнере курбсиде. Вы по-прежнему можете получать доступ к элементу, если это необходимо, но немного сложнее.  <br/><br/>Для получения дополнительных сведений о корзине (также называемой папкой "элементы с возможностью восстановления") и сценариями, такими как обнаружение электронных данных и судебное разбирательства, просмотрите [папку элементы с возможностью восстановления](http://technet.microsoft.com/en-us/library/ee364755%28v=exchg.150%29.aspx) на сайте TechNet.<br/><br/>Обратимое удаление не рекомендуется для приложений, предназначенных для Exchange 2007. В Exchange 2007, обратимое удаление обрабатывается путем установки бита для элемента, указывающего на то, что он будет перемещен в корзину в неуказанное время.<br/><br/>При обратимом удалении или поиске элементов, которые были обратимо удалены с помощью [операции FindItem](http://msdn.microsoft.com/library/ebad6aae-16e7-44de-ae63-a95b24539729%28Office.15%29.aspx), не поддерживаются в Exchange Online, Exchange Online в составе Office 365 и версиях Exchange, начиная с Exchange 2010.  <br/><br/>**Note**: папки нельзя удалять с возможностью восстановления.           |
|Необратимое удаление  <br/> |Элемент или папка окончательно удаляется.<br/><br/>Окончательно удаленные элементы помещаются в папку очистки корзины. Это аналогично, когда грузовик перезапуска очищает контейнер курбсиде. Доступ к элементам из почтового клиента, например Outlook или Outlook Web App, невозможен, если для почтового ящика не указан набор удержаний, элементы будут безвозвратно удалены по истечении определенного периода времени.<br/><br/>Дополнительные сведения о хранении элементов можно узнать в статье [Настройка квот хранения удаленных элементов и элементов для восстановления](http://technet.microsoft.com/en-us/library/ee364752%28v=exchg.150%29.aspx).<br/><br/>**Note**: папки не помещаются в папку "очистки" при их окончательном удалении. Окончательно удаленные папки удаляются из почтового ящика.  |
   
Перемещение в папку "Удаленные" и параметры окончательного удаления являются транзакционными, что означает, что при завершении вызова веб-службы элемент был перемещен в папку "Удаленные" или в корзину.
  
Чтобы лучше понять экосистему папок, которые используются для хранения удаленных элементов, на следующем рисунке показана иерархия папок, которые могут содержать удаленные элементы. Имена папок отображаются в соответствии с типом схемы **дистингуишедфолдериднаметипе** или перечислением **веллкновнфолдернаме** в управляемом API EWS. 
  
**Рис. 3. Иерархия папок, содержащих удаленные элементы**

![Изображение иерархии папок для удаленных элементов в основном и архивном почтовых ящиках. Каждая папка на рисунке представлена ее уникальным именем.](media/Ex_FolderHierarchyDeletedItems.png)
  
**Таблица 2: папки, содержащие удаленные элементы**

|**Имя папки**|**Версия, где параметр был представлен**|**Описание**|
|:-----|:-----|:-----|
|deleteditems  <br/> |Exchange 2007  <br/> |Папка "Удаленные", используемая по умолчанию. Элементы хранятся в этой папке до тех пор, пока они не будут мягкими или жестко удалены или пока не будет превышен срок хранения. Затем они перемещаются в папку корзины. Удаленные папки помещаются в папку "Удаленные", а при их обратимом удалении они удаляются из почтового ящика и не могут быть восстановлены.  <br/> |
|рековераблеитемсрут  <br/> |Exchange 2010  <br/> |Корневой каталог корзины или папка "элементы с возможностью восстановления". Доступ к корзине реализован в EWS в Exchange 2010. Отображаемое имя этой папки — "элементы с возможностью восстановления".  <br/> |
|recoverableitemsdeletions  <br/> |Exchange 2010  <br/> |Основная папка корзины для почтового ящика. Обратимо удаленные элементы и элементы, перемещенные из папки "Удаленные" в соответствии с политикой хранения, помещаются в эту папку. Отображаемое имя этой папки — "удаления".  <br/> |
|рековераблеитемсверсионс  <br/> |Exchange 2010  <br/> |Где хранятся более ранние версии элемента. Старые версии элемента создаются при обновлении элемента. Версии элементов черновиков не сохраняются в этой папке. Отображаемым именем этой папки является "Versions".  <br/> |
|рековераблеитемспуржес  <br/> |Exchange 2010  <br/> |Место хранения элементов, удаленных из папки "удаления". Все окончательно удаленные элементы хранилища перемещаются в эту папку. Отображаемое имя папки "очищается".  <br/> |
|арчиведделетедтитемс  <br/> |Exchange 2010  <br/> |Папка "Удаленные" по умолчанию для архивного почтового ящика.  <br/> |
|арчиверековераблеситемсрут  <br/> |Exchange 2010  <br/> |Корневая папка корзины для архивного почтового ящика. Архивированные элементы, удаленные с возможностью восстановления, перемещаются в подпапку, находящийся в этой папке.  <br/> |
|арчиверековераблеитемсделетионс  <br/> |Exchange 2010  <br/> |Основная папка корзины для архивного почтового ящика. Архивированные элементы, перемещенные в корзину, размещаются здесь.  <br/> |
|арчиверековераблеитемсверсионс  <br/> |Exchange 2010  <br/> |Где хранятся более ранние версии архивных элементов.  <br/> |
|арчиверековераблеитемспуржес  <br/> |Exchange 2010  <br/> |Место хранения необратимо удаленных элементов из папки "архивы" в корзине. Все архивные элементы, архивы которых были удалены в хранилище, перемещаются в эту папку.  <br/> |
   
## <a name="how-do-i-delete-items"></a>Как удалить элементы?
<a name="bk_howdoIdeleteitems"> </a>

Используйте один из следующих вариантов, чтобы указать, следует ли переместить элемент в папку "Удаленные" или выполнить обратимое удаление или жесткое удаление.
  
- Простой тип **диспосалтипе** , если вы используете EWS для доступа к Exchange. 
    
- [Перечисление делетемоде](http://msdn.microsoft.com/en-us/library/exchange/microsoft.exchange.webservices.data.deletemode%28v=exchg.80%29.aspx), если используется управляемый API EWS.
    
Чтобы удалить элементы и папки из почтового ящика, можно использовать несколько различных операций EWS или методов управляемого API EWS.
  
**Таблица 3: операции служб EWS и методы управляемого API EWS для удаления элементов**

|**Операция служб EWS**|**Метод управляемого API EWS**|**Версия, где параметр был представлен**|**Действие**|
|:-----|:-----|:-----|:-----|
|[Операция DeleteFolder](http://msdn.microsoft.com/library/b0f92682-4895-4bcf-a4a1-e4c2e8403979%28Office.15%29.aspx) <br/> |[Метод Folder. Delete](http://msdn.microsoft.com/en-us/library/exchange/microsoft.exchange.webservices.data.folder.delete%28v=exchg.80%29.aspx) <br/> |Exchange 2007  <br/> |Удаляет папки из почтового ящика. С помощью EWS можно пакетно удалить папки. С помощью управляемого API EWS можно удалить только одну папку для каждого вызова.  <br/> |
|[Операция DeleteItem](http://msdn.microsoft.com/library/3e26c416-fa12-476e-bfd2-5c1f4bb7b348%28Office.15%29.aspx) <br/> |[Метод Item. Delete](http://msdn.microsoft.com/en-us/library/exchange/microsoft.exchange.webservices.data.item.delete%28v=exchg.80%29.aspx)<br/><br/>[Метод ExchangeService. Делетеитемс](http://msdn.microsoft.com/en-us/library/exchange/microsoft.exchange.webservices.data.exchangeservice.deleteitems%28v=exchg.80%29.aspx) <br/> |Exchange 2007  <br/> |Удаляет элементы из почтового ящика.  <br/> |
|[Операция EmptyFolder](http://msdn.microsoft.com/library/98161486-e2f2-480f-8d5d-708ba81b208a%28Office.15%29.aspx) <br/> |[Метод Folder. Empty](http://msdn.microsoft.com/en-us/library/exchange/microsoft.exchange.webservices.data.folder.empty%28v=exchg.80%29.aspx) <br/> |Exchange 2010  <br/> |Удаляет все элементы в папке, а при необходимости удаляет все вложенные папки в папке.  <br/> |
|[Операция ApplyConversationAction](http://msdn.microsoft.com/library/73d7943d-d361-4f8b-9948-d85f886efa1a%28Office.15%29.aspx) <br/> |[Метод CONVERSATION. Енаблеалвайсделетеитемс](http://msdn.microsoft.com/en-us/library/exchange/microsoft.exchange.webservices.data.conversation.enablealwaysdeleteitems%28v=exchg.80%29.aspx)<br/><br/>[Метод CONVERSATION. Делетеитемс](http://msdn.microsoft.com/en-us/library/exchange/microsoft.exchange.webservices.data.conversation.deleteitems%28v=exchg.80%29.aspx) <br/> |Exchange 2010  <br/> |Задает действие по удалению для обработки сообщений электронной почты в беседе, чтобы они были удалены.  <br/> |
|[Операция DeleteUserConfiguration](http://msdn.microsoft.com/library/93e44690-be2d-4fdb-96a8-4ded3c193aed%28Office.15%29.aspx) <br/> |[Метод Усерконфигуратион. Delete](http://msdn.microsoft.com/en-us/library/exchange/microsoft.exchange.webservices.data.userconfiguration.delete%28v=exchg.80%29.aspx) <br/> |Exchange 2010  <br/> |Удаляет элемент, связанный с папкой, и перемещает его в корзину.  <br/> |
|[Операция CreateItem](http://msdn.microsoft.com/library/78a52120-f1d0-4ed7-8748-436e554f75b6%28Office.15%29.aspx) <br/> |[Метод встречи. Accept](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.appointment.accept%28v=exchg.80%29.aspx) <br/><br/>[Метод встреча. Акцепттентативели](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.appointment.accepttentatively%28v=exchg.80%29.aspx)<br/><br/>[Метод встреча. Канцелмитинг](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.appointment.cancelmeeting%28v=exchg.80%29.aspx)<br/><br/>[Встреча. отклонить](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.appointment.decline%28v=exchg.80%29.aspx)<br/><br/>[Метод свойство meetingrequest. Accept](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.meetingrequest.accept%28v=exchg.80%29.aspx)<br/><br/>[Метод свойство meetingrequest. Акцепттентативели](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.meetingrequest.accepttentatively%28v=exchg.80%29.aspx)<br/><br/>[Метод свойство meetingrequest. отклонить](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.meetingrequest.decline%28v=exchg.80%29.aspx) <br/> |Exchange 2007  <br/> |Косвенно перемещает элемент в папку "Удаленные" при отправке ответа на приглашение на собрание или при задании ответа на встречу.<br/><br/>Для этой операции не задан тип удаления. Сообщения о собраниях перемещаются в папку "Удаленные", когда служба успешно обрабатывает объект ответа.  <br/> |
   
Вы также можете перемещать элементы в папку "Удаленные" с помощью правил папки "Входящие". Например, вы можете [создать правила](inbox-management-and-ews-in-exchange.md) с действием Delete (удалить). 
  
Некоторые моменты, которые следует учитывать при удалении элементов:
  
- Удаление повторяющегося элемента не вызывает перемещение в папку "Удаленные" или в корзину. Это приводит к обновлению повторяющегося элемента шаблона повторяющейся серии.
    
- Вы не можете удалять папки по умолчанию из почтового ящика.
    
- Избегайте удаления собраний и сообщений о собраниях, таких как приглашения на собрания и обновления собраний. Вместо этого ответьте на эти элементы с помощью объектов ответа. Таким образом, связанные элементы календаря обновляются в соответствии с действиями респондента или организатора.
    
- Ключ изменения элемента не обновляется при перемещении элемента в папку "Удаленные" или "удаления".
    
- Если выполняется окончательное удаление элемента, а затем вызывается [Операция SyncFolderHierarchy](http://msdn.microsoft.com/library/b31916b1-bc6c-4451-a475-b7c5417f752d%28Office.15%29.aspx) или метод [SyncFolderHierarchy](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.exchangeservice.syncfolderhierarchy%28v=exchg.80%29.aspx) , управляемый API, или метод [SyncFolderItems](http://msdn.microsoft.com/library/7f0de089-8876-47ec-a871-df118ceae75d%28Office.15%29.aspx) или метод [SyncFolderItems](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.exchangeservice.syncfolderitems%28v=exchg.80%29.aspx) , возвращается запись об **удалении** изменений. Если переместить элемент в папку "Удаленные", возвращается запись изменения **обновления** . Это связано с тем, что элемент или папка будут иметь новое значение свойства [ParentFolderId](http://msdn.microsoft.com/library/258f4b1f-367e-4c7d-9c29-eb775a2398c7%28Office.15%29.aspx) . [Узнайте больше о синхронизации](mailbox-synchronization-and-ews-in-exchange.md) , если синхронизация удаленных элементов является частью вашего сценария. 
    
## <a name="find-out-more-about-deleting-items"></a>Узнайте больше об удалении элементов
<a name="findoutmore"> </a>

- [Получение уведомлений о событиях почтовых ящиков, связанных с удалением EWS, в Exchange](pull-notifications-for-ews-deletion-related-mailbox-events-in-exchange.md)
    
- [Обработка ошибок, связанных с удалением, в EWS в Exchange](handling-deletion-related-errors-in-ews-in-exchange.md)
    
## <a name="see-also"></a>См. также

- [Папки и элементы в веб-службах Exchange](folders-and-items-in-ews-in-exchange.md)    
- [Разработка клиентов веб-служб для Exchange](develop-web-service-clients-for-exchange.md)    
- [Папка "элементы с возможностью восстановления"](http://technet.microsoft.com/en-us/library/ee364755.aspx)    
- [Восстановление отдельных элементов в Exchange Server 2010](http://blogs.technet.com/b/exchange/archive/2009/09/25/3408389.aspx#_Single_Item_Recovery)    
- [Exchange 2013: удаление повторяющихся рядов программным способом из серверов Exchange Server](http://code.msdn.microsoft.com/exchange/Exchange-2013-Delete-a-e1c7b89d)    
- [Exchange 2013: Программное удаление задач из учетной записи на серверах Exchange Server](http://code.msdn.microsoft.com/exchange/Exchange-2013-Delete-tasks-13824637)    
- [Exchange 2013: пустые папки на серверах Exchange Server программным способом](http://code.msdn.microsoft.com/exchange/Exchange-2013-Empty-6487df37)    
- [Exchange 2013: Программное удаление папок из серверов Exchange Server](http://code.msdn.microsoft.com/exchange/Exchange-2013-Delete-aa1a5823)    
- [Exchange 2013: Программное удаление многих элементов из серверов Exchange Server](http://code.msdn.microsoft.com/exchange/Exchange-2013-Delete-many-064f8760)    
- [Exchange 2013: Программное удаление контактов из серверов Exchange Server](http://code.msdn.microsoft.com/exchange/Exchange-2013-Delete-3b8b0640)    
- [Удаление встреч и отмена собраний с помощью EWS в Exchange](how-to-delete-appointments-and-cancel-meetings-by-using-ews-in-exchange.md)    
- [Управление параметрами сохраняемого приложения с помощью EWS в Exchange](how-to-manage-persistent-application-settings-by-using-ews-in-exchange.md)
    

