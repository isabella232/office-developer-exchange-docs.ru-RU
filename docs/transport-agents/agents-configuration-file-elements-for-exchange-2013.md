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
# <a name="agents-configuration-file-elements-for-exchange-2013"></a><span data-ttu-id="77272-103">Элементы файла конфигурации агентов для Exchange 2013</span><span class="sxs-lookup"><span data-stu-id="77272-103">Agents configuration file elements for Exchange 2013</span></span>

<span data-ttu-id="77272-104">Сведения о XML-элементы в файле конфигурации agents.config и fetagents.config в Exchange 2013.</span><span class="sxs-lookup"><span data-stu-id="77272-104">Find information about the XML elements in the agents.config and fetagents.config configuration file in Exchange 2013.</span></span>
  
<span data-ttu-id="77272-105">**Применимо к:** Exchange Server 2013</span><span class="sxs-lookup"><span data-stu-id="77272-105">**Applies to:** Exchange Server 2013</span></span>
  
<span data-ttu-id="77272-106">При установке клиентского доступа или роль сервера почтовых ящиков на сервере Exchange, программа установки создает XML-файл, содержащий сведения о конфигурации об агентах, установленных на сервере.</span><span class="sxs-lookup"><span data-stu-id="77272-106">When you install the Client Access or the Mailbox server role on an Exchange server, the installer creates an XML file that contains configuration information about agents that are installed on the server.</span></span> <span data-ttu-id="77272-107">Не удается записать непосредственно к этому разделу.</span><span class="sxs-lookup"><span data-stu-id="77272-107">You cannot write directly to this file.</span></span> 
  
<span data-ttu-id="77272-108">Служба транспорта переднего плана запускается на серверы клиентского доступа и записывает данные в файл с именем fetagents.config. Транспортная служба и служба транспорта почтовых ящиков выполняются на серверах почтовых ящиков и записи в файл с именем agents.config. Компьютер с ролью сервера клиентского доступа и роли сервера почтовых ящиков будут иметь fetagents.config и в файле agents.config.</span><span class="sxs-lookup"><span data-stu-id="77272-108">The Front End Transport service runs on Client Access servers and writes to a file named fetagents.config. The Transport service and the Mailbox Transport service run on Mailbox servers, and write to a file named agents.config. A computer that has both the Client Access server role and the Mailbox server role will have both a fetagents.config and an agents.config file.</span></span> 
  
