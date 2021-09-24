---
title: Элементы конфигурации файлов агентов для Exchange 2013 г.
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: overview
ms.prod: office-online-server
ms.localizationpriority: medium
api_name:
- Agents
api_type:
- schema
ms.assetid: 3047653b-d712-46c1-ae0a-73f3975f5e9d
description: Сведения об элементах XML можно найти в agents.config и fetagents.config в Exchange 2013 г.
ms.openlocfilehash: bdf394130f7818c5b956e8b15eed86a6318b9698
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/24/2021
ms.locfileid: "59510423"
---
# <a name="agents-configuration-file-elements-for-exchange-2013"></a>Элементы конфигурации файлов агентов для Exchange 2013 г.

Сведения об элементах XML можно найти в agents.config и fetagents.config в Exchange 2013 г.
  
**Применяется к:** Exchange Server 2013 г.
  
При установке клиентского доступа или роли сервера почтовых ящиков на Exchange сервере установщик создает XML-файл, содержащий сведения о конфигурации агентов, установленных на сервере. Вы не можете написать непосредственно в этот файл. 
  
Передняя транспортная служба работает на серверах клиентского доступа и записывает в файл с именем fetagents.config. Служба транспорта и служба транспорта почтовых ящиков работают на серверах почтовых ящиков и записывают в файл с именем agents.config. Компьютер с ролью сервера клиентского доступа и ролью сервера почтовых ящиков будет иметь как fetagents.config, так и agents.config файл. 
  
Единственный поддерживаемый способ записи этих файлов — это использование комлетов транспортного агента в Exchange Management Shell. Сведения о комлетах транспортного агента см. в Flow [в](https://technet.microsoft.com/library/aa998553%28v=exchg.150%29.aspx) TechNet. 
  
> [!NOTE]
> Чтобы отличить агентов, которые расширяют службу переднего конечного транспорта на сервере клиентского доступа, и службу транспорта на сервере почтовых ящиков, командалеты транспортных агентов имеют параметр  _TransportService_ со значением "Концентратор" для транспортной службы и "FrontEnd" для передней транспортной службы. 
  
Вы можете прочитать agents.config или fetagents.config, чтобы определить наличие и конфигурацию данных для одного или более агентов на сервере. В этой документации содержится ссылка, которую можно использовать для чтения сведений в agents.config или fetagents.config. Формат обоих этих файлов один и тот же. Эта документация не предоставляет сведений о записи в файлы.
  
> [!CAUTION]
> Использование неподтверждаемого метода записи в файл agents.config или fetagents.config может привести к неожиданным результатам, включая сбой транспортной службы или транспортных агентов, или оба. Не записывай непосредственно ни в один из этих файлов. Единственный поддерживаемый метод записи этих файлов — это использование Exchange агентов транспортного агента management Shell. 
  
## <a name="location-of-the-transport-agent-configuration-files"></a>Расположение файлов конфигурации транспортного агента
<a name="bk_ConfigLoc"> </a>

При установке Exchange 2013 г. установщик создает XML-файл с именем agents.config.template или fetagents.config.template в зависимости от установленной роли сервера в папке \TransportRoles\Agents (где находится папка, в которой установлена \<ExchangeInstallFolder\> \<ExchangeInstallFolder\> Exchange 2013 г.). Если вы установите роль сервера клиентского доступа, Exchange 2013 г. копирует файл fetagents.config.template для fetagents.config. При установке роли сервера почтовых ящиков Exchange 2013 г. agents.config.template файл agents.config. Exchange 2013 г. читает и записывает этот файл при изменении конфигурации транспортных агентов на сервере.
  
## <a name="verifying-a-transport-agent-installation"></a>Проверка установки транспортного агента
<a name="bk_verifyinstall"> </a>

Вы можете использовать возможности XML, которые предоставляет платформа .NET Framework для чтения и проверки agents.config или fetagents.config XML-файла. Чтобы проверить установку и конфигурацию транспортного агента, ознакомьтесь с [](agent.md) XML в файле конфигурации и найдите элемент агента, соответствующий транспортному агенту. Если элемента **агента** для конкретного транспортного агента не существует, транспортный агент не устанавливается. Если транспортный агент установлен, можно прочитать атрибуты элемента **агента,** чтобы определить его конфигурацию. 
  
## <a name="configuration-file-element-hierarchy"></a>Иерархия элементов файла конфигурации
<a name="bk_elementref"> </a>

В следующем коде показана иерархия элементов в XML-файле конфигурации.
  
```XML
<configuration>
    <mexRuntime>
        <monitoring>
            <agentExecution/>
            <messageSnapshot/>
        </monitoring>
        <agentList>
            <agent/>
            <agent/>
            <agent />
        </agentList>
    </mexRuntim>
</configuration>
```

## <a name="in-this-section"></a>В этом разделе:
<a name="bk_elementreflist"> </a>

- [агент](agent.md)
    
- [agentExecution](agentexecution.md)
    
- [agentList](agentlist.md)
    
- [configuration](configuration.md)
    
- [messageSnapshot](messagesnapshot.md)
    
- [mexRuntime](mexruntime.md)
    
- [мониторинг](monitoring.md)
    
## <a name="see-also"></a>См. также

- [Агенты транспорта в Exchange](transport-agents-in-exchange-2013.md)
- [Концепции транспортного агента в Exchange 2013 г.](transport-agent-concepts-in-exchange-2013.md)
- [Ссылка агента транспорта на Exchange 2013 г.](transport-agent-reference-for-exchange-2013.md)
- [Пространства имен транспортного агента в Exchange 2013 г.](transport-agent-namespaces-in-exchange-2013.md)
- [Почтовые Flow cmdlets](https://docs.microsoft.com/powershell/exchange/?view=exchange-ps)
    

