---
title: Обнаружение конечных точек автообнаружения с помощью поиска SCP в Exchange
manager: kelbow
ms.date: 09/17/2015
ms.audience: Developer
localization_priority: Normal
ms.assetid: b24228a8-5127-4bac-aef0-9c9e8843c9ff
description: Информация, содержащаяся в этом документе, может относиться к функциям и продуктам предварительной версии и может претерпеть значительные изменения до окончательного коммерческого выпуска. Настоящий документ предоставляется "как есть" и служит только для информационных целей. Корпорация Майкрософт не предоставляет никаких гарантий, явных или подразумеваемых, в связи с этим документом Сведения о том, как найти объекты точек подключения к службе автообнаружения в доменных службах Active Directory (AD DS), чтобы с их помощью находить URL-адреса конечных точек автообнаружения, которые затем будут использоваться совместно со службой автообнаружения Exchange.
ms.openlocfilehash: 59fd316d0aa0feea81b60c279040da018c51b47d
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/25/2018
ms.locfileid: "19761001"
---
# <a name="find-autodiscover-endpoints-by-using-scp-lookup-in-exchange"></a><span data-ttu-id="bf952-103">Обнаружение конечных точек автообнаружения с помощью поиска SCP в Exchange</span><span class="sxs-lookup"><span data-stu-id="bf952-103">How to: Find Autodisover endpoints by using SCP lookup in Exchange</span></span>

<span data-ttu-id="bf952-104">Информация, содержащаяся в этом документе, может относиться к функциям и продуктам предварительной версии и может претерпеть значительные изменения до окончательного коммерческого выпуска. Настоящий документ предоставляется "как есть" и служит только для информационных целей. Корпорация Майкрософт не предоставляет никаких гарантий, явных или подразумеваемых, в связи с этим документом Сведения о том, как найти объекты точек подключения к службе автообнаружения в доменных службах Active Directory (AD DS), чтобы с их помощью находить URL-адреса конечных точек автообнаружения, которые затем будут использоваться совместно со службой автообнаружения Exchange.</span><span class="sxs-lookup"><span data-stu-id="bf952-104">Find out how to locate Autodiscover SCP objects in Active Directory Domain Services (AD DS) and use them to find Autodiscover endpoint URLs to use with the Exchange Autodiscover service.</span></span>
  
<span data-ttu-id="bf952-p101">С помощью автообнаружения можно легко получить сведения, необходимые для подключения к почтовым ящиками на серверах Exchange. Однако, чтобы использовать эту функцию, требуется отыскать сервера автообнаружения, соответствующие пользователю, для которого извлекаются данные параметры. С помощью объектов точек подключения к службе (объектов SCP) в AD DS клиенты, присоединенные к домену, могут вести поиск на серверах автообнаружения.</span><span class="sxs-lookup"><span data-stu-id="bf952-p101">Autodiscover makes it easy to retrieve information that you need to connect to mailboxes on Exchange servers. However, in order to use Autodiscover, you need a way to find Autodiscover servers that are appropriate for the user you're retrieving settings for. Service connection point (SCP) objects in AD DS provide an easy way for domain-joined clients to look up Autodiscover servers.</span></span> 
  
## <a name="get-set-up-to-find-autodiscover-endpoints"></a><span data-ttu-id="bf952-108">Настройка поиска конечных точек автообнаружения</span><span class="sxs-lookup"><span data-stu-id="bf952-108">Get set up to find Autodiscover endpoints</span></span>
<span data-ttu-id="bf952-109"><a name="bk_PreReqs"> </a></span><span class="sxs-lookup"><span data-stu-id="bf952-109"></span></span>

<span data-ttu-id="bf952-110">Чтобы найти объекты точек подключения к службе автообнаружения в AD DS, вам потребуется доступ:</span><span class="sxs-lookup"><span data-stu-id="bf952-110">To locate Autodiscover SCP objects in AD DS, you need to have access to the following:</span></span>
  
