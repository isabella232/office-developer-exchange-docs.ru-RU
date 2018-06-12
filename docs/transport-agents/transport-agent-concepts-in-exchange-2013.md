---
title: Транспорта концепции агентов в Exchange 2013
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: overview
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: 0c700af8-2792-4d3f-8571-8860e0550d8e
description: Найдите сведения о влиянии архитектуры роли конвейера и сервер агента транспорта в Exchange 2013 на разработка агента транспорта и соответствующие им классы, которые можно использовать при разработке агенты транспорта.
ms.openlocfilehash: 9ddee0d68c9104357f84322b2cce7c5f2576d871
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/11/2018
ms.locfileid: "19761321"
---
# <a name="transport-agent-concepts-in-exchange-2013"></a>Транспорта концепции агентов в Exchange 2013

Найдите сведения о влиянии архитектуры роли конвейера и сервер агента транспорта в Exchange 2013 на разработка агента транспорта и соответствующие им классы, которые можно использовать при разработке агенты транспорта. 
  
**Применимо к:** Exchange Server 2013 
  
Библиотека классов, представленные в Exchange Server 2013 можно использовать для реализации агенты транспорта, регистрации событий и выполните действия на сообщения, проходящие через транспортный конвейер. Агенты транспорта можно также использовать для изменения сообщений и преобразование содержимого. 
  
В этой статье представлены сведения о агенты транспорта и архитектура транспортный конвейер. Важно понимать архитектуру транспортный конвейер, чтобы его можно изменить поведение транспорта в соответствии с требованиями вашей организации. В этой статье также предоставляет сведения об изменениях в архитектуре Exchange 2013, влияющие на агенты транспорта и соответствующие им классы, которые можно использовать при разработке агенты транспорта. 
  
## <a name="transport-agents-in-the-transport-pipeline"></a>Агенты транспорта в транспортный конвейер
<a name="Pipeline"> </a>

Агенты транспорта являются производными от одного из следующих трех классов:
  
