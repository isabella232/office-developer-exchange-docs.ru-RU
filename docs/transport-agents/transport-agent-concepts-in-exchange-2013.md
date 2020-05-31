---
title: Основные понятия, связанные с агентами транспорта в Exchange 2013
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: overview
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: 0c700af8-2792-4d3f-8571-8860e0550d8e
description: Сведения о том, как архитектура агента транспорта и роль сервера в Exchange 2013 влияет на разработку агента транспорта, а также классы, которые можно использовать для разработки агентов транспорта.
ms.openlocfilehash: 6f7a03e16b260117c6ee27b86ec0e55b5346e301
ms.sourcegitcommit: 9061fcf40c218ebe88911783f357b7df278846db
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/28/2018
ms.locfileid: "21353709"
---
# <a name="transport-agent-concepts-in-exchange-2013"></a>Основные понятия, связанные с агентами транспорта в Exchange 2013

Сведения о том, как архитектура агента транспорта и роль сервера в Exchange 2013 влияет на разработку агента транспорта, а также классы, которые можно использовать для разработки агентов транспорта. 
  
**Применимо к:** Exchange Server 2013 
  
С помощью библиотеки классов, предоставляемой в Exchange Server 2013, можно реализовать агенты транспорта, которые регистрируют события и принимают действия к сообщениям, проходящих через транспортный конвейер. Вы также можете использовать агенты транспорта для изменения сообщений и преобразования контента. 
  
В этой статье представлены сведения об агентах транспорта и об архитектуре конвейера транспорта. Важно понимать архитектуру транспортного конвейера, чтобы можно было изменить поведение транспорта в соответствии с потребностями Организации. В этой статье также приводятся сведения об изменениях в архитектуре Exchange 2013, влияющих на агенты транспорта и классы, которые можно использовать для разработки агентов транспорта. 
  
## <a name="transport-agents-in-the-transport-pipeline"></a>Агенты транспорта в транспортном конвейере
<a name="Pipeline"> </a>

Агенты транспорта являются производными от одного из следующих трех классов:
  