- <span data-ttu-id="bf952-111">к серверу с запущенной на нем локальной версией Exchange, начиная с Exchange 2007 с пакетом обновления 1 (SP1);</span><span class="sxs-lookup"><span data-stu-id="bf952-111">A server that is running a version of Exchange on-premises starting with Exchange 2007 SP1.</span></span>
    
- <span data-ttu-id="bf952-112">клиентскому компьютеру, присоединенному к домену, на котором установлен сервер Exchange;</span><span class="sxs-lookup"><span data-stu-id="bf952-112">A client computer that is joined to the domain that the Exchange server is installed in.</span></span>
    
- <span data-ttu-id="bf952-113">учетной записи пользователя, имеющего почтовый ящик на сервере Exchange.</span><span class="sxs-lookup"><span data-stu-id="bf952-113">A user account that has a mailbox on the Exchange server.</span></span> 
    
<span data-ttu-id="bf952-p102">Кроме того, прежде чем начать, рекомендуем ознакомиться с некоторыми основными понятиями. Ниже приведены ресурсы, которые вам в этом помогут.</span><span class="sxs-lookup"><span data-stu-id="bf952-p102">Also, before you begin, you'll want to be familiar some basic concepts. The following are some resources that you'll find helpful.</span></span>
  
<span data-ttu-id="bf952-116">**Таблица 1. Статьи, касающиеся поиска конечных точек автообнаружения из объектов SCP**</span><span class="sxs-lookup"><span data-stu-id="bf952-116">**Table 1. Related articles for finding Autodiscover endpoints from SCP objects**</span></span>

