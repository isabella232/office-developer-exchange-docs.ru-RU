---
title: Концепции транспортного агента в Exchange 2013 г.
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: overview
ms.prod: office-online-server
ms.localizationpriority: medium
ms.assetid: 0c700af8-2792-4d3f-8571-8860e0550d8e
description: Сведения о том, как архитектура роли конвейера транспортных агентов и серверов в 2013 Exchange 2013 г. влияет на разработку транспортного агента, а также классы, которые можно использовать для разработки транспортных агентов.
ms.openlocfilehash: 9116c9b7811958a2479421a642052df3cee24e34
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/24/2021
ms.locfileid: "59537163"
---
# <a name="transport-agent-concepts-in-exchange-2013"></a>Концепции транспортного агента в Exchange 2013 г.

Сведения о том, как архитектура роли конвейера транспортных агентов и серверов в 2013 Exchange 2013 г. влияет на разработку транспортного агента, а также классы, которые можно использовать для разработки транспортных агентов. 
  
**Применяется к:** Exchange Server 2013 г. 
  
Вы можете использовать библиотеку классов, предоставленную в Exchange Server 2013 г., для реализации транспортных агентов, которые регистрируются для событий и принимают меры к сообщениям по мере их прохода по транспортному конвейеру. Вы также можете использовать транспортные агенты для изменения сообщений и преобразования контента. 
  
В этой статье данная статья содержит сведения о транспортных агентах и архитектуре транспортного конвейера. Важно понимать архитектуру транспортного конвейера, чтобы можно было изменить поведение транспорта для удовлетворения потребностей организации. В этой статье также приводится информация об изменениях в архитектуре Exchange 2013 г., влияющих на транспортные агенты, и классах, которые можно использовать для разработки транспортных агентов. 
  
## <a name="transport-agents-in-the-transport-pipeline"></a>Транспортные агенты в транспортном конвейере
<a name="Pipeline"> </a>

Транспортные агенты являются производными от одного из следующих трех классов:
  