<span data-ttu-id="77272-109">— Это единственный способ записывать в эти файлы с помощью командлетов агента транспорта в командной консоли Exchange.</span><span class="sxs-lookup"><span data-stu-id="77272-109">The only supported way to write to these files is by using the transport agent cmdlets in the Exchange Management Shell.</span></span> <span data-ttu-id="77272-110">Сведения о командлеты агента транспорта содержатся [Командлеты потока обработки почты](http://technet.microsoft.com/en-us/library/aa998553%28v=exchg.150%29.aspx) на сайте TechNet.</span><span class="sxs-lookup"><span data-stu-id="77272-110">For information about the transport agent cmdlets, see [Mail Flow Cmdlets](http://technet.microsoft.com/en-us/library/aa998553%28v=exchg.150%29.aspx) on TechNet.</span></span> 
  
> [!NOTE]
> <span data-ttu-id="77272-111">Чтобы различать агентов, которые расширяют транспортной службы на сервере клиентского доступа и транспортной службы на сервере почтовых ящиков, командлеты агента транспорта указан параметр _TransportService_ со значением «Сервер-концентратор» транспорта службы и «FrontEnd» для службы транспорта переднего плана.</span><span class="sxs-lookup"><span data-stu-id="77272-111">To distinguish between agents that extend the Front End Transport service on the Client Access server and the Transport service on the Mailbox server, transport agent cmdlets have a  _TransportService_ parameter with a value of "Hub" for the Transport service and "FrontEnd" for the Front End Transport service.</span></span> 
  
<span data-ttu-id="77272-112">Для получения agents.config или fetagents.config файл, чтобы определить наличие и данные конфигурации для одного или нескольких агентов на сервере.</span><span class="sxs-lookup"><span data-stu-id="77272-112">You can read the agents.config or fetagents.config file to determine the presence of and configuration information for one or more agents on the server.</span></span> <span data-ttu-id="77272-113">В этой документации содержит ссылки, которые можно использовать для чтения сведений в файле agents.config или fetagents.config. Используется тот же формат для обоих этих файлов.</span><span class="sxs-lookup"><span data-stu-id="77272-113">This documentation provides a reference that you can use to read the information in either the agents.config file or the fetagents.config. The format for both of these files is the same.</span></span> <span data-ttu-id="77272-114">В этой документации не предоставляет сведения о том, как выполнить запись в файлы.</span><span class="sxs-lookup"><span data-stu-id="77272-114">This documentation does not provide information about how to write to the files.</span></span>
  
> [!CAUTION]
> <span data-ttu-id="77272-115">С помощью неподдерживаемые методы для записи в файл agents.config или fetagents.config может привести к непредсказуемым последствиям, в том числе сбоя службы транспорта или агенты транспорта.</span><span class="sxs-lookup"><span data-stu-id="77272-115">Using unsupported methods to write to the agents.config file or fetagents.config can produce unexpected results, including failure of the transport service or transport agents, or both.</span></span> <span data-ttu-id="77272-116">Не записываются непосредственно в любой из этих файлов.</span><span class="sxs-lookup"><span data-stu-id="77272-116">Do not write directly to either of these files.</span></span> <span data-ttu-id="77272-117">С помощью командлетов командной консоли Exchange транспортных агентов является единственным поддерживаемым способом при записи в эти файлы.</span><span class="sxs-lookup"><span data-stu-id="77272-117">The only supported method for writing to these files is by using the Exchange Management Shell transport agent cmdlets.</span></span> 
  
## <a name="location-of-the-transport-agent-configuration-files"></a><span data-ttu-id="77272-118">Расположение файлов конфигурации агента транспорта</span><span class="sxs-lookup"><span data-stu-id="77272-118">Location of the transport agent configuration files</span></span>
<span data-ttu-id="77272-119"><a name="bk_ConfigLoc"> </a></span><span class="sxs-lookup"><span data-stu-id="77272-119"></span></span>

<span data-ttu-id="77272-120">Когда вы устанавливаете Exchange 2013, программа установки создает XML-файл с именем agents.config.template или fetagents.config.template, в зависимости от роли сервера, установленные в \<ExchangeInstallFolder\>\TransportRoles\Agents папка (где \<ExchangeInstallFolder\> — это папка, в которой установлен Exchange 2013).</span><span class="sxs-lookup"><span data-stu-id="77272-120">When you install Exchange 2013, the installer creates an XML file that is named either agents.config.template or fetagents.config.template, depending on the server role installed, in the \<ExchangeInstallFolder\>\TransportRoles\Agents folder (where \<ExchangeInstallFolder\> is the folder in which you installed Exchange 2013).</span></span> <span data-ttu-id="77272-121">При установке роли сервера клиентского доступа Exchange 2013 копирует файл fetagents.config.template fetagents.config. При установке роли сервера почтовых ящиков Exchange 2013 копирует файл agents.config.template agents.config. Exchange 2013 чтение и запись этого файла при изменении конфигурации агенты транспорта на сервере.</span><span class="sxs-lookup"><span data-stu-id="77272-121">If you install the Client Access server role, Exchange 2013 copies the fetagents.config.template file to fetagents.config. If you install the Mailbox server role, Exchange 2013 copies the agents.config.template file to agents.config. Exchange 2013 reads and writes this file when you change the transport agents configuration on the server.</span></span>
  
## <a name="verifying-a-transport-agent-installation"></a><span data-ttu-id="77272-122">Проверка установки агента транспорта</span><span class="sxs-lookup"><span data-stu-id="77272-122">Verifying a transport agent installation</span></span>
<span data-ttu-id="77272-123"><a name="bk_verifyinstall"> </a></span><span class="sxs-lookup"><span data-stu-id="77272-123"></span></span>

<span data-ttu-id="77272-124">Можно использовать возможности XML, которые предоставляет .NET Framework для чтения и проверки agents.config или fetagents.config XML-файл.</span><span class="sxs-lookup"><span data-stu-id="77272-124">You can use the XML capabilities that the .NET Framework provides to read and validate the agents.config or the fetagents.config XML file.</span></span> <span data-ttu-id="77272-125">Проверка установки и настройки агента транспорта, чтение XML-файла конфигурации и найдите элемент [агента](agent.md) , соответствующий агента транспорта.</span><span class="sxs-lookup"><span data-stu-id="77272-125">To verify the installation and configuration of a transport agent, read the XML in the configuration file and find the [agent](agent.md) element that corresponds to the transport agent.</span></span> <span data-ttu-id="77272-126">Если элемент **агентов** для агента транспорта конкретных не существует, агента транспорта не установлен.</span><span class="sxs-lookup"><span data-stu-id="77272-126">If an **agent** element for the specific transport agent does not exist, the transport agent is not installed.</span></span> <span data-ttu-id="77272-127">Если установлен агента транспорта, могут читать атрибуты элемента **агента** для определения его конфигурации.</span><span class="sxs-lookup"><span data-stu-id="77272-127">If the transport agent is installed, you can read the attributes of the **agent** element to determine its configuration.</span></span> 
  
## <a name="configuration-file-element-hierarchy"></a><span data-ttu-id="77272-128">Элемент иерархии файла конфигурации</span><span class="sxs-lookup"><span data-stu-id="77272-128">Configuration file element hierarchy</span></span>
<span data-ttu-id="77272-129"><a name="bk_elementref"> </a></span><span class="sxs-lookup"><span data-stu-id="77272-129"></span></span>

<span data-ttu-id="77272-130">В следующем коде показан элемент иерархии в XML-файл конфигурации.</span><span class="sxs-lookup"><span data-stu-id="77272-130">The following code shows the element hierarchy in the configuration XML file.</span></span>
  
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

## <a name="in-this-section"></a><span data-ttu-id="77272-131">В этом разделе</span><span class="sxs-lookup"><span data-stu-id="77272-131">In this section</span></span>
<span data-ttu-id="77272-132"><a name="bk_elementreflist"> </a></span><span class="sxs-lookup"><span data-stu-id="77272-132"></span></span>

- [<span data-ttu-id="77272-133">агент</span><span class="sxs-lookup"><span data-stu-id="77272-133">agent</span></span>](agent.md)
    
- [<span data-ttu-id="77272-134">agentExecution</span><span class="sxs-lookup"><span data-stu-id="77272-134">agentExecution</span></span>](agentexecution.md)
    
- [<span data-ttu-id="77272-135">agentList</span><span class="sxs-lookup"><span data-stu-id="77272-135">agentList</span></span>](agentlist.md)
    
- [<span data-ttu-id="77272-136">Конфигурация</span><span class="sxs-lookup"><span data-stu-id="77272-136">configuration</span></span>](configuration.md)
    
- [<span data-ttu-id="77272-137">messageSnapshot</span><span class="sxs-lookup"><span data-stu-id="77272-137">messageSnapshot</span></span>](messagesnapshot.md)
    
- [<span data-ttu-id="77272-138">mexRuntime</span><span class="sxs-lookup"><span data-stu-id="77272-138">mexRuntime</span></span>](mexruntime.md)
    
- [<span data-ttu-id="77272-139">мониторинг</span><span class="sxs-lookup"><span data-stu-id="77272-139">monitoring</span></span>](monitoring.md)
    
## <a name="see-also"></a><span data-ttu-id="77272-140">См. также</span><span class="sxs-lookup"><span data-stu-id="77272-140">See also</span></span>

- [<span data-ttu-id="77272-141">Агенты транспорта в Exchange</span><span class="sxs-lookup"><span data-stu-id="77272-141">Transport agents in Exchange</span></span>](transport-agents-in-exchange-2013.md)
- [<span data-ttu-id="77272-142">Транспорта концепции агентов в Exchange 2013</span><span class="sxs-lookup"><span data-stu-id="77272-142">Transport agent concepts in Exchange 2013</span></span>](transport-agent-concepts-in-exchange-2013.md)
- [<span data-ttu-id="77272-143">Справочник по агента транспорта для Exchange 2013</span><span class="sxs-lookup"><span data-stu-id="77272-143">Transport agent reference for Exchange 2013</span></span>](transport-agent-reference-for-exchange-2013.md)
- [<span data-ttu-id="77272-144">Транспорта агента пространства имен в Exchange 2013</span><span class="sxs-lookup"><span data-stu-id="77272-144">Transport agent namespaces in Exchange 2013</span></span>](transport-agent-namespaces-in-exchange-2013.md)
- [<span data-ttu-id="77272-145">Командлеты потока обработки почты</span><span class="sxs-lookup"><span data-stu-id="77272-145">Mail Flow Cmdlets</span></span>](https://docs.microsoft.com/en-us/powershell/exchange/?view=exchange-ps)
    