|<span data-ttu-id="bf952-117">**Прочитайте эту статью**</span><span class="sxs-lookup"><span data-stu-id="bf952-117">**Read this article**</span></span>|<span data-ttu-id="bf952-118">**Здесь описывается…**</span><span class="sxs-lookup"><span data-stu-id="bf952-118">**To learn about…**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="bf952-119">Автообнаружение для Exchange</span><span class="sxs-lookup"><span data-stu-id="bf952-119">Autodiscover for Exchange</span></span>](autodiscover-for-exchange.md) <br/> |<span data-ttu-id="bf952-120">Как работает служба автообнаружения.</span><span class="sxs-lookup"><span data-stu-id="bf952-120">How the Autodiscover service works.</span></span>  <br/> |
|[<span data-ttu-id="bf952-121">Публикация с помощью точек подключения службы</span><span class="sxs-lookup"><span data-stu-id="bf952-121">Publishing with Service Connection Points</span></span>](http://msdn.microsoft.com/library/3544aa64-ecb0-48a1-ae49-05247a983842%28Office.15%29.aspx) <br/> |<span data-ttu-id="bf952-122">Как используются объекты SCP для публикации данных соответствующей службы.</span><span class="sxs-lookup"><span data-stu-id="bf952-122">How SCP objects are used to publish service-specific data.</span></span>  <br/> |
   
## <a name="locate-autodiscover-scp-objects-in-ad-ds"></a><span data-ttu-id="bf952-123">Поиск объектов точек подключения к службе автообнаружения в AD DS</span><span class="sxs-lookup"><span data-stu-id="bf952-123">Locate Autodiscover SCP objects in AD DS</span></span>
<span data-ttu-id="bf952-124"><a name="bk_LocateScpObjects"> </a></span><span class="sxs-lookup"><span data-stu-id="bf952-124"></span></span>

<span data-ttu-id="bf952-p103">Чтобы найти конечные точки автообнаружения, опубликованные в AD DS, нужно сперва найти объекты точек подключения к службе автообнаружения. В Exchange публикуется два типа объектов SCP для автообнаружения:</span><span class="sxs-lookup"><span data-stu-id="bf952-p103">The first step toward finding Autodiscover endpoints published in AD DS is to locate the Autodiscover SCP objects. Exchange publishes two types of SCP objects for Autodiscover:</span></span>
  
- <span data-ttu-id="bf952-p104">**Указатели SCP**: в них содержатся сведения, указывающие на соответствующие LDAP-серверы, которые нужно использовать, чтобы найти объекты точек подключения к службе автообнаружения для домена пользователя. GUID указателей SCP: 67661d7F-8FC4-4fa7-BFAC-E1D7794C1F68.</span><span class="sxs-lookup"><span data-stu-id="bf952-p104">**SCP pointers** — These contain information that points to specific LDAP servers that should be used to locate Autodiscover SCP objects for the user's domain. SCP pointers are stamped with the following GUID: 67661d7F-8FC4-4fa7-BFAC-E1D7794C1F68.</span></span> 
    
- <span data-ttu-id="bf952-p105">**URL-адреса SCP**: в них содержатся URL-адреса конечных точек автообнаружения. GUID URL-адресов SCP: 77378F46-2C66-4aa9-A6A6-3E7A48B19596.</span><span class="sxs-lookup"><span data-stu-id="bf952-p105">**SCP URLs** — These contain URLs for Autodiscover endpoints. SCP URLs are stamped with the following GUID: 77378F46-2C66-4aa9-A6A6-3E7A48B19596.</span></span> 
    
### <a name="to-locate-autodiscover-scp-objects"></a><span data-ttu-id="bf952-131">Поиск объектов точек подключения к службе автообнаружения</span><span class="sxs-lookup"><span data-stu-id="bf952-131">To locate Autodiscover SCP objects</span></span>

1. <span data-ttu-id="bf952-p106">Ознакомьтесь со свойством **configurationNamingContext** корневой DSE записи в AD DS, чтобы узнать путь для контекста именования конфигурации для домена. Это можно сделать с помощью класса [DirectoryEntry](http://msdn2.microsoft.com/ru-RU/library/z9cddzaa) или с помощью любого интерфейса API, имеющего доступ к AD DS.</span><span class="sxs-lookup"><span data-stu-id="bf952-p106">Read the **configurationNamingContext** property of the root DSE entry in AD DS to get the path to the configuration naming context for the domain. You can do this by using the [DirectoryEntry](http://msdn2.microsoft.com/ru-RU/library/z9cddzaa) class, or any other API that can acces AD DS.</span></span> 
    
2. <span data-ttu-id="bf952-134">В контексте именования конфигурации найдите объекты SCP, которые в свойстве **keywords** имеют соответствующий идентификатор GUID для указателя SCP или URL-адреса SCP.</span><span class="sxs-lookup"><span data-stu-id="bf952-134">Search for SCP objects in the configuration naming context that have either the SCP pointer GUID or the SCP URL GUID in the **keywords** property.</span></span> 
    
3. <span data-ttu-id="bf952-135">Проверьте объекты SCP, которые вы обнаружили для указателя SCP, находящегося в области пользовательского домена, запустив проверку **ключевых слов** для записи `"Domain=<domain>"`.</span><span class="sxs-lookup"><span data-stu-id="bf952-135">Check the SCP objects you found for an SCP pointer that is scoped to the user's domain by checking the **keywords** property for an entry equal to `"Domain=<domain>"`.</span></span> <span data-ttu-id="bf952-136">Например, для адреса электронной почты пользователя elvin@contoso.com нужно искать указатель SCP с записью `"Domain=contoso.com"` в свойствах **keywords**.</span><span class="sxs-lookup"><span data-stu-id="bf952-136">For example, if the user's email address is elvin@contoso.com, you would look for an SCP pointer with an entry in the **keywords** property that is equal to `"Domain=contoso.com"`.</span></span> <span data-ttu-id="bf952-137">Если найден совпадающий указатель SCP, удалите группу объектов SCP и начните снова с шага 1, используя значение свойства **serviceBindingInformation** в качестве сервера для подключения к записи Root DSE.</span><span class="sxs-lookup"><span data-stu-id="bf952-137">If a matching SCP pointer is found, discard the set of SCP objects and start over at step 1 using the value of the **serviceBindingInformation** property as the server to connect to for the Root DSE entry.</span></span> 
    
4. <span data-ttu-id="bf952-138">Если не удалось найти ни одного указателя SCP, относящегося к домену пользователя, найдите указатели SCP, которые не относятся ни к одному домену, и сохраните значение свойства **serviceBindingInformation** в качестве "резервного" сервера, на случай если поиск для текущего сервера не принесет результатов.</span><span class="sxs-lookup"><span data-stu-id="bf952-138">If you don't find any SCP pointers scoped to the user's domain, check for any SCP pointers that aren't scoped to any domain, and save the value of the **serviceBindingInformation** property as a "fallback" server, in case the current server doesn't give you any results.</span></span> 
    
5. <span data-ttu-id="bf952-139">Если не удалось найти ни одного указателя SCP, относящегося к домену, переходите к следующему шагу: оформите полученные результаты в виде приоритетного списка конечных точек автообнаружения.</span><span class="sxs-lookup"><span data-stu-id="bf952-139">If you didn't find any SCP pointers scoped to the domain, you're ready to move on to the next step: generating a prioritized list of Autodiscover endpoints from your results.</span></span>
    
## <a name="generate-a-prioritized-list-of-autodiscover-endpoints"></a><span data-ttu-id="bf952-140">Создание приоритетного списка конечных точек автообнаружения</span><span class="sxs-lookup"><span data-stu-id="bf952-140">Generate a prioritized list of Autodiscover endpoints</span></span>
<span data-ttu-id="bf952-141"><a name="bk_GenerateList"> </a></span><span class="sxs-lookup"><span data-stu-id="bf952-141"></span></span>

<span data-ttu-id="bf952-142">Чтобы создать приоритетный список URL-адресов конечных точек автообнаружения с помощью набора найденных вами объектов SCP, следуйте инструкциям ниже.</span><span class="sxs-lookup"><span data-stu-id="bf952-142">You can generate a prioritized list of Autodiscover endpoint URLs, using the set of SCP objects that you located, by doing the following:</span></span>
  
1. <span data-ttu-id="bf952-143">Получите имя сайта Active Directory на клиентском компьютере.</span><span class="sxs-lookup"><span data-stu-id="bf952-143">Get the Active Directory site name of the client computer.</span></span>
    
2. <span data-ttu-id="bf952-144">Проверьте свойство **keywords** для всех URL-адресов точек подключения службы, входящих в набор найденных объектов SCP, и присвойте URL-адресам приоритет, основываясь на следующих правилах:</span><span class="sxs-lookup"><span data-stu-id="bf952-144">Check the **keywords** property on each SCP URL in the set of SCP objects you found, and assign a priority to the URL based on the following rules:</span></span> 
    
  - <span data-ttu-id="bf952-145">Если для свойства **keywords** указано значение `"Site=<site name>"`, где `<site name>` соответствует сайту Active Directory, полученному в предыдущем шаге, присвойте этому URL-адресу приоритет "1".</span><span class="sxs-lookup"><span data-stu-id="bf952-145">If the keywords property contains a value of "Site=<site name>", where <site name> equals the name of the Active Directory site you retrieved in the previous step, assign the URL a priority of 1.</span></span> 
    
  - <span data-ttu-id="bf952-146">Если свойство **keywords** не содержит запись со значением, начинающимся с выражения `"Site="`, присвойте этому URL-адресу приоритет "2".</span><span class="sxs-lookup"><span data-stu-id="bf952-146">If the keywords property does not contain an entry with a value that starts with "Site=", assign the URL a priority of 2.</span></span> 
    
  - <span data-ttu-id="bf952-147">Если для свойства **keywords** указано значение `"Site=<site name>`, где `<site name>` не совпадает с именем сайта Active Directory, полученным в предыдущем шаге, присвойте такому URL-адресу приоритет "3".</span><span class="sxs-lookup"><span data-stu-id="bf952-147">If the keywords property contains a value of "Site=<site name>, where <site name> does not equal the name of the Active Directory site you retrieved in the previous step, assign the URL a priority of 3.</span></span> 
    
## <a name="code-example-performing-an-scp-lookup"></a><span data-ttu-id="bf952-148">Пример кода: подстановка SCP</span><span class="sxs-lookup"><span data-stu-id="bf952-148">Code example: Performing an SCP lookup</span></span>
<span data-ttu-id="bf952-149"><a name="bk_CodeExample"> </a></span><span class="sxs-lookup"><span data-stu-id="bf952-149"></span></span>

<span data-ttu-id="bf952-150">Ниже приводится пример кода, с помощью которого можно найти объекты точек подключения службы автообнаружения и составить приоритетный список конечных точек автообнаружения.</span><span class="sxs-lookup"><span data-stu-id="bf952-150">In the following code example, you'll see how to locate Autodiscover SCP objects and generate a prioritized list of Autodiscover endpoints.</span></span>
  
```cs
using System;
using System.Collections.Generic;
using System.DirectoryServices;
using System.DirectoryServices.ActiveDirectory;
namespace ScpLookup
{
    // This sample is for demonstration purposes only. Before you run this sample, make sure 
    // that the code meets the coding requirements of your organization. 
    class Program
    {
        static void Main(string[] args)
        {
            string domain = args[0];
            Console.WriteLine("Performing SCP lookup for {0}.", domain);
            List<string> scpUrls = GetScpUrls(null, domain);
            Console.WriteLine("\nOrdered List of Autodiscover endpoints:");
            foreach (string url in scpUrls)
            {
                Console.WriteLine("  {0}", url);
            }
            Console.WriteLine("SCP lookup done.");
        }
        // GUID for SCP URL keyword.
        private const string ScpUrlGuidString = @"77378F46-2C66-4aa9-A6A6-3E7A48B19596";
        // GUID for SCP pointer keyword.
        private const string ScpPtrGuidString = @"67661d7F-8FC4-4fa7-BFAC-E1D7794C1F68";
        static List<string> GetScpUrls(string ldapServer, string domain)
        {
            // Create a new list to return.
            List<string> scpUrlList = new List<string>();
            string rootDSEPath = null;
            // If ldapServer is null/empty, use LDAP://RootDSE to
            // connect to Active Directory Domain Services (AD DS). Otherwise, use
            // LDAP://SERVERNAME/RootDSE to connect to a specific server.
            if (string.IsNullOrEmpty(ldapServer))
            {
                rootDSEPath = "LDAP://RootDSE";
            }
            else
            {
                rootDSEPath = ldapServer + "/RootDSE";
            }
            SearchResultCollection scpEntries = null;
            try
            {
                // Get the root directory entry.
                DirectoryEntry rootDSE = new DirectoryEntry(rootDSEPath);
                // Get the configuration path.
                string configPath = rootDSE.Properties["configurationNamingContext"].Value as string;
                // Get the configuration entry.
                DirectoryEntry configEntry = new DirectoryEntry("LDAP://" + configPath);
                // Create a search object for the configuration entry.
                DirectorySearcher configSearch = new DirectorySearcher(configEntry);
                // Set the search filter to find SCP URLs and SCP pointers.
                configSearch.Filter = "(&amp;(objectClass=serviceConnectionPoint)" +
                    "(|(keywords=" + ScpPtrGuidString + ")(keywords=" + ScpUrlGuidString + ")))";
                // Specify which properties you want to retrieve.
                configSearch.PropertiesToLoad.Add("keywords");
                configSearch.PropertiesToLoad.Add("serviceBindingInformation");
                scpEntries = configSearch.FindAll();
            }
            catch (Exception ex)
            {
                Console.WriteLine("SCP lookup failed with: ");
                Console.WriteLine(ex.ToString());
            }
            // If no SCP entries were found, then exit.
            if (scpEntries == null || scpEntries.Count <= 0)
            {
                Console.WriteLine("No SCP records found.");
                return null;
            }
            string fallBackLdapPath = null;
            // Check for SCP pointers.
            foreach (SearchResult scpEntry in scpEntries)
            {
                ResultPropertyValueCollection entryKeywords = scpEntry.Properties["keywords"];
                if (CollectionContainsExactValue(entryKeywords, ScpPtrGuidString))
                {
                    string ptrLdapPath = scpEntry.Properties["serviceBindingInformation"][0] as string;
                    // Determine whether this pointer is scoped to the user's domain.
                    if (CollectionContainsExactValue(entryKeywords, "Domain=" + domain))
                    {
                        Console.WriteLine("Found SCP pointer for " + domain + " in " + scpEntry.Path);
                        // Restart SCP lookup with the server assigned for the domain.
                        Console.WriteLine("Restarting SCP lookup in " + ptrLdapPath);
                        return GetScpUrls(ptrLdapPath, domain);
                    }
                    else
                    {
                        // Save the first SCP pointer that is not scoped to a domain as a fallback
                        // in case you do not get any results from this server.
                        if (entryKeywords.Count == 1 &amp;&amp; string.IsNullOrEmpty(fallBackLdapPath))
                        {
                            fallBackLdapPath = ptrLdapPath;
                            Console.WriteLine("Saved fallback SCP pointer: " + fallBackLdapPath);
                        }
                    }
                }
            }
            string computerSiteName = null;
            try
            {
                // Get the name of the ActiveDirectorySite the computer
                // belongs to (if it belongs to one).
                ActiveDirectorySite site = ActiveDirectorySite.GetComputerSite();
                computerSiteName = site.Name;
                Console.WriteLine("Local computer in site: " + computerSiteName);
            }
            catch (Exception ex)
            {
                Console.WriteLine("Unable to get computer site name.");
                Console.WriteLine(ex.ToString());
            }
            if (!string.IsNullOrEmpty(computerSiteName))
            {
                // Scan the search results for SCP URLs.
                // SCP URLs fit into three tiers:
                //   Priority 1: The URL is scoped to the computer's Active Directory site.
                //   Priority 2: The URL is not scoped to any Active Directory site.
                //   Priority 3: The URL is scoped to a different Active Directory site.
                // Temporary lists to hold priority 2 and 3 URLs.
                List<string> priorityTwoUrls = new List<string>();
                List<string> priorityThreeUrls = new List<string>();
                foreach (SearchResult scpEntry in scpEntries)
                {
                    ResultPropertyValueCollection entryKeywords = scpEntry.Properties["keywords"];
                    // Check for SCP URLs.
                    if (CollectionContainsExactValue(entryKeywords, ScpUrlGuidString))
                    {
                        string scpUrlPath = scpEntry.Properties["adsPath"][0] as string;
                        Console.WriteLine("SCP URL found at {0}", scpUrlPath);
                        string scpUrl = scpEntry.Properties["serviceBindingInformation"][0] as string;
                        scpUrl = scpUrl.ToLower();
                        // Determine whether this entry is scoped to the computer's site.
                        if (CollectionContainsExactValue(entryKeywords, "Site=" + computerSiteName))
                        {
                            // Priority 1.
                            if (!scpUrlList.Contains(scpUrl.ToLower()))
                            {
                                Console.WriteLine("Adding priority 1 SCP URL: {0}", scpUrl.ToLower());
                                scpUrlList.Add(scpUrl);
                            }
                            else
                            {
                                Console.WriteLine("Priority 1 SCP URL already found: {0}", scpUrl);
                            }
                        }
                        else
                        {
                            // Determine whether this is a priority 2 or 3 URL.
                            if (CollectionContainsPrefixValue(entryKeywords, "Site="))
                            {
                                // Priority 3.
                                if (!priorityThreeUrls.Contains(scpUrl))
                                {
                                    Console.WriteLine("Adding priority 3 SCP URL: {0}", scpUrl);
                                    priorityThreeUrls.Add(scpUrl);
                                }
                                else
                                {
                                    Console.WriteLine("Priority 3 SCP URL already found: {0}", scpUrl);
                                }
                            }
                            else
                            {
                                // Priority 2.
                                if (!priorityTwoUrls.Contains(scpUrl))
                                {
                                    Console.WriteLine("Adding priority 2 SCP URL: {0}", scpUrl);
                                    priorityTwoUrls.Add(scpUrl);
                                }
                                else
                                {
                                    Console.WriteLine("Priority 2 SCP URL already found: {0}", scpUrl);
                                }
                            }
                        }
                    }
                }
                // Now add the priority 2 URLs into the main list.
                foreach (string priorityTwoUrl in priorityTwoUrls)
                {
                    // If the URL is already in the list as a priority 1, 
                    // don't add it again.
                    if (!scpUrlList.Contains(priorityTwoUrl))
                    {
                        scpUrlList.Add(priorityTwoUrl);
                    }
                }
                // Now add the priority 3 URLs into the main list.
                foreach (string priorityThreeUrl in priorityThreeUrls)
                {
                    // If the URL is already in the list as a priority 1
                    // or priority 2, don't add it again.
                    if (!scpUrlList.Contains(priorityThreeUrl))
                    {
                        scpUrlList.Add(priorityThreeUrl);
                    }
                }
                // If after all this, you still have no URLs in your list,
                // try the fallback SCP pointer, if you have one.
                if (scpUrlList.Count == 0 &amp;&amp; fallBackLdapPath != null)
                {
                    return GetScpUrls(fallBackLdapPath, domain);
                }
            }
            return scpUrlList;
        }
        private static bool CollectionContainsExactValue(ResultPropertyValueCollection collection, string value)
        {
            foreach (object obj in collection)
            {
                string entry = obj as string;
                if (entry != null)
                {
                    if (string.Compare(value, entry, true) == 0)
                        return true;
                }
            }
            return false;
        }
        private static bool CollectionContainsPrefixValue(ResultPropertyValueCollection collection, string value)
        {
            foreach (object obj in collection)
            {
                string entry = obj as string;
                if (entry != null)
                {
                    if (entry.StartsWith(value))
                        return true;
                }
            }
            return false;
        }
    }
}
```

## <a name="next-steps"></a><span data-ttu-id="bf952-151">Дальнейшие действия</span><span class="sxs-lookup"><span data-stu-id="bf952-151">Next steps</span></span>
<span data-ttu-id="bf952-152"><a name="bk_NextSteps"> </a></span><span class="sxs-lookup"><span data-stu-id="bf952-152"></span></span>

<span data-ttu-id="bf952-p108">На следующем этапе процесса автообнаружения необходимо отправить запросы автообнаружения на найденные ранее URL-адреса в соответствии с присвоенными им приоритетами: сначала на URL-адреса с приоритетом "1", затем  на URL-адреса с приоритетом "2" и, наконец, на URL-адреса с приоритетом "3". Больше об отправке запросов автообнаружения и их обработке можно узнать в следующих статьях:</span><span class="sxs-lookup"><span data-stu-id="bf952-p108">The next step in the Autodiscover process is to send Autodiscover requests to the URLs that you found, starting with priority 1 URLs, then priority 2 URLs, and finally priority 3 URLs. To learn more about how to send Autodiscover requests and handle responses, read the following articles:</span></span>
  
- [<span data-ttu-id="bf952-155">Получение параметров пользователя из Exchange с помощью службы автообнаружения</span><span class="sxs-lookup"><span data-stu-id="bf952-155">How to: Get user settings from Exchange by using Autodiscover</span></span>](how-to-get-user-settings-from-exchange-by-using-autodiscover.md)
    
- [<span data-ttu-id="bf952-156">Обработка сообщений об ошибках службы автообнаружения</span><span class="sxs-lookup"><span data-stu-id="bf952-156">Handling Autodiscover error messages</span></span>](handling-autodiscover-error-messages.md)
    
## <a name="see-also"></a><span data-ttu-id="bf952-157">См. также</span><span class="sxs-lookup"><span data-stu-id="bf952-157">See also</span></span>

- [<span data-ttu-id="bf952-158">Автообнаружение в Exchange</span><span class="sxs-lookup"><span data-stu-id="bf952-158">Autodiscover for Exchange</span></span>](autodiscover-for-exchange.md)   
- [<span data-ttu-id="bf952-159">Настройка приложения веб-служб Exchange</span><span class="sxs-lookup"><span data-stu-id="bf952-159">Setting up your EWS application</span></span>](setting-up-your-ews-application.md)
    

