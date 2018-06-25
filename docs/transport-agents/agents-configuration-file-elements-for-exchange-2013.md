---
title: Элементы файла конфигурации агентов для Exchange 2013
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: overview
ms.prod: office-online-server
localization_priority: Normal
api_name:
- Agents
api_type:
- schema
ms.assetid: 3047653b-d712-46c1-ae0a-73f3975f5e9d
description: Сведения о XML-элементы в файле конфигурации agents.config и fetagents.config в Exchange 2013.
ms.openlocfilehash: dd58c4bc21a968db2ca5b13e0c53f7058b29f233
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/25/2018
ms.locfileid: "19761294"
---
# <a name="agents-configuration-file-elements-for-exchange-2013"></a>Элементы файла конфигурации агентов для Exchange 2013

Сведения о XML-элементы в файле конфигурации agents.config и fetagents.config в Exchange 2013.
  
**Применимо к:** Exchange Server 2013
  
При установке клиентского доступа или роль сервера почтовых ящиков на сервере Exchange, программа установки создает XML-файл, содержащий сведения о конфигурации об агентах, установленных на сервере. Не удается записать непосредственно к этому разделу. 
  
Служба транспорта переднего плана запускается на серверы клиентского доступа и записывает данные в файл с именем fetagents.config. Транспортная служба и служба транспорта почтовых ящиков выполняются на серверах почтовых ящиков и записи в файл с именем agents.config. Компьютер с ролью сервера клиентского доступа и роли сервера почтовых ящиков будут иметь fetagents.config и в файле agents.config. 
  
— Это единственный способ записывать в эти файлы с помощью командлетов агента транспорта в командной консоли Exchange. Сведения о командлеты агента транспорта содержатся [Командлеты потока обработки почты](http://technet.microsoft.com/en-us/library/aa998553%28v=exchg.150%29.aspx) на сайте TechNet. 
  
> [!NOTE]
> Чтобы различать агентов, которые расширяют транспортной службы на сервере клиентского доступа и транспортной службы на сервере почтовых ящиков, командлеты агента транспорта указан параметр _TransportService_ со значением «Сервер-концентратор» транспорта службы и «FrontEnd» для службы транспорта переднего плана. 
  
Для получения agents.config или fetagents.config файл, чтобы определить наличие и данные конфигурации для одного или нескольких агентов на сервере. В этой документации содержит ссылки, которые можно использовать для чтения сведений в файле agents.config или fetagents.config. Используется тот же формат для обоих этих файлов. В этой документации не предоставляет сведения о том, как выполнить запись в файлы.
  
> [!CAUTION]
> С помощью неподдерживаемые методы для записи в файл agents.config или fetagents.config может привести к непредсказуемым последствиям, в том числе сбоя службы транспорта или агенты транспорта. Не записываются непосредственно в любой из этих файлов. С помощью командлетов командной консоли Exchange транспортных агентов является единственным поддерживаемым способом при записи в эти файлы. 
  
## <a name="location-of-the-transport-agent-configuration-files"></a>Расположение файлов конфигурации агента транспорта
<a name="bk_ConfigLoc"> </a>

Когда вы устанавливаете Exchange 2013, программа установки создает XML-файл с именем agents.config.template или fetagents.config.template, в зависимости от роли сервера, установленные в \<ExchangeInstallFolder\>\TransportRoles\Agents папка (где \<ExchangeInstallFolder\> — это папка, в которой установлен Exchange 2013). При установке роли сервера клиентского доступа Exchange 2013 копирует файл fetagents.config.template fetagents.config. При установке роли сервера почтовых ящиков Exchange 2013 копирует файл agents.config.template agents.config. Exchange 2013 чтение и запись этого файла при изменении конфигурации агенты транспорта на сервере.
  
## <a name="verifying-a-transport-agent-installation"></a>Проверка установки агента транспорта
<a name="bk_verifyinstall"> </a>

Можно использовать возможности XML, которые предоставляет .NET Framework для чтения и проверки agents.config или fetagents.config XML-файл. Проверка установки и настройки агента транспорта, чтение XML-файла конфигурации и найдите элемент [агента](agent.md) , соответствующий агента транспорта. Если элемент **агентов** для агента транспорта конкретных не существует, агента транспорта не установлен. Если установлен агента транспорта, могут читать атрибуты элемента **агента** для определения его конфигурации. 
  
## <a name="configuration-file-element-hierarchy"></a>Элемент иерархии файла конфигурации
<a name="bk_elementref"> </a>

В следующем коде показан элемент иерархии в XML-файл конфигурации.
  
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

## <a name="in-this-section"></a>В этом разделе
<a name="bk_elementreflist"> </a>

- [агент](agent.md)
    
- [agentExecution](agentexecution.md)
    
- [agentList](agentlist.md)
    
- [Конфигурация](configuration.md)
    
- [messageSnapshot](messagesnapshot.md)
    
- [mexRuntime](mexruntime.md)
    
- [мониторинг](monitoring.md)
    
## <a name="see-also"></a>См. также

- [Агенты транспорта в Exchange](transport-agents-in-exchange-2013.md)
- [Транспорта концепции агентов в Exchange 2013](transport-agent-concepts-in-exchange-2013.md)
- [Справочник по агента транспорта для Exchange 2013](transport-agent-reference-for-exchange-2013.md)
- [Транспорта агента пространства имен в Exchange 2013](transport-agent-namespaces-in-exchange-2013.md)
- [Командлеты потока обработки почты](https://docs.microsoft.com/en-us/powershell/exchange/?view=exchange-ps)
    

