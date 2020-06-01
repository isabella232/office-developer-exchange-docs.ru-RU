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
description: Найдите сведения об элементах XML в файле конфигурации Agents. config и фетажентс. config в Exchange 2013.
ms.openlocfilehash: f19fe8316a78cef668db881e630562d3be8be64a
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/31/2020
ms.locfileid: "44461571"
---
# <a name="agents-configuration-file-elements-for-exchange-2013"></a>Элементы файла конфигурации агентов для Exchange 2013

Найдите сведения об элементах XML в файле конфигурации Agents. config и фетажентс. config в Exchange 2013.
  
**Применимо к:** Exchange Server 2013
  
При установке роли сервера клиентского доступа или сервера почтовых ящиков на сервере Exchange Installer создает XML-файл, содержащий сведения о конфигурации агентов, установленных на сервере. Вы не можете выполнять запись непосредственно в этот файл. 
  
Внешняя служба транспорта работает на серверах клиентского доступа и выполняет запись в файл с именем фетажентс. config. Служба транспорта и служба транспорта почтовых ящиков выполняются на серверах почтовых ящиков и записываются в файл с именем Agents. config. У компьютера, у которого есть роль сервера клиентского доступа и роль сервера почтовых ящиков, есть файл фетажентс. config и Agents. config. 
  
Единственный поддерживаемый способ записи в эти файлы — использование командлетов агента транспорта в командной консоли Exchange. Сведения о командлетах агента транспорта можно найти в разделе [командлеты обработки почты](https://technet.microsoft.com/library/aa998553%28v=exchg.150%29.aspx) на сайте TechNet. 
  
> [!NOTE]
> Для различения агентов, расширяющих службу транспорта переднего плана на сервере клиентского доступа и транспортной службе на сервере почтовых ящиков, Командлеты агента транспорта имеют параметр _TransportService_ со значением "Hub" для транспортной службы и сервера переднего плана для внешней серверной службы транспорта. 
  
Можно прочитать файл Agents. config или фетажентс. config, чтобы определить присутствие и сведения о конфигурации для одного или нескольких агентов на сервере. В этой документации представлена ссылка, которую можно использовать для чтения информации либо в файле Agents. config, либо в файле фетажентс. config. Формат обоих этих файлов один и тот же. В этой документации не приводятся сведения о том, как выполнять запись в файлы.
  
> [!CAUTION]
> Использование неподдерживаемых методов для записи в файл Agents. config или фетажентс. config может привести к непредвиденным результатам, в том числе отказам в службе транспорта или агентах транспорта или обоим. Не записывайте непосредственно ни один из этих файлов. Единственный поддерживаемый метод для записи в эти файлы заключается в использовании командлетов агента транспорта Exchange Management Shell. 
  
## <a name="location-of-the-transport-agent-configuration-files"></a>Расположение файлов конфигурации агента транспорта
<a name="bk_ConfigLoc"> </a>

При установке Exchange 2013 установщик создает XML-файл с именем Agents. config. Template или фетажентс. config. Template в зависимости от установленной роли сервера, в \<ExchangeInstallFolder\> папке \транспортролес\ажентс (где \<ExchangeInstallFolder\> — Папка, в которой установлено Exchange 2013). При установке роли сервера клиентского доступа Exchange 2013 копирует файл фетажентс. config. Template в фетажентс. config. При установке роли сервера почтовых ящиков Exchange 2013 копирует файл Agents. config. Template в Agents. config. Exchange 2013 считывает и записывает этот файл при изменении конфигурации агентов транспорта на сервере.
  
## <a name="verifying-a-transport-agent-installation"></a>Проверка установки агента транспорта
<a name="bk_verifyinstall"> </a>

Вы можете использовать возможности XML, предоставляемые .NET Framework для чтения и проверки файла Agents. config или XML-файла фетажентс. config. Чтобы проверить установку и конфигурацию агента транспорта, прочтите XML-код в файле конфигурации и найдите элемент [Agent](agent.md) , соответствующий агенту транспорта. Если элемент **Agent** для определенного агента транспорта не существует, агент транспорта не установлен. Если агент транспорта установлен, можно прочитать атрибуты элемента **Agent** , чтобы определить его конфигурацию. 
  
## <a name="configuration-file-element-hierarchy"></a>Иерархия элементов файла конфигурации
<a name="bk_elementref"> </a>

В приведенном ниже коде показана иерархия элементов в XML-файле конфигурации.
  
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

## <a name="in-this-section"></a>В этой статье
<a name="bk_elementreflist"> </a>

- [агента](agent.md)
    
- [ажентексекутион](agentexecution.md)
    
- [ажентлист](agentlist.md)
    
- [configuration](configuration.md)
    
- [мессажеснапшот](messagesnapshot.md)
    
- [мексрунтиме](mexruntime.md)
    
- [текущего](monitoring.md)
    
## <a name="see-also"></a>См. также

- [Агенты транспорта в Exchange](transport-agents-in-exchange-2013.md)
- [Основные понятия, связанные с агентами транспорта в Exchange 2013](transport-agent-concepts-in-exchange-2013.md)
- [Справочник по агентам транспорта для Exchange 2013](transport-agent-reference-for-exchange-2013.md)
- [Пространства имен агента транспорта в Exchange 2013](transport-agent-namespaces-in-exchange-2013.md)
- [Командлеты почтового процесса](https://docs.microsoft.com/powershell/exchange/?view=exchange-ps)
    