- [SmtpReceiveAgent](https://msdn.microsoft.com/library/Microsoft.Exchange.Data.Transport.Smtp.SmtpReceiveAgent.aspx)
- [RoutingAgent](https://msdn.microsoft.com/library/Microsoft.Exchange.Data.Transport.Routing.RoutingAgent.aspx)
- [DeliveryAgent](https://msdn.microsoft.com/library/Microsoft.Exchange.Data.Transport.Delivery.DeliveryAgent.aspx)
    
Транспортный конвейер относится к потоку данных сообщений в пределах границ организации Exchange 2013. Конвейер состоит из служб, перечисленных в следующей таблице.
  
**Таблица 1. Службы транспортного конвейера**

|**Служба**|**Описание**|**Поддерживаемые классы**|
|:-----|:-----|:-----|
|Транспортный сервер переднего плана  <br/> |Выполняется на всех [серверах клиентского доступа](http://technet.microsoft.com/en-us/library/dd298114%28v=exchg.150%29.aspx) и выступает в роли прокси-сервера без состояний для всего входящего и исходящего внешнего SMTP-трафика для организации Exchange 2013. Внешняя служба транспорта не проверяет содержимое сообщения и не ставит в очередь локальное сообщение. Он связывается со службой транспорта на [сервере почтовых ящиков](http://technet.microsoft.com/en-us/library/jj150491%28v=exchg.150%29.aspx).  <br/> |[SmtpReceiveAgent](https://msdn.microsoft.com/library/Microsoft.Exchange.Data.Transport.Smtp.SmtpReceiveAgent.aspx) <br/> |
|Transport  <br/> |Выполняется на всех серверах почтовых ящиков и аналогично роли [транспортного сервера-концентратора](http://technet.microsoft.com/en-us/library/bb123494%28v=exchg.141%29.aspx) в Exchange Server 2010. Служба транспорта маршрутизирует сообщения между собой, а также транспортным сервером и интерфейсным транспортным службам. Эта служба не взаимодействует напрямую с базами данных почтовых ящиков.  <br/> |[SmtpReceiveAgent](https://msdn.microsoft.com/library/Microsoft.Exchange.Data.Transport.Smtp.SmtpReceiveAgent.aspx) <br/> [RoutingAgent](https://msdn.microsoft.com/library/Microsoft.Exchange.Data.Transport.Routing.RoutingAgent.aspx) <br/> [DeliveryAgent](https://msdn.microsoft.com/library/Microsoft.Exchange.Data.Transport.Delivery.DeliveryAgent.aspx) <br/> |
|Транспортная служба почтовых ящиков.  <br/> |Выполняется на всех серверах почтовых ящиков и состоит из двух отдельных служб: отправка транспорта почтового ящика и доставка транспорта почтовых ящиков. Доставка транспорта почтовых ящиков получает сообщения SMTP от службы транспорта и подключается к базе данных почтовых ящиков с помощью удаленного вызова процедур (RPC) Exchange для доставки сообщения. Отправка транспорта почтовых ящиков подключается к базе данных почтовых ящиков с помощью RPC для получения сообщений и отправки сообщений по протоколу SMTP в службу транспорта.  <br/> |Нет.  <br/> |
   
### <a name="transport-events"></a>Транспортные события
<a name="Events"> </a>

Вы реализуете агенты транспорта, сначала регистрируя их для события, а затем выполнив действие при срабатывании этого события. Каждый из трех типов агентов может регистрироваться для разных наборов событий.
  
На следующем рисунке показано, где в агенте транспорта транспортного конвейера могут регистрироваться события.
  
**Рис. 1. Транспортные события**

![Изображение, показывающее поток сообщений через конвейер транспорта и события, для которых может зарегистрироваться каждый агент, начиная с событий SMTP для агента SmtpReceivedAgent, событий категоризатора для агента RoutingAgent и заканчивая событиями доставки для агента DeliveryAgent.](media/TAConceptsFig1.png)
  
Когда сообщение поступает в транспортный конвейер, агент транспорта, производный от класса [SmtpReceiveAgent](https://msdn.microsoft.com/library/Microsoft.Exchange.Data.Transport.Smtp.SmtpReceiveAgent.aspx) , может работать с сообщением во время любого события SMTP, зарегистрированного агентом. Агент, производный от класса [RoutingAgent](https://msdn.microsoft.com/library/Microsoft.Exchange.Data.Transport.Routing.RoutingAgent.aspx) , может работать с любым из четырех событий классификатора, для которых он зарегистрирован. Агент, производный от класса [DeliveryAgent](https://msdn.microsoft.com/library/Microsoft.Exchange.Data.Transport.Delivery.DeliveryAgent.aspx) , может работать с сообщением во время любого события доставки, для которого он зарегистрирован. 
  
## <a name="transport-agents-and-server-roles"></a>Агенты транспорта и роли сервера
<a name="ServerRoles"> </a>

Изменения архитектуры ролей сервера в Exchange 2013 влияют на агенты транспорта и действия, которые могут выполнять агенты транспорта. Exchange 2013 включает следующие роли сервера:
  
- Сервер почтовых ящиков — включает протоколы клиентского доступа, службу транспорта, базы данных почтовых ящиков и компоненты единой системы обмена сообщениями. Сервер почтовых ящиков взаимодействуют непосредственно с доменными службами Active Directory (AD DS), серверами клиентского доступа и почтовыми клиентами, такими как Outlook.
    
- Сервер клиентского доступа — обеспечивает проверку подлинности, ограниченное перенаправление, прокси-службы и протоколы клиентского доступа, такие как HTTP, POP, IMAP и SMTP.
    
- Пограничный транспортный сервер — направляет электронную почту в организацию и из нее. Пограничные транспортные серверы обычно располагаются на периметре топологии Exchange.
    
Эта консолидированная структура сокращает количество серверов, которые необходимо развернуть в среде Exchange 2013. Администраторам больше не нужно развертывать серверы транспортных серверов-концентраторов и клиентского доступа на каждом сайте Active Directory, включающем сервер почтовых ящиков, и больше не нужно обновлять все роли сервера, чтобы воспользоваться преимуществами новых функций.
  
Эти изменения в архитектуре ролей сервера потенциально могут повлиять на то, где в конвейере может реагировать ваш агент на события. Если вы создали агенты транспорта для более ранних версий Exchange, чем Exchange 2013, ознакомьтесь с изменениями архитектуры, чтобы определить, нужно ли вносить изменения в агенты.
  
На следующем рисунке показано, как изменения архитектуры в Exchange 2013 приводят к упрощенному консолидированному транспортному конвейеру. На этом рисунке серверы клиентского доступа помечены как ЦС. Серверы почтовых ящиков помечаются метками MBX.
  
**Рис. 2. Архитектура ролей сервера Exchange 2013**

![Изображение, показывающее, как трафик клиента через внешний брандмауэр и пограничный транспортный сервер (слева) проходит через балансировщик нагрузки четвертого слоя в консолидированный массив CAS и набор серверов почтовых ящиков в группе доступа к базе данных (справа).](media/Transport_Agent_Concepts_Fig_3.png)
  
На следующем рисунке показаны взаимодействия между ролями сервера Exchange 2013.
  
**Рис. 3. Взаимодействия сервера почтовых ящиков и клиентского доступа**

![Изображение, показывающее взаимодействие, начиная со стрелок от трафика клиента, проходящих через балансировщик нагрузки четвертого слоя, для которого на сервере клиентского доступа имеется 4 цели: IIS/HTTP-прокси, POP/IMAP, SMTP и UM. Стрелки указывают на соответствующие цели в хранилище почтовых ящиков.](media/Transport_Agent_Concepts_Fig_4.png)
  
Более подробную информацию об изменениях в архитектуре ролей сервера Exchange 2013 можно узнать в статье Exchange [2013 Architecture](http://technet.microsoft.com/en-us/library/jj150540%28v=exchg.150%29.aspx#BKMK_Arch) в статье [новые возможности Exchange 2013](http://technet.microsoft.com/en-us/library/jj150540%28v=exchg.150%29.aspx). 
  
## <a name="transport-agent-classes"></a>Классы агентов транспорта
<a name="Create"> </a>

Класс, производный от агента транспорта, определяет события, которые агент может зарегистрировать. Ваш агент обычно содержит класс агента, фабрику агентов, один или несколько обработчиков событий, а также код, выполняющий действия, которые должен выполнять агент.
  
В следующей таблице перечислены классы, от которых наследуются типы агентов.
  
**Таблица 2. Классы агентов**

||||
|:-----|:-----|:-----|
|Тип агента  <br/> |Базовый класс фабрики  <br/> |Базовый класс агента  <br/> |
|Получение SMTP  <br/> |[смтпрецеивеажентфактори](https://msdn.microsoft.com/library/Microsoft.Exchange.Data.Transport.Smtp.SmtpReceiveAgentFactory.aspx) <br/> |[SmtpReceiveAgent](https://msdn.microsoft.com/library/Microsoft.Exchange.Data.Transport.Smtp.SmtpReceiveAgent.aspx) <br/> |
|Включен  <br/> |[раутингажентфактори](https://msdn.microsoft.com/library/Microsoft.Exchange.Data.Transport.Routing.RoutingAgentFactory.aspx) <br/> |[RoutingAgent](https://msdn.microsoft.com/library/Microsoft.Exchange.Data.Transport.Routing.RoutingAgent.aspx) <br/> |
|Delivery  <br/> |[Диспетчер\<деливеряжентфактори\>](https://msdn.microsoft.com/en-us/library/dd877550(v=exchg.150).aspx) <br/> |[DeliveryAgent](https://msdn.microsoft.com/en-us/library/microsoft.exchange.data.transport.delivery.deliveryagent(v=exchg.150).aspx) <br/> |
   
Эти базовые классы агентов и агентов предоставляют свойства и методы, которые можно использовать для доступа к событиям транспорта и сообщениям. Реализуйте классы в агенте, которые наследуются от этих классов. В производном классе фабрики агентов Переопределите метод **креатеажент** таким образом, чтобы он возвращал новый экземпляр класса агента. 
  
Аргументы, передаваемые событиям, могут содержать экземпляр класса [EmailMessage](https://msdn.microsoft.com/library/Microsoft.Exchange.Data.Transport.Email.EmailMessage.aspx) , с помощью которого можно изменить свойства и содержимое базового сообщения. В каждом событии доступны не все сведения о сообщении. Необходимо определить, какой агент и какое событие лучше всего подходит для задачи, которую необходимо выполнить. 
  
Следующие пространства имен содержат типы, которые можно использовать для чтения, записи и изменения сообщений в транспортном конвейере.
  
- [Microsoft. Exchange. Data. MIME. Encoders](https://msdn.microsoft.com/library/Microsoft.Exchange.Data.Mime.Encoders.aspx)
    
- [Microsoft. Exchange. Data. ContentTypes. iCalendar](https://msdn.microsoft.com/library/Microsoft.Exchange.Data.ContentTypes.iCalendar.aspx)
    
- [Microsoft. Exchange. Data. MIME](https://msdn.microsoft.com/library/Microsoft.Exchange.Data.Mime.aspx)
    
- [Microsoft. Exchange. Data. ContentTypes. TNEF](https://msdn.microsoft.com/library/Microsoft.Exchange.Data.ContentTypes.Tnef.aspx)
    
- [Microsoft. Exchange. Data. ContentTypes. vCard](https://msdn.microsoft.com/library/Microsoft.Exchange.Data.ContentTypes.vCard.aspx)
    
После того как вы запишете агент транспорта, вы [устанавливаете агент и управляете им](http://technet.microsoft.com/en-us/library/bb125175%28v=exchg.150%29.aspx) с помощью командной консоли Exchange. Дополнительные сведения см. в статье [Создание агентов транспорта для Exchange 2013](creating-transport-agents-for-exchange-2013.md). 
  
## <a name="see-also"></a>См. также

- [Агенты транспорта в Exchange](transport-agents-in-exchange-2013.md)    
- [Справочник по агентам транспорта для Exchange 2013](transport-agent-reference-for-exchange-2013.md)   
- [Чтение и изменение сообщений в транспортном конвейере Exchange 2013](reading-and-modifying-messages-in-the-exchange-2013-transport-pipeline.md)    
- [Новые возможности Exchange 2013](http://technet.microsoft.com/en-us/library/jj150540%28v=exchg.150%29.aspx)   
- [Архитектура ролей сервера Exchange 2013](http://blogs.technet.com/b/exchange/archive/2013/01/23/exchange-2013-server-role-architecture.aspx)    
- [Серверы почтовых ящиков и клиентского доступа](http://technet.microsoft.com/en-us/library/jj150519%28v=exchg.150%29.aspx)   
- [Почтовые потоки Exchange Server 2013](http://technet.microsoft.com/en-us/library/aa996349.aspx)
- [Маршрутизация почты Exchange Server 2013](http://technet.microsoft.com/en-us/library/aa998825%28v=exchg.150%29.aspx)   
- [PowerShell в Exchange Server (Командная консоль Exchange)](https://docs.microsoft.com/en-us/powershell/exchange/exchange-server/exchange-management-shell?view=exchange-ps)
    