- [SmtpReceiveAgent](https://msdn.microsoft.com/library/Microsoft.Exchange.Data.Transport.Smtp.SmtpReceiveAgent.aspx)
- [RoutingAgent](https://msdn.microsoft.com/library/Microsoft.Exchange.Data.Transport.Routing.RoutingAgent.aspx)
- [DeliveryAgent](https://msdn.microsoft.com/library/Microsoft.Exchange.Data.Transport.Delivery.DeliveryAgent.aspx)
    
Конвейер транспорта относится к потоку данных сообщений в пределах организации Exchange 2013 г. Конвейер состоит из служб, перечисленных в следующей таблице.
  
**Таблица 1. Службы конвейера транспорта**

|**Служба**|**Описание**|**Поддерживаемые классы**|
|:-----|:-----|:-----|
|Передний конечный транспорт  <br/> |Выполняется [на](https://technet.microsoft.com/library/dd298114%28v=exchg.150%29.aspx) всех серверах клиентского доступа и выполняется в качестве прокси-сервера без состояния для всех входящий и исходящие внешние трафики SMTP для Exchange организации 2013 г. Служба транспорта переднего конца не проверяет содержимое сообщений и не выстроит очереди на локальном уровне. Он взаимодействует со службой транспорта на [сервере почтовых ящиков.](https://technet.microsoft.com/library/jj150491%28v=exchg.150%29.aspx)  <br/> |[SmtpReceiveAgent](https://msdn.microsoft.com/library/Microsoft.Exchange.Data.Transport.Smtp.SmtpReceiveAgent.aspx) <br/> |
|Transport  <br/> |Выполняется на всех серверах почтовых [](https://technet.microsoft.com/library/bb123494%28v=exchg.141%29.aspx) ящиков и аналогична роли транспортного сервера hub в Exchange Server 2010 г. Служба транспорта передает сообщения между собой и службами транспорта почтовых ящиков и переднего транспорта. Эта служба не взаимодействует напрямую с базами данных почтовых ящиков.  <br/> |[SmtpReceiveAgent](https://msdn.microsoft.com/library/Microsoft.Exchange.Data.Transport.Smtp.SmtpReceiveAgent.aspx) <br/> [RoutingAgent](https://msdn.microsoft.com/library/Microsoft.Exchange.Data.Transport.Routing.RoutingAgent.aspx) <br/> [DeliveryAgent](https://msdn.microsoft.com/library/Microsoft.Exchange.Data.Transport.Delivery.DeliveryAgent.aspx) <br/> |
|Транспортная служба почтовых ящиков.  <br/> |Выполняется на всех серверах почтовых ящиков и состоит из двух отдельных служб: отправки транспорта почтовых ящиков и доставки транспорта почтовых ящиков. Транспортная доставка почтовых ящиков получает сообщения SMTP из транспортной службы и подключается к базе данных почтовых ящиков с помощью Exchange удаленного вызова процедуры (RPC) для доставки сообщения. Отправка транспорта почтовых ящиков подключается к базе данных почтовых ящиков с помощью RPC для получения сообщений и передает сообщения через SMTP в службу транспорта.  <br/> |Нет.  <br/> |
   
### <a name="transport-events"></a>События транспорта
<a name="Events"> </a>

Реализуются транспортные агенты, которые сначала регистрируются для события, а затем выполняют действие, когда это событие загореется. Каждый из трех типов агентов может зарегистрироваться для другого набора событий.
  
На следующем рисунке показано, где в транспортном конвейере транспортные агенты могут регистрироваться для событий.
  
**Рис. 1. События транспорта**

![Изображение, показывающее поток сообщений через конвейер транспорта и события, для которых может зарегистрироваться каждый агент, начиная с событий SMTP для агента SmtpReceivedAgent, событий категоризатора для агента RoutingAgent и заканчивая событиями доставки для агента DeliveryAgent.](media/TAConceptsFig1.png)
  
Когда сообщение входит в конвейер транспорта, транспортный агент, полученный из класса [SmtpReceiveAgent,](https://msdn.microsoft.com/library/Microsoft.Exchange.Data.Transport.Smtp.SmtpReceiveAgent.aspx) может действовать в сообщении во время любого из событий SMTP, для которые зарегистрирован агент. Агент, полученный из [класса RoutingAgent,](https://msdn.microsoft.com/library/Microsoft.Exchange.Data.Transport.Routing.RoutingAgent.aspx) может действовать в любом из четырех событий категоризатора, для которые он зарегистрировался. Агент, полученный из класса [DeliveryAgent,](https://msdn.microsoft.com/library/Microsoft.Exchange.Data.Transport.Delivery.DeliveryAgent.aspx) может действовать по сообщению во время любого из зарегистрированных событий доставки. 
  
## <a name="transport-agents-and-server-roles"></a>Транспортные агенты и роли сервера
<a name="ServerRoles"> </a>

Изменения архитектуры ролей сервера в Exchange 2013 г. влияют на транспортные агенты и то, что могут сделать ваши транспортные агенты. Exchange 2013 включает следующие роли сервера:
  
- Сервер почтовых ящиков — включает протоколы клиентского доступа, транспортную службу, базы данных почтовых ящиков и компоненты единой системы обмена сообщениями. Сервер почтовых ящиков напрямую взаимодействует с службами домена Active Directory (AD DS), серверами клиентского доступа и почтовыми клиентами, такими как Outlook.
    
- Сервер клиентского доступа — обеспечивает проверку подлинности, ограниченное перенаправление, прокси-службы и протоколы клиентского доступа, такие как HTTP, POP, IMAP и SMTP.
    
- Edge Transport server — маршруты электронной почты в организацию и из нее. Edge Transport servers typically sit at the perimeter of an Exchange topology.
    
Эта консолидированная структура сокращает число серверов, которые необходимо развернуть в среде Exchange 2013 г. Администраторам больше не нужно развертывать серверы hub Transport и Client Access на каждом сайте Active Directory, который включает сервер почтовых ящиков, и им больше не нужно обновлять все роли сервера, чтобы воспользоваться новыми функциями.
  
Эти изменения в архитектуре ролей сервера могут потенциально повлиять на то, где в конвейере агент может реагировать на события. Если вы создали транспортные агенты для версий Exchange до Exchange 2013 г., обязательно просмотрите архитектурные изменения, чтобы определить, нужно ли вносить какие-либо изменения в агенты.
  
На следующем рисунке показано, как изменения архитектуры в Exchange 2013 г. привели к упрощенному и консолидированному транспортному конвейеру. На этом рисунке серверы клиентского доступа помечены как CAS. А серверы почтовых ящиков помечены как MBX.
  
**Рис. 2. Exchange 2013 года архитектура ролей сервера**

![Изображение, показывающее, как трафик клиента через внешний брандмауэр и пограничный транспортный сервер (слева) проходит через балансировщик нагрузки четвертого слоя в консолидированный массив CAS и набор серверов почтовых ящиков в группе доступа к базе данных (справа).](media/Transport_Agent_Concepts_Fig_3.png)
  
На следующем рисунке показано взаимодействие между Exchange серверными ролями 2013 года.
  
**Рис. 3. Взаимодействие почтовых ящиков и серверов клиентского доступа**

![Изображение, показывающее взаимодействие, начиная со стрелок от трафика клиента, проходящих через балансировщик нагрузки четвертого слоя, для которого на сервере клиентского доступа имеется 4 цели: IIS/HTTP-прокси, POP/IMAP, SMTP и UM. Стрелки указывают на соответствующие цели в хранилище почтовых ящиков.](media/Transport_Agent_Concepts_Fig_4.png)
  
Дополнительные сведения об изменениях в архитектуре ролей Exchange 2013 г. см. в Exchange [2013](https://technet.microsoft.com/library/jj150540%28v=exchg.150%29.aspx#BKMK_Arch) г. в Exchange [2013](https://technet.microsoft.com/library/jj150540%28v=exchg.150%29.aspx)г. 
  
## <a name="transport-agent-classes"></a>Классы агентов транспорта
<a name="Create"> </a>

Класс, который получает транспортный агент, определяет события, для которых агент может зарегистрироваться. Обычно агент содержит класс агента, фабрику агентов, один или несколько обработчиков событий и код, который выполняет действия, которые необходимо выполнить агенту.
  
В следующей таблице перечислены классы, из которых следует извлечь для каждого типа агента.
  
**Таблица 2. Классы агентов**

||||
|:-----|:-----|:-----|
|Тип агента  <br/> |Базовый класс фабрики  <br/> |Базовый класс агента  <br/> |
|Получение SMTP  <br/> |[SmtpReceiveAgentFactory](https://msdn.microsoft.com/library/Microsoft.Exchange.Data.Transport.Smtp.SmtpReceiveAgentFactory.aspx) <br/> |[SmtpReceiveAgent](https://msdn.microsoft.com/library/Microsoft.Exchange.Data.Transport.Smtp.SmtpReceiveAgent.aspx) <br/> |
|Маршрутная маршрутика  <br/> |[RoutingAgentFactory](https://msdn.microsoft.com/library/Microsoft.Exchange.Data.Transport.Routing.RoutingAgentFactory.aspx) <br/> |[RoutingAgent](https://msdn.microsoft.com/library/Microsoft.Exchange.Data.Transport.Routing.RoutingAgent.aspx) <br/> |
|Delivery  <br/> |[DeliveryAgentFactory\<Manager\>](https://msdn.microsoft.com/library/dd877550(v=exchg.150).aspx) <br/> |[DeliveryAgent](https://msdn.microsoft.com/library/microsoft.exchange.data.transport.delivery.deliveryagent(v=exchg.150).aspx) <br/> |
   
Эти базовые классы фабрики и агента предоставляют свойства и методы, которые можно использовать для доступа к транспортным событиям и сообщениям. Реализуйте классы в агенте, унаследованные от этих классов. В производных классах фабрики агентов переопределите метод **CreateAgent,** чтобы он возвращал новый экземпляр класса агента. 
  
Аргументы, переданные событиям, могут содержать экземпляр класса [EmailMessage,](https://msdn.microsoft.com/library/Microsoft.Exchange.Data.Transport.Email.EmailMessage.aspx) который можно использовать для изменения свойств и содержимого в основном сообщении. Не все сведения о сообщениях доступны в каждом событии. Необходимо определить, какой агент и какое событие является наилучшим для задачи, которую вы хотите выполнить. 
  
В следующих пространствах имен содержатся типы, которые можно использовать для чтения, записи и изменения сообщений в транспортном конвейере:
  
- [Microsoft. Exchange. Data.Mime.Encoders](https://msdn.microsoft.com/library/Microsoft.Exchange.Data.Mime.Encoders.aspx)
    
- [Microsoft. Exchange. Data.ContentTypes.iCalendar](https://msdn.microsoft.com/library/Microsoft.Exchange.Data.ContentTypes.iCalendar.aspx)
    
- [Microsoft. Exchange. Data.Mime](https://msdn.microsoft.com/library/Microsoft.Exchange.Data.Mime.aspx)
    
- [Microsoft. Exchange. Data.ContentTypes.Tnef](https://msdn.microsoft.com/library/Microsoft.Exchange.Data.ContentTypes.Tnef.aspx)
    
- [Microsoft. Exchange. Data.ContentTypes.vCard](https://msdn.microsoft.com/library/Microsoft.Exchange.Data.ContentTypes.vCard.aspx)
    
После записи транспортного агента [установите](https://technet.microsoft.com/library/bb125175%28v=exchg.150%29.aspx) и управляйте агентом с помощью Exchange management Shell. Дополнительные сведения см. в дополнительных сведениях о создании транспортных [агентов для Exchange 2013 г.](creating-transport-agents-for-exchange-2013.md) 
  
## <a name="see-also"></a>См. также

- [Агенты транспорта в Exchange](transport-agents-in-exchange-2013.md)    
- [Ссылка агента транспорта на Exchange 2013 г.](transport-agent-reference-for-exchange-2013.md)   
- [Чтение и изменение сообщений в конвейере Exchange 2013 г.](reading-and-modifying-messages-in-the-exchange-2013-transport-pipeline.md)    
- [Что нового в Exchange 2013 г.](https://technet.microsoft.com/library/jj150540%28v=exchg.150%29.aspx)   
- [Exchange 2013 серверной архитектуры ролей](https://blogs.technet.com/b/exchange/archive/2013/01/23/exchange-2013-server-role-architecture.aspx)    
- [Серверы почтового ящика и клиентского доступа](https://technet.microsoft.com/library/jj150519%28v=exchg.150%29.aspx)   
- [Exchange Server 2013 почтовый Flow](https://technet.microsoft.com/library/aa996349.aspx)
- [Exchange Server рассылки почты 2013 г.](https://technet.microsoft.com/library/aa998825%28v=exchg.150%29.aspx)   
- [Exchange Server PowerShell (Exchange управленческой оболочки)](https://docs.microsoft.com/powershell/exchange/exchange-server/exchange-management-shell?view=exchange-ps)
    

