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
ms.lasthandoff: 06/03/2020
ms.locfileid: "44461571"
---
# <a name="agents-configuration-file-elements-for-exchange-2013"></a><span data-ttu-id="6c115-103">Элементы файла конфигурации агентов для Exchange 2013</span><span class="sxs-lookup"><span data-stu-id="6c115-103">Agents configuration file elements for Exchange 2013</span></span>

<span data-ttu-id="6c115-104">Найдите сведения об элементах XML в файле конфигурации Agents. config и фетажентс. config в Exchange 2013.</span><span class="sxs-lookup"><span data-stu-id="6c115-104">Find information about the XML elements in the agents.config and fetagents.config configuration file in Exchange 2013.</span></span>
  
<span data-ttu-id="6c115-105">**Применимо к:** Exchange Server 2013</span><span class="sxs-lookup"><span data-stu-id="6c115-105">**Applies to:** Exchange Server 2013</span></span>
  
<span data-ttu-id="6c115-106">При установке роли сервера клиентского доступа или сервера почтовых ящиков на сервере Exchange Installer создает XML-файл, содержащий сведения о конфигурации агентов, установленных на сервере.</span><span class="sxs-lookup"><span data-stu-id="6c115-106">When you install the Client Access or the Mailbox server role on an Exchange server, the installer creates an XML file that contains configuration information about agents that are installed on the server.</span></span> <span data-ttu-id="6c115-107">Вы не можете выполнять запись непосредственно в этот файл.</span><span class="sxs-lookup"><span data-stu-id="6c115-107">You cannot write directly to this file.</span></span> 
  
<span data-ttu-id="6c115-108">Внешняя служба транспорта работает на серверах клиентского доступа и выполняет запись в файл с именем фетажентс. config. Служба транспорта и служба транспорта почтовых ящиков выполняются на серверах почтовых ящиков и записываются в файл с именем Agents. config. У компьютера, у которого есть роль сервера клиентского доступа и роль сервера почтовых ящиков, есть файл фетажентс. config и Agents. config.</span><span class="sxs-lookup"><span data-stu-id="6c115-108">The Front End Transport service runs on Client Access servers and writes to a file named fetagents.config. The Transport service and the Mailbox Transport service run on Mailbox servers, and write to a file named agents.config. A computer that has both the Client Access server role and the Mailbox server role will have both a fetagents.config and an agents.config file.</span></span> 
  