- [SmtpReceiveAgent](https://msdn.microsoft.com/library/Microsoft.Exchange.Data.Transport.Smtp.SmtpReceiveAgent.aspx)
- [RoutingAgent](https://msdn.microsoft.com/library/Microsoft.Exchange.Data.Transport.Routing.RoutingAgent.aspx)
- [DeliveryAgent](https://msdn.microsoft.com/library/Microsoft.Exchange.Data.Transport.Delivery.DeliveryAgent.aspx)
    
Транспортный конвейер относится к потоку данных сообщений в пределах организации Exchange 2013. Конвейер состоит из служб, перечисленных в следующей таблице.
  
**В таблице 1. Транспортный конвейер служб**

|**Служба**|**Описание**|**Поддерживаемые классы**|
|:-----|:-----|:-----|
|Транспорта переднего плана  <br/> |Запускается на всех [серверах клиентского доступа](http://technet.microsoft.com/en-us/library/dd298114%28v=exchg.150%29.aspx) и действует как прокси-сервер без сведений о состоянии для всех входящих и исходящих внешний SMTP-трафика для организации Exchange 2013. Служба транспорта переднего плана не проверки содержимого сообщения или его в очередь любые сообщения на локальном компьютере. Он взаимодействует со службой транспорта на [сервере почтовых ящиков](http://technet.microsoft.com/en-us/library/jj150491%28v=exchg.150%29.aspx).  <br/> |[SmtpReceiveAgent](https://msdn.microsoft.com/library/Microsoft.Exchange.Data.Transport.Smtp.SmtpReceiveAgent.aspx) <br/> |
|Транспорта  <br/> |Выполняется на всех серверах почтовых ящиков и похож на роль [транспортного сервера-концентратора](http://technet.microsoft.com/en-us/library/bb123494%28v=exchg.141%29.aspx) в Exchange Server 2010. Транспортная служба Маршрутизация сообщений между собой и службы транспорта почтовых ящиков и транспортного сервера переднего плана. Эта служба не напрямую связываются с базы данных почтовых ящиков.  <br/> |[SmtpReceiveAgent](https://msdn.microsoft.com/library/Microsoft.Exchange.Data.Transport.Smtp.SmtpReceiveAgent.aspx) <br/> [RoutingAgent](https://msdn.microsoft.com/library/Microsoft.Exchange.Data.Transport.Routing.RoutingAgent.aspx) <br/> [DeliveryAgent](https://msdn.microsoft.com/library/Microsoft.Exchange.Data.Transport.Delivery.DeliveryAgent.aspx) <br/> |
|Транспорта почтовых ящиков  <br/> |Запускается на всех серверах почтовых ящиков и состоит из двух отдельных служб: отправки почтовых ящиков и транспортного доставки почтового ящика. Доставка транспорта почтовых ящиков принимает SMTP-сообщения из транспортной службы и подключается к базе данных почтовых ящиков с помощью Exchange удаленный вызов процедур (RPC) для доставки сообщения. Отправки почтовых ящиков подключается к базе данных почтовых ящиков, используя протокол RPC для получения сообщений и отправляет сообщения по протоколу SMTP для транспортной службы.  <br/> |Нет.  <br/> |
   
### <a name="transport-events"></a>События транспорта
<a name="Events"> </a>

Реализовать агенты транспорта, сначала Регистрация события, а затем — действие при включении этого события. Каждый из типов три агента можно зарегистрировать для другой набор событий.
  
На следующем рисунке показана where в транспортный конвейер транспорта, агенты можно регистрировать события.
  
**На рисунке 1. События транспорта**

![Изображение, показывающее поток сообщений через конвейер транспорта и события, для которых может зарегистрироваться каждый агент, начиная с событий SMTP для агента SmtpReceivedAgent, событий категоризатора для агента RoutingAgent и заканчивая событиями доставки для агента DeliveryAgent.](media/TAConceptsFig1.png)
  
При поступлении сообщения транспортный конвейер, производные от класса [SmtpReceiveAgent](https://msdn.microsoft.com/library/Microsoft.Exchange.Data.Transport.Smtp.SmtpReceiveAgent.aspx) агента транспорта может выступать в окне сообщения во время события SMTP, агентов, зарегистрированных для. Агент, производные от класса [RoutingAgent](https://msdn.microsoft.com/library/Microsoft.Exchange.Data.Transport.Routing.RoutingAgent.aspx) может выступать на любой из четырех классификатор событий, которые он был зарегистрирован для. Агент, производные от класса [DeliveryAgent](https://msdn.microsoft.com/library/Microsoft.Exchange.Data.Transport.Delivery.DeliveryAgent.aspx) может выступать на сообщение во время доставки событий, которые он был зарегистрирован для. 
  
## <a name="transport-agents-and-server-roles"></a>Агенты транспорта и роли сервера
<a name="ServerRoles"> </a>

Изменения архитектуры роли сервера в Exchange 2013 влияют на агенты транспорта и что можно сделать агентов транспорта. Exchange 2013 включает в себя следующие роли сервера:
  
- Сервер почтовых ящиков — протоколы включает в себя клиентского доступа, служба транспорта, базы данных почтовых ящиков и компоненты единой системы обмена сообщениями. Сервер почтовых ящиков взаимодействует непосредственно с помощью доменных служб Active Directory (AD DS), серверов клиентского доступа и почтовых клиентов, например Outlook.
    
- Сервер клиентского доступа — предоставляет проверки подлинности, только в режиме одобрения администратором, службы прокси-сервера и клиентского доступа протоколов, таких как HTTP, POP, IMAP и SMTP.
    
- Пограничный транспортный сервер — маршрутов электронной почты, в и вне организации. Пограничные транспортные серверы обычно находятся в пограничной топологии Exchange.
    
Эта структура консолидированной сокращает число серверов, необходимо развернуть в среде Exchange 2013. Администраторы больше не нужно развертывать серверы клиентского доступа и транспортного сервера-концентратора в каждом сайте Active Directory, которая включает в себя на сервере почтовых ящиков, и они больше не требуется для обновления всех ролей сервера, чтобы воспользоваться преимуществами новых возможностей.
  
Эти изменения в архитектуре роли сервера может повлиять на которых в конвейере агента может реагировать на события. При создании агенты транспорта для версии Exchange, предшествующие Exchange 2013, обязательно просмотрите архитектурные изменения, определите, нужно ли изменять агентов.
  
На следующем рисунке показана взаимосвязь архитектурные изменения в Exchange 2013 результатов в оптимальное и консолидированная транспортный конвейер. На этом рисунке серверов клиентского доступа, помечаются как сервер клиентского доступа. И серверы почтовых ящиков, помечаются как MBX.
  
**На рисунке 2. Архитектура роли сервера Exchange 2013**

![Изображение, показывающее, как трафик клиента через внешний брандмауэр и пограничный транспортный сервер (слева) проходит через балансировщик нагрузки четвертого слоя в консолидированный массив CAS и набор серверов почтовых ящиков в группе доступа к базе данных (справа).](media/Transport_Agent_Concepts_Fig_3.png)
  
На следующем рисунке показана взаимодействие между ролями серверов Exchange 2013.
  
**На рисунке 3. Взаимодействие сервера почтовых ящиков и клиентского доступа**

![Изображение, показывающее взаимодействие, начиная со стрелок от трафика клиента, проходящих через балансировщик нагрузки четвертого слоя, для которого на сервере клиентского доступа имеется 4 цели: IIS/HTTP-прокси, POP/IMAP, SMTP и UM. Стрелки указывают на соответствующие цели в хранилище почтовых ящиков.](media/Transport_Agent_Concepts_Fig_4.png)
  
Дополнительные сведения об изменениях в архитектуре роли сервера Exchange 2013 можно [архитектура Exchange 2013](http://technet.microsoft.com/en-us/library/jj150540%28v=exchg.150%29.aspx#BKMK_Arch) в [новые возможности в Exchange 2013](http://technet.microsoft.com/en-us/library/jj150540%28v=exchg.150%29.aspx). 
  
## <a name="transport-agent-classes"></a>Классы агента транспорта
<a name="Create"> </a>

Класс, который наследует агента транспорта определяет события, для которых можно регистрировать агентом. Агента обычно будет содержать класс агентов, фабрика агентов, один или несколько обработчиков событий и код, который выполняет действия, которые будут агента вступило в.
  
В следующей таблице перечислены классы, из которых формируется для каждого типа агента.
  
**В таблице 2. Классы агента**

||||
|:-----|:-----|:-----|
|Тип агента  <br/> |Базовый класс фабрики  <br/> |Базовый класс агентов  <br/> |
|Получения SMTP  <br/> |[SmtpReceiveAgentFactory](https://msdn.microsoft.com/library/Microsoft.Exchange.Data.Transport.Smtp.SmtpReceiveAgentFactory.aspx) <br/> |[SmtpReceiveAgent](https://msdn.microsoft.com/library/Microsoft.Exchange.Data.Transport.Smtp.SmtpReceiveAgent.aspx) <br/> |
|Маршрутизация  <br/> |[RoutingAgentFactory](https://msdn.microsoft.com/library/Microsoft.Exchange.Data.Transport.Routing.RoutingAgentFactory.aspx) <br/> |[RoutingAgent](https://msdn.microsoft.com/library/Microsoft.Exchange.Data.Transport.Routing.RoutingAgent.aspx) <br/> |
|Доставки  <br/> |[DeliveryAgentFactory\<Manager\>](https://msdn.microsoft.com/library/Microsoft.Exchange.Data.Transport.Delivery.DeliveryAgentFactory`1.aspx) <br/> |[DeliveryAgent](https://msdn.microsoft.com/library/Microsoft.Exchange.Data.Transport.Delivery.DeliveryAgent.aspx) <br/> |
   
Эти фабрики и агент базовые классы предоставляют свойства и методы, которые можно использовать для доступа к транспорта события и сообщения. Реализация классов в агента, производные от этих классов. В классе фабрики производные агента переопределение метода **CreateAgent** , чтобы он возвращает новый экземпляр класса агента. 
  
Аргументы, передаваемые в события может содержать экземпляр класса [EmailMessage](https://msdn.microsoft.com/library/Microsoft.Exchange.Data.Transport.Email.EmailMessage.aspx) , который можно использовать для изменения свойства и содержимое базового сообщения. Не все сообщения в каждом событии. Необходимо определить, какие агента и какие события лучше всего подходит для задач, которые необходимо выполнить. 
  
Следующие пространства имен содержат типы, которые можно использовать для чтения, записи и изменения сообщений в транспортный конвейер:
  
- [Microsoft.Exchange.Data.Mime.Encoders](https://msdn.microsoft.com/library/Microsoft.Exchange.Data.Mime.Encoders.aspx)
    
- [Microsoft.Exchange.Data.ContentTypes.iCalendar](https://msdn.microsoft.com/library/Microsoft.Exchange.Data.ContentTypes.iCalendar.aspx)
    
- [Microsoft.Exchange.Data.Mime](https://msdn.microsoft.com/library/Microsoft.Exchange.Data.Mime.aspx)
    
- [Microsoft.Exchange.Data.ContentTypes.Tnef](https://msdn.microsoft.com/library/Microsoft.Exchange.Data.ContentTypes.Tnef.aspx)
    
- [Microsoft.Exchange.Data.ContentTypes.vCard](https://msdn.microsoft.com/library/Microsoft.Exchange.Data.ContentTypes.vCard.aspx)
    
После того, как записать агента транспорта, вы [Установка и управление ими агента](http://technet.microsoft.com/en-us/library/bb125175%28v=exchg.150%29.aspx) с помощью командной консоли Exchange. Дополнительные сведения содержатся в разделе [Создание агенты транспорта для Exchange 2013](creating-transport-agents-for-exchange-2013.md). 
  
## <a name="see-also"></a>См. также

- [Агенты транспорта в Exchange](transport-agents-in-exchange-2013.md)    
- [Справочник по агента транспорта для Exchange 2013](transport-agent-reference-for-exchange-2013.md)   
- [Чтение и изменение сообщений в транспортный конвейер Exchange 2013](reading-and-modifying-messages-in-the-exchange-2013-transport-pipeline.md)    
- [Новые возможности Exchange 2013](http://technet.microsoft.com/en-us/library/jj150540%28v=exchg.150%29.aspx)   
- [Архитектура роли сервера Exchange 2013](http://blogs.technet.com/b/exchange/archive/2013/01/23/exchange-2013-server-role-architecture.aspx)    
- [Почтовый ящик и серверов клиентского доступа](http://technet.microsoft.com/en-us/library/jj150519%28v=exchg.150%29.aspx)   
- [Поток почты Exchange Server 2013](http://technet.microsoft.com/en-us/library/aa996349.aspx)
- [Маршрутизация почты 2013 сервера Exchange](http://technet.microsoft.com/en-us/library/aa998825%28v=exchg.150%29.aspx)   
- [Exchange Server PowerShell (Командная консоль Exchange)](https://docs.microsoft.com/en-us/powershell/exchange/exchange-server/exchange-management-shell?view=exchange-ps)
    

