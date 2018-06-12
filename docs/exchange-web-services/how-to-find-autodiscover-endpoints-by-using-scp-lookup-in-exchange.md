---
title: Найдите конечных точек службы автообнаружения с помощью поиска SCP в Exchange
manager: kelbow
ms.date: 09/17/2015
ms.audience: Developer
localization_priority: Normal
ms.assetid: b24228a8-5127-4bac-aef0-9c9e8843c9ff
description: Информация, содержащаяся в этом документе, может относиться к функциям и продуктам предварительной версии и может претерпеть значительные изменения до окончательного коммерческого выпуска. Настоящий документ предоставляется "как есть" и служит только для информационных целей. Корпорация Майкрософт не предоставляет никаких гарантий, явных или подразумеваемых, в связи с этим документом Сведения о том, как найти объекты точек подключения к службе автообнаружения в доменных службах Active Directory (AD DS), чтобы с их помощью находить URL-адреса конечных точек автообнаружения, которые затем будут использоваться совместно со службой автообнаружения Exchange.
ms.openlocfilehash: 59fd316d0aa0feea81b60c279040da018c51b47d
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/11/2018
ms.locfileid: "19761001"
---
# <a name="find-autodiscover-endpoints-by-using-scp-lookup-in-exchange"></a>Найдите конечных точек службы автообнаружения с помощью поиска SCP в Exchange

Информация, содержащаяся в этом документе, может относиться к функциям и продуктам предварительной версии и может претерпеть значительные изменения до окончательного коммерческого выпуска. Настоящий документ предоставляется "как есть" и служит только для информационных целей. Корпорация Майкрософт не предоставляет никаких гарантий, явных или подразумеваемых, в связи с этим документом Сведения о том, как найти объекты точек подключения к службе автообнаружения в доменных службах Active Directory (AD DS), чтобы с их помощью находить URL-адреса конечных точек автообнаружения, которые затем будут использоваться совместно со службой автообнаружения Exchange.
  
С помощью автообнаружения можно легко получить сведения, необходимые для подключения к почтовым ящиками на серверах Exchange. Однако, чтобы использовать эту функцию, требуется отыскать сервера автообнаружения, соответствующие пользователю, для которого извлекаются данные параметры. С помощью объектов точек подключения к службе (объектов SCP) в AD DS клиенты, присоединенные к домену, могут вести поиск на серверах автообнаружения. 
  
## <a name="get-set-up-to-find-autodiscover-endpoints"></a>Настройка поиска конечных точек автообнаружения
<a name="bk_PreReqs"> </a>

Чтобы найти объекты точек подключения к службе автообнаружения в AD DS, вам потребуется доступ:
  
- к серверу с запущенной на нем локальной версией Exchange, начиная с Exchange 2007 с пакетом обновления 1 (SP1);
    
- клиентскому компьютеру, присоединенному к домену, на котором установлен сервер Exchange;
    
- учетной записи пользователя, имеющего почтовый ящик на сервере Exchange. 
    
Кроме того, прежде чем начать, рекомендуем ознакомиться с некоторыми основными понятиями. Ниже приведены ресурсы, которые вам в этом помогут.
  
**Таблица 1. Статьи, касающиеся поиска конечных точек автообнаружения из объектов SCP**