<span data-ttu-id="6c115-109">Единственный поддерживаемый способ записи в эти файлы — использование командлетов агента транспорта в командной консоли Exchange.</span><span class="sxs-lookup"><span data-stu-id="6c115-109">The only supported way to write to these files is by using the transport agent cmdlets in the Exchange Management Shell.</span></span> <span data-ttu-id="6c115-110">Сведения о командлетах агента транспорта можно найти в разделе [командлеты обработки почты](https://technet.microsoft.com/library/aa998553%28v=exchg.150%29.aspx) на сайте TechNet.</span><span class="sxs-lookup"><span data-stu-id="6c115-110">For information about the transport agent cmdlets, see [Mail Flow Cmdlets](https://technet.microsoft.com/library/aa998553%28v=exchg.150%29.aspx) on TechNet.</span></span> 
  
> [!NOTE]
> <span data-ttu-id="6c115-111">Для различения агентов, расширяющих службу транспорта переднего плана на сервере клиентского доступа и транспортной службе на сервере почтовых ящиков, Командлеты агента транспорта имеют параметр _TransportService_ со значением "Hub" для транспортной службы и сервера переднего плана для внешней серверной службы транспорта.</span><span class="sxs-lookup"><span data-stu-id="6c115-111">To distinguish between agents that extend the Front End Transport service on the Client Access server and the Transport service on the Mailbox server, transport agent cmdlets have a  _TransportService_ parameter with a value of "Hub" for the Transport service and "FrontEnd" for the Front End Transport service.</span></span> 
  
<span data-ttu-id="6c115-112">Можно прочитать файл Agents. config или фетажентс. config, чтобы определить присутствие и сведения о конфигурации для одного или нескольких агентов на сервере.</span><span class="sxs-lookup"><span data-stu-id="6c115-112">You can read the agents.config or fetagents.config file to determine the presence of and configuration information for one or more agents on the server.</span></span> <span data-ttu-id="6c115-113">В этой документации представлена ссылка, которую можно использовать для чтения информации либо в файле Agents. config, либо в файле фетажентс. config. Формат обоих этих файлов один и тот же.</span><span class="sxs-lookup"><span data-stu-id="6c115-113">This documentation provides a reference that you can use to read the information in either the agents.config file or the fetagents.config. The format for both of these files is the same.</span></span> <span data-ttu-id="6c115-114">В этой документации не приводятся сведения о том, как выполнять запись в файлы.</span><span class="sxs-lookup"><span data-stu-id="6c115-114">This documentation does not provide information about how to write to the files.</span></span>
  
> [!CAUTION]
> <span data-ttu-id="6c115-115">Использование неподдерживаемых методов для записи в файл Agents. config или фетажентс. config может привести к непредвиденным результатам, в том числе отказам в службе транспорта или агентах транспорта или обоим.</span><span class="sxs-lookup"><span data-stu-id="6c115-115">Using unsupported methods to write to the agents.config file or fetagents.config can produce unexpected results, including failure of the transport service or transport agents, or both.</span></span> <span data-ttu-id="6c115-116">Не записывайте непосредственно ни один из этих файлов.</span><span class="sxs-lookup"><span data-stu-id="6c115-116">Do not write directly to either of these files.</span></span> <span data-ttu-id="6c115-117">Единственный поддерживаемый метод для записи в эти файлы заключается в использовании командлетов агента транспорта Exchange Management Shell.</span><span class="sxs-lookup"><span data-stu-id="6c115-117">The only supported method for writing to these files is by using the Exchange Management Shell transport agent cmdlets.</span></span> 
  
## <a name="location-of-the-transport-agent-configuration-files"></a><span data-ttu-id="6c115-118">Расположение файлов конфигурации агента транспорта</span><span class="sxs-lookup"><span data-stu-id="6c115-118">Location of the transport agent configuration files</span></span>
<span data-ttu-id="6c115-119"><a name="bk_ConfigLoc"> </a></span><span class="sxs-lookup"><span data-stu-id="6c115-119"><a name="bk_ConfigLoc"> </a></span></span>

<span data-ttu-id="6c115-120">При установке Exchange 2013 установщик создает XML-файл с именем Agents. config. Template или фетажентс. config. Template в зависимости от установленной роли сервера, в \<ExchangeInstallFolder\> папке \транспортролес\ажентс (где \<ExchangeInstallFolder\> — Папка, в которой установлено Exchange 2013).</span><span class="sxs-lookup"><span data-stu-id="6c115-120">When you install Exchange 2013, the installer creates an XML file that is named either agents.config.template or fetagents.config.template, depending on the server role installed, in the \<ExchangeInstallFolder\>\TransportRoles\Agents folder (where \<ExchangeInstallFolder\> is the folder in which you installed Exchange 2013).</span></span> <span data-ttu-id="6c115-121">При установке роли сервера клиентского доступа Exchange 2013 копирует файл фетажентс. config. Template в фетажентс. config. При установке роли сервера почтовых ящиков Exchange 2013 копирует файл Agents. config. Template в Agents. config. Exchange 2013 считывает и записывает этот файл при изменении конфигурации агентов транспорта на сервере.</span><span class="sxs-lookup"><span data-stu-id="6c115-121">If you install the Client Access server role, Exchange 2013 copies the fetagents.config.template file to fetagents.config. If you install the Mailbox server role, Exchange 2013 copies the agents.config.template file to agents.config. Exchange 2013 reads and writes this file when you change the transport agents configuration on the server.</span></span>
  
## <a name="verifying-a-transport-agent-installation"></a><span data-ttu-id="6c115-122">Проверка установки агента транспорта</span><span class="sxs-lookup"><span data-stu-id="6c115-122">Verifying a transport agent installation</span></span>
<span data-ttu-id="6c115-123"><a name="bk_verifyinstall"> </a></span><span class="sxs-lookup"><span data-stu-id="6c115-123"><a name="bk_verifyinstall"> </a></span></span>

<span data-ttu-id="6c115-124">Вы можете использовать возможности XML, предоставляемые .NET Framework для чтения и проверки файла Agents. config или XML-файла фетажентс. config.</span><span class="sxs-lookup"><span data-stu-id="6c115-124">You can use the XML capabilities that the .NET Framework provides to read and validate the agents.config or the fetagents.config XML file.</span></span> <span data-ttu-id="6c115-125">Чтобы проверить установку и конфигурацию агента транспорта, прочтите XML-код в файле конфигурации и найдите элемент [Agent](agent.md) , соответствующий агенту транспорта.</span><span class="sxs-lookup"><span data-stu-id="6c115-125">To verify the installation and configuration of a transport agent, read the XML in the configuration file and find the [agent](agent.md) element that corresponds to the transport agent.</span></span> <span data-ttu-id="6c115-126">Если элемент **Agent** для определенного агента транспорта не существует, агент транспорта не установлен.</span><span class="sxs-lookup"><span data-stu-id="6c115-126">If an **agent** element for the specific transport agent does not exist, the transport agent is not installed.</span></span> <span data-ttu-id="6c115-127">Если агент транспорта установлен, можно прочитать атрибуты элемента **Agent** , чтобы определить его конфигурацию.</span><span class="sxs-lookup"><span data-stu-id="6c115-127">If the transport agent is installed, you can read the attributes of the **agent** element to determine its configuration.</span></span> 
  
## <a name="configuration-file-element-hierarchy"></a><span data-ttu-id="6c115-128">Иерархия элементов файла конфигурации</span><span class="sxs-lookup"><span data-stu-id="6c115-128">Configuration file element hierarchy</span></span>
<span data-ttu-id="6c115-129"><a name="bk_elementref"> </a></span><span class="sxs-lookup"><span data-stu-id="6c115-129"><a name="bk_elementref"> </a></span></span>

<span data-ttu-id="6c115-130">В приведенном ниже коде показана иерархия элементов в XML-файле конфигурации.</span><span class="sxs-lookup"><span data-stu-id="6c115-130">The following code shows the element hierarchy in the configuration XML file.</span></span>
  
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

## <a name="in-this-section"></a><span data-ttu-id="6c115-131">В этой статье</span><span class="sxs-lookup"><span data-stu-id="6c115-131">In this section</span></span>
<span data-ttu-id="6c115-132"><a name="bk_elementreflist"> </a></span><span class="sxs-lookup"><span data-stu-id="6c115-132"><a name="bk_elementreflist"> </a></span></span>

- [<span data-ttu-id="6c115-133">агента</span><span class="sxs-lookup"><span data-stu-id="6c115-133">agent</span></span>](agent.md)
    
- [<span data-ttu-id="6c115-134">ажентексекутион</span><span class="sxs-lookup"><span data-stu-id="6c115-134">agentExecution</span></span>](agentexecution.md)
    
- [<span data-ttu-id="6c115-135">ажентлист</span><span class="sxs-lookup"><span data-stu-id="6c115-135">agentList</span></span>](agentlist.md)
    
- [<span data-ttu-id="6c115-136">configuration</span><span class="sxs-lookup"><span data-stu-id="6c115-136">configuration</span></span>](configuration.md)
    
- [<span data-ttu-id="6c115-137">мессажеснапшот</span><span class="sxs-lookup"><span data-stu-id="6c115-137">messageSnapshot</span></span>](messagesnapshot.md)
    
- [<span data-ttu-id="6c115-138">мексрунтиме</span><span class="sxs-lookup"><span data-stu-id="6c115-138">mexRuntime</span></span>](mexruntime.md)
    
- [<span data-ttu-id="6c115-139">текущего</span><span class="sxs-lookup"><span data-stu-id="6c115-139">monitoring</span></span>](monitoring.md)
    
## <a name="see-also"></a><span data-ttu-id="6c115-140">См. также</span><span class="sxs-lookup"><span data-stu-id="6c115-140">See also</span></span>

- [<span data-ttu-id="6c115-141">Агенты транспорта в Exchange</span><span class="sxs-lookup"><span data-stu-id="6c115-141">Transport agents in Exchange</span></span>](transport-agents-in-exchange-2013.md)
- [<span data-ttu-id="6c115-142">Основные понятия, связанные с агентами транспорта в Exchange 2013</span><span class="sxs-lookup"><span data-stu-id="6c115-142">Transport agent concepts in Exchange 2013</span></span>](transport-agent-concepts-in-exchange-2013.md)
- [<span data-ttu-id="6c115-143">Справочник по агентам транспорта для Exchange 2013</span><span class="sxs-lookup"><span data-stu-id="6c115-143">Transport agent reference for Exchange 2013</span></span>](transport-agent-reference-for-exchange-2013.md)
- [<span data-ttu-id="6c115-144">Пространства имен агента транспорта в Exchange 2013</span><span class="sxs-lookup"><span data-stu-id="6c115-144">Transport agent namespaces in Exchange 2013</span></span>](transport-agent-namespaces-in-exchange-2013.md)
- [<span data-ttu-id="6c115-145">Командлеты почтового процесса</span><span class="sxs-lookup"><span data-stu-id="6c115-145">Mail Flow Cmdlets</span></span>](https://docs.microsoft.com/powershell/exchange/?view=exchange-ps)
    