|**Прочитайте эту статью**|**Здесь описывается…**|
|:-----|:-----|
|[Автообнаружение для Exchange](autodiscover-for-exchange.md) <br/> |Как работает служба автообнаружения.  <br/> |
|[Публикация с помощью точек подключения службы](http://msdn.microsoft.com/library/3544aa64-ecb0-48a1-ae49-05247a983842%28Office.15%29.aspx) <br/> |Как используются объекты SCP для публикации данных соответствующей службы.  <br/> |
   
## <a name="locate-autodiscover-scp-objects-in-ad-ds"></a>Поиск объектов точек подключения к службе автообнаружения в AD DS
<a name="bk_LocateScpObjects"> </a>

Чтобы найти конечные точки автообнаружения, опубликованные в AD DS, нужно сперва найти объекты точек подключения к службе автообнаружения. В Exchange публикуется два типа объектов SCP для автообнаружения:
  
- **Указатели SCP**: в них содержатся сведения, указывающие на соответствующие LDAP-серверы, которые нужно использовать, чтобы найти объекты точек подключения к службе автообнаружения для домена пользователя. GUID указателей SCP: 67661d7F-8FC4-4fa7-BFAC-E1D7794C1F68. 
    
- **URL-адреса SCP**: в них содержатся URL-адреса конечных точек автообнаружения. GUID URL-адресов SCP: 77378F46-2C66-4aa9-A6A6-3E7A48B19596. 
    
### <a name="to-locate-autodiscover-scp-objects"></a>Поиск объектов точек подключения к службе автообнаружения

1. Ознакомьтесь со свойством **configurationNamingContext** корневой DSE записи в AD DS, чтобы узнать путь для контекста именования конфигурации для домена. Это можно сделать с помощью класса [DirectoryEntry](http://msdn2.microsoft.com/EN-US/library/z9cddzaa) или с помощью любого интерфейса API, имеющего доступ к AD DS. 
    
2. В контексте именования конфигурации найдите объекты SCP, которые в свойстве **keywords** имеют соответствующий идентификатор GUID для указателя SCP или URL-адреса SCP. 
    
3. Проверьте точку подключения службы объектов найдено для указатель точки подключения службы, предназначенную для пользователя домена, обращаясь к свойству **ключевые слова** для записи равно `"Domain=<domain>"`. К примеру, если адрес электронной почты пользователя elvin@contoso.com, необходимо найти соответствующую указатель SCP с записью в свойстве **ключевые слова** , равный `"Domain=contoso.com"`. При обнаружении соответствия указатель точки подключения службы, отменить набор объектов точки подключения службы и переходит на шаге 1, с помощью значение свойства **serviceBindingInformation** сервером для подключения к корневым DSE запись. 
    
4. Если не удалось найти ни одного указателя SCP, относящегося к домену пользователя, найдите указатели SCP, которые не относятся ни к одному домену, и сохраните значение свойства **serviceBindingInformation** в качестве "резервного" сервера, на случай если поиск для текущего сервера не принесет результатов. 
    
5. Если не удалось найти ни одного указателя SCP, относящегося к домену, переходите к следующему шагу: оформите полученные результаты в виде приоритетного списка конечных точек автообнаружения.
    
## <a name="generate-a-prioritized-list-of-autodiscover-endpoints"></a>Создание приоритетного списка конечных точек автообнаружения
<a name="bk_GenerateList"> </a>

Чтобы создать приоритетный список URL-адресов конечных точек автообнаружения с помощью набора найденных вами объектов SCP, следуйте инструкциям ниже.
  
1. Получите имя сайта Active Directory на клиентском компьютере.
    
2. Проверьте свойство **keywords** для всех URL-адресов точек подключения службы, входящих в набор найденных объектов SCP, и присвойте URL-адресам приоритет, основываясь на следующих правилах: 
    
  - Если свойство **ключевые слова** , содержит значение `"Site=<site name>"`, где `<site name>` равно имя Active Directory веб-сайтов можно получить на предыдущем шаге, назначение URL-адрес приоритет 1. 
    
  - Если свойство **ключевых слов** не содержит записи со значением, начинающимся с `"Site="`, назначьте приоритет 2 URL-адрес. 
    
  - Если свойство **ключевые слова** , содержит значение `"Site=<site name>`, где `<site name>` не равно имя сайта Active Directory, полученные на предыдущем шаге, назначение URL-адрес с приоритетом 3. 
    
## <a name="code-example-performing-an-scp-lookup"></a>Пример кода: поиск точек подключения службы
<a name="bk_CodeExample"> </a>

Ниже приводится пример кода, с помощью которого можно найти объекты точек подключения службы автообнаружения и составить приоритетный список конечных точек автообнаружения.
  
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

## <a name="next-steps"></a>Дальнейшие действия
<a name="bk_NextSteps"> </a>

На следующем этапе процесса автообнаружения необходимо отправить запросы автообнаружения на найденные ранее URL-адреса в соответствии с присвоенными им приоритетами: сначала на URL-адреса с приоритетом "1", затем  на URL-адреса с приоритетом "2" и, наконец, на URL-адреса с приоритетом "3". Больше об отправке запросов автообнаружения и их обработке можно узнать в следующих статьях:
  
- [Получить параметры пользователя из Exchange с помощью службы автообнаружения](how-to-get-user-settings-from-exchange-by-using-autodiscover.md)
    
- [Обработка сообщений об ошибках службы автообнаружения](handling-autodiscover-error-messages.md)
    
## <a name="see-also"></a>См. также

- [Автообнаружение для Exchange](autodiscover-for-exchange.md)   
- [Настройка приложения веб-служб Exchange](setting-up-your-ews-application.md)
    

