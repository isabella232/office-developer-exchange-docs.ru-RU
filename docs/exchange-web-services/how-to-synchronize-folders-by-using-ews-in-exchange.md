---
title: Синхронизация папок с помощью EWS в Exchange
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
localization_priority: Normal
ms.assetid: d3bbacd1-8e4b-4fd0-8d27-4cbbc045ec3f
description: Узнайте, как использовать управляемый API EWS или EWS для получения списка папок или списка папок, которые были изменены, чтобы синхронизировать клиент.
ms.openlocfilehash: e49fdaf2faf97c2369f2ad7dbb141c5ac3100884
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/03/2020
ms.locfileid: "44455865"
---
# <a name="synchronize-folders-by-using-ews-in-exchange"></a><span data-ttu-id="2fc86-103">Синхронизация папок с помощью EWS в Exchange</span><span class="sxs-lookup"><span data-stu-id="2fc86-103">Synchronize folders by using EWS in Exchange</span></span>

<span data-ttu-id="2fc86-104">Узнайте, как использовать управляемый API EWS или EWS для получения списка папок или списка папок, которые были изменены, чтобы синхронизировать клиент.</span><span class="sxs-lookup"><span data-stu-id="2fc86-104">Find out how to use the EWS Managed API or EWS to get a list of folders, or a list of folders that have changed, in order to synchronize your client.</span></span>
  
<span data-ttu-id="2fc86-105">Служба EWS в Exchange использует синхронизацию элементов и синхронизацию папок для синхронизации содержимого почтовых ящиков между клиентом и сервером.</span><span class="sxs-lookup"><span data-stu-id="2fc86-105">EWS in Exchange uses item synchronization and folder synchronization to sync mailbox content between the client and server.</span></span> <span data-ttu-id="2fc86-106">Синхронизация папок получает исходный список папок из корневой папки, а затем получает изменения, внесенные в эти папки, а также создает новые папки.</span><span class="sxs-lookup"><span data-stu-id="2fc86-106">Folder synchronization gets the initial list of folders from a root folder and then, over time, gets changes that were made to those folders and gets new folders as well.</span></span>
  
<span data-ttu-id="2fc86-107">Если вы выполняете синхронизацию папок с помощью управляемого API EWS, сначала необходимо [получить исходный список папок в корневой папке](how-to-synchronize-folders-by-using-ews-in-exchange.md#bk_cesyncinitialewsma) с помощью метода [ExchangeService. SyncFolderHierarchy](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.exchangeservice.syncfolderhierarchy%28v=exchg.80%29.aspx) .</span><span class="sxs-lookup"><span data-stu-id="2fc86-107">If you're performing folder synchronization by using the EWS Managed API, you first [get the initial list of folders in the root folder](how-to-synchronize-folders-by-using-ews-in-exchange.md#bk_cesyncinitialewsma) by using the [ExchangeService.SyncFolderHierarchy](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.exchangeservice.syncfolderhierarchy%28v=exchg.80%29.aspx) method.</span></span> <span data-ttu-id="2fc86-108">Затем необходимо обновить значение параметра _ксинкстате_ во время последующих вызовов, чтобы получить список новых и измененных папок.</span><span class="sxs-lookup"><span data-stu-id="2fc86-108">You then update the value of the  _cSyncState_ parameter during subsequent calls to get the list of new and changed folders.</span></span> 
  
<span data-ttu-id="2fc86-109">Чтобы выполнить синхронизацию папок с помощью EWS, запросите [исходный список папок в корневой папке](how-to-synchronize-folders-by-using-ews-in-exchange.md#bk_cesyncewsrequest) с помощью операции [SyncFolderHierarchy](https://msdn.microsoft.com/library/b31916b1-bc6c-4451-a475-b7c5417f752d%28Office.15%29.aspx) , выполните синтаксический анализ ответа, а затем в некоторый момент в будущем [получите изменения папок в корне](how-to-synchronize-folders-by-using-ews-in-exchange.md#bk_cesyncrespews)и проанализируйте ответ.</span><span class="sxs-lookup"><span data-stu-id="2fc86-109">To perform folder synchronization by using EWS, you request the [initial list of folders in the root folder](how-to-synchronize-folders-by-using-ews-in-exchange.md#bk_cesyncewsrequest) by using the [SyncFolderHierarchy](https://msdn.microsoft.com/library/b31916b1-bc6c-4451-a475-b7c5417f752d%28Office.15%29.aspx) operation, parse the response, and then at some point in the future [get the changes to the folders in the root](how-to-synchronize-folders-by-using-ews-in-exchange.md#bk_cesyncrespews), and parse the response.</span></span> <span data-ttu-id="2fc86-110">После получения клиентом списка начальной или измененной папки он [выполняет локальное обновление](how-to-synchronize-folders-by-using-ews-in-exchange.md#bk_nextsteps).</span><span class="sxs-lookup"><span data-stu-id="2fc86-110">After the client receives the list of initial or changed folders, it [makes updates locally](how-to-synchronize-folders-by-using-ews-in-exchange.md#bk_nextsteps).</span></span> <span data-ttu-id="2fc86-111">Как и когда вы извлечете изменения в будущем, зависит от [шаблона проекта синхронизации](mailbox-synchronization-and-ews-in-exchange.md#bk_syncpatterns) , используемого приложением.</span><span class="sxs-lookup"><span data-stu-id="2fc86-111">How and when you retrieve changes in the future depends on the [synchronization design pattern](mailbox-synchronization-and-ews-in-exchange.md#bk_syncpatterns) your application is using.</span></span> 
  
## <a name="get-the-list-of-all-folders-or-changed-folders-by-using-the-ews-managed-api"></a><span data-ttu-id="2fc86-112">Получение списка всех папок или измененных папок с помощью управляемого API EWS</span><span class="sxs-lookup"><span data-stu-id="2fc86-112">Get the list of all folders or changed folders by using the EWS Managed API</span></span>
<span data-ttu-id="2fc86-113"><a name="bk_cesyncinitialewsma"> </a></span><span class="sxs-lookup"><span data-stu-id="2fc86-113"><a name="bk_cesyncinitialewsma"> </a></span></span>

<span data-ttu-id="2fc86-114">В приведенном ниже примере кода показано, как получить исходный список папок в корневой папке, а затем получить список изменений в папках корневой папки, произошедших с момента предыдущей синхронизации.</span><span class="sxs-lookup"><span data-stu-id="2fc86-114">The following code example shows how to get an initial list of folders in a root folder and then get a list of changes to folders in the root folder that have occurred since the previous synchronization.</span></span> <span data-ttu-id="2fc86-115">Во время начального вызова метода [ExchangeService. SyncFolderHierarchy](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.exchangeservice.syncfolderhierarchy%28v=exchg.80%29.aspx) задайте для параметра _ксинкстате_ значение null.</span><span class="sxs-lookup"><span data-stu-id="2fc86-115">During the initial call to the [ExchangeService.SyncFolderHierarchy](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.exchangeservice.syncfolderhierarchy%28v=exchg.80%29.aspx) method, set the  _cSyncState_ value to null.</span></span> <span data-ttu-id="2fc86-116">После выполнения метода сохраните значение _ксинкстате_ локально, чтобы использовать его в следующем вызове метода **SyncFolderHierarchy** .</span><span class="sxs-lookup"><span data-stu-id="2fc86-116">When the method completes, save the  _cSyncState_ value locally to use in the next **SyncFolderHierarchy** method call.</span></span> <span data-ttu-id="2fc86-117">При первом вызове и последующих вызовах папки извлекаются в пакетах десяти, с помощью последовательных вызовов метода **SyncFolderHierarchy** , пока не будут сохранены другие изменения.</span><span class="sxs-lookup"><span data-stu-id="2fc86-117">In both the initial call and the subsequent calls, the folders are retrieved in batches of ten, by using successive calls to the **SyncFolderHierarchy** method, until no more changes remain.</span></span> <span data-ttu-id="2fc86-118">В этом примере параметру _Property_ присваивается значение идонли для уменьшения числа вызовов к базе данных Exchange, что является [наилучшим вариантом синхронизации](mailbox-synchronization-and-ews-in-exchange.md#bk_bestpractices).</span><span class="sxs-lookup"><span data-stu-id="2fc86-118">This example sets the  _propertySet_ parameter to IdOnly to reduce calls to the Exchange database, which is a [synchronization best practice](mailbox-synchronization-and-ews-in-exchange.md#bk_bestpractices).</span></span> <span data-ttu-id="2fc86-119">В этом примере предполагается, что **Служба** является допустимой привязкой объекта **ExchangeService** и _ксинкстате_ представляет состояние синхронизации, возвращенное предыдущим вызовом в **SyncFolderHierarchy**.</span><span class="sxs-lookup"><span data-stu-id="2fc86-119">In this example, we assume that **service** is a valid **ExchangeService** object binding and that  _cSyncState_ represents the sync state that was returned by a prior call to **SyncFolderHierarchy**.</span></span> 
  
```cs
// Get a list of all folders in the mailbox by calling SyncFolderHierarchy.
// The folderId parameter must be set to the root folder to synchronize. 
// The propertySet parameter is set to IdOnly to reduce calls to the Exchange database
// because any additional properties result in additional calls to the Exchange database. 
// The syncState parameter is set to cSyncState, which should be null in the initial call, 
// and should be set to the sync state returned by the previous SyncFolderHierarchy call 
// in subsequent calls.
ChangeCollection<FolderChange> fcc = service.SyncFolderHierarchy(new FolderId(WellKnownFolderName.Root), PropertySet.IdOnly, cSyncState);
// If the count of changes is zero, there are no changes to synchronize.
if (fcc.Count == 0)
{
    Console.WriteLine("There are no folders to synchronize.");
}
// Otherwise, write all the changes included in the response 
// to the console. 
// For the initial synchronization, all the changes will be of type
// ChangeType.Create.
else
{
    foreach (FolderChange fc in fcc)
    {
        Console.WriteLine("ChangeType: " + fc.ChangeType.ToString());
        Console.WriteLine("FolderId: " + fc.FolderId);
        Console.WriteLine("===========");
    }
}
// Save the sync state for use in future SyncFolderItems requests.
// The sync state is used by the server to determine what changes to report
// to the client.
string fSyncState = fcc.SyncState;

```

<span data-ttu-id="2fc86-120">После получения списка новых или измененных папок на сервере [Создайте или обновите папки на клиенте](how-to-synchronize-folders-by-using-ews-in-exchange.md#bk_nextsteps).</span><span class="sxs-lookup"><span data-stu-id="2fc86-120">After you retrieve the list of new or changed folders on the server, [create or update the folders on the client](how-to-synchronize-folders-by-using-ews-in-exchange.md#bk_nextsteps).</span></span>
  
## <a name="get-the-initial-list-of-folders-by-using-ews"></a><span data-ttu-id="2fc86-121">Получение исходного списка папок с помощью EWS</span><span class="sxs-lookup"><span data-stu-id="2fc86-121">Get the initial list of folders by using EWS</span></span>
<span data-ttu-id="2fc86-122"><a name="bk_cesyncewsrequest"> </a></span><span class="sxs-lookup"><span data-stu-id="2fc86-122"><a name="bk_cesyncewsrequest"> </a></span></span>

<span data-ttu-id="2fc86-123">В следующем примере показан XML-запрос для получения исходной иерархии папок с помощью операции [SyncFolderHierarchy](https://msdn.microsoft.com/library/b31916b1-bc6c-4451-a475-b7c5417f752d%28Office.15%29.aspx) .</span><span class="sxs-lookup"><span data-stu-id="2fc86-123">The following example shows an XML request to get the initial folder hierarchy by using the [SyncFolderHierarchy](https://msdn.microsoft.com/library/b31916b1-bc6c-4451-a475-b7c5417f752d%28Office.15%29.aspx) operation.</span></span> <span data-ttu-id="2fc86-124">Это также запрос XML, который управляемый API EWS отправляет при [получении списка исходных папок с помощью метода SyncFolderHierarchy](how-to-synchronize-folders-by-using-ews-in-exchange.md#bk_cesyncinitialewsma).</span><span class="sxs-lookup"><span data-stu-id="2fc86-124">This is also the XML request that the EWS Managed API sends when [retrieving the list of initial folders by using the SyncFolderHierarchy method](how-to-synchronize-folders-by-using-ews-in-exchange.md#bk_cesyncinitialewsma).</span></span> <span data-ttu-id="2fc86-125">Элемент [синкстате](https://msdn.microsoft.com/library/e5ebaae3-0f07-481d-ac67-d9687a3c7ac3%28Office.15%29.aspx) операции [SyncFolderHierarchy](https://msdn.microsoft.com/library/7f0de089-8876-47ec-a871-df118ceae75d%28Office.15%29.aspx) не включается, так как это начальная синхронизация.</span><span class="sxs-lookup"><span data-stu-id="2fc86-125">The [SyncState](https://msdn.microsoft.com/library/e5ebaae3-0f07-481d-ac67-d9687a3c7ac3%28Office.15%29.aspx) element of the [SyncFolderHierarchy](https://msdn.microsoft.com/library/7f0de089-8876-47ec-a871-df118ceae75d%28Office.15%29.aspx) operation is not included because this is the initial synchronization.</span></span> <span data-ttu-id="2fc86-126">В этом примере для элемента [басешапе](https://msdn.microsoft.com/library/42c04f3b-abaa-4197-a3d6-d21677ffb1c0%28Office.15%29.aspx) задается значение **идонли** для уменьшения числа вызовов к базе данных Exchange, что является [наилучшим вариантом синхронизации](mailbox-synchronization-and-ews-in-exchange.md#bk_bestpractices).</span><span class="sxs-lookup"><span data-stu-id="2fc86-126">This example sets the [BaseShape](https://msdn.microsoft.com/library/42c04f3b-abaa-4197-a3d6-d21677ffb1c0%28Office.15%29.aspx) element to **IdOnly** to reduce calls to the Exchange database, which is a [synchronization best practice](mailbox-synchronization-and-ews-in-exchange.md#bk_bestpractices).</span></span>
  
```XML
<?xml version="1.0" encoding="utf-8"?>
<soap:Envelope xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" 
                    xmlns:m="https://schemas.microsoft.com/exchange/services/2006/messages"
                    xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types"
                    xmlns:soap="https://schemas.xmlsoap.org/soap/envelope/">
  <soap:Header>
    <t:RequestServerVersion Version="Exchange2013" />
  </soap:Header>
  <soap:Body>
    <m:SyncFolderHierarchy>
      <m:FolderShape>
        <t:BaseShape>IdOnly</t:BaseShape>
      </m:FolderShape>
      <m:SyncFolderId>
        <t:DistinguishedFolderId Id="root" />
      </m:SyncFolderId>
    </m:SyncFolderHierarchy>
  </soap:Body>
</soap:Envelope>
```

<span data-ttu-id="2fc86-127">В следующем примере показан ответ XML, возвращенный сервером после обработки запроса операции [SyncFolderHierarchy](https://msdn.microsoft.com/library/b31916b1-bc6c-4451-a475-b7c5417f752d%28Office.15%29.aspx) .</span><span class="sxs-lookup"><span data-stu-id="2fc86-127">The following example shows the XML response that is returned by the server after it processes the [SyncFolderHierarchy](https://msdn.microsoft.com/library/b31916b1-bc6c-4451-a475-b7c5417f752d%28Office.15%29.aspx) operation request.</span></span> <span data-ttu-id="2fc86-128">Исходный ответ содержит элементы [CREATE](https://msdn.microsoft.com/library/6b463d0a-70e9-40c5-ade4-c7d9a5f36bc1%28Office.15%29.aspx) для всех папок, так как во время начальной синхронизации все папки считаются новыми.</span><span class="sxs-lookup"><span data-stu-id="2fc86-128">The initial response includes [Create](https://msdn.microsoft.com/library/6b463d0a-70e9-40c5-ade4-c7d9a5f36bc1%28Office.15%29.aspx) elements for all folders because all folders are considered new during an initial synchronization.</span></span> <span data-ttu-id="2fc86-129">Значения некоторых атрибутов и элементов были сокращены для удобочитаемости, а некоторые блоки элементов **создания** были удалены для краткости.</span><span class="sxs-lookup"><span data-stu-id="2fc86-129">The values of some attributes and elements have been shortened for readability, and some **Create** element blocks were removed for brevity.</span></span> 
  
```xml
<?xml version="1.0" encoding="utf-8"?>
<s:Envelope xmlns:s="https://schemas.xmlsoap.org/soap/envelope/">
  <s:Header>
    <h:ServerVersionInfo MajorVersion="15"
                         MinorVersion="0"
                         MajorBuildNumber="785"
                         MinorBuildNumber="6"
                         Version="V2_6"
                         xmlns:h="https://schemas.microsoft.com/exchange/services/2006/types"
                         xmlns="https://schemas.microsoft.com/exchange/services/2006/types"
                         xmlns:xsd="http://www.w3.org/2001/XMLSchema"
                         xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance"/>
  </s:Header>
  <s:Body xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance"
          xmlns:xsd="http://www.w3.org/2001/XMLSchema">
    <m:SyncFolderHierarchyResponse xmlns:m="https://schemas.microsoft.com/exchange/services/2006/messages"
                                   xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types">
      <m:ResponseMessages>
        <m:SyncFolderHierarchyResponseMessage ResponseClass="Success">
          <m:ResponseCode>NoError</m:ResponseCode>
          <m:SyncState>H4sIAA==</m:SyncState>
          <m:IncludesLastFolderInRange>true</m:IncludesLastFolderInRange>
          <m:Changes>
            <t:Create>
              <t:Folder>
                <t:FolderId Id="AAMkADM="
                            ChangeKey="AQAAABYA"/>
              </t:Folder>
            </t:Create>
            <t:Create>
              <t:Folder>
                <t:FolderId Id="AAMkADMzM="
                            ChangeKey="AQAAABY"/>
              </t:Folder>
            </t:Create>
            <t:Create>
              <t:Folder>
                <t:FolderId Id="AAMkAD/AAA="
                            ChangeKey="AQAAABYA"/>
              </t:Folder>
            </t:Create>
            <t:Create>
              <t:Folder>
                <t:FolderId Id="AAMkADBh="
                            ChangeKey="AQAAABYA"/>
              </t:Folder>
            </t:Create>
            ...
          </m:Changes>
        </m:SyncFolderHierarchyResponseMessage>
      </m:ResponseMessages>
    </m:SyncFolderHierarchyResponse>
  </s:Body>
</s:Envelope>
```

<span data-ttu-id="2fc86-130">После получения списка новых папок на сервере [Создайте папки на клиенте](how-to-synchronize-folders-by-using-ews-in-exchange.md#bk_nextsteps).</span><span class="sxs-lookup"><span data-stu-id="2fc86-130">After you retrieve the list of new folders on the server, [create the folders on the client](how-to-synchronize-folders-by-using-ews-in-exchange.md#bk_nextsteps).</span></span>
  
## <a name="get-the-changes-since-the-last-sync-by-using-ews"></a><span data-ttu-id="2fc86-131">Получение изменений с момента последней синхронизации с помощью EWS</span><span class="sxs-lookup"><span data-stu-id="2fc86-131">Get the changes since the last sync by using EWS</span></span>
<span data-ttu-id="2fc86-132"><a name="bk_cesyncrespews"> </a></span><span class="sxs-lookup"><span data-stu-id="2fc86-132"><a name="bk_cesyncrespews"> </a></span></span>

<span data-ttu-id="2fc86-133">В следующем примере показан XML-запрос для получения списка изменений в папках корневой папки с помощью операции [SyncFolderHierarchy](https://msdn.microsoft.com/library/b31916b1-bc6c-4451-a475-b7c5417f752d%28Office.15%29.aspx) .</span><span class="sxs-lookup"><span data-stu-id="2fc86-133">The following example shows the XML request to get the list of changes to folders in the root folder by using the [SyncFolderHierarchy](https://msdn.microsoft.com/library/b31916b1-bc6c-4451-a475-b7c5417f752d%28Office.15%29.aspx) operation.</span></span> <span data-ttu-id="2fc86-134">Это также запрос XML, который отправляет управляемый API EWS при [получении списка изменений в корневой папке](how-to-synchronize-folders-by-using-ews-in-exchange.md#bk_cesyncinitialewsma).</span><span class="sxs-lookup"><span data-stu-id="2fc86-134">This is also the XML request that the EWS Managed API sends when [retrieving the list of changes to the root folder](how-to-synchronize-folders-by-using-ews-in-exchange.md#bk_cesyncinitialewsma).</span></span> <span data-ttu-id="2fc86-135">В этом примере для элемента [синкстате](https://msdn.microsoft.com/library/e5ebaae3-0f07-481d-ac67-d9687a3c7ac3%28Office.15%29.aspx) задается значение, возвращенное в предыдущем ответе.</span><span class="sxs-lookup"><span data-stu-id="2fc86-135">This example sets the [SyncState](https://msdn.microsoft.com/library/e5ebaae3-0f07-481d-ac67-d9687a3c7ac3%28Office.15%29.aspx) element value to the value returned in the previous response.</span></span> <span data-ttu-id="2fc86-136">Для демонстрационных целей в этом примере для элемента [басешапе](https://msdn.microsoft.com/library/42c04f3b-abaa-4197-a3d6-d21677ffb1c0%28Office.15%29.aspx) задается значение **аллпропертиес** вместо **идонли** для отображения возвращаемых дополнительных свойств.</span><span class="sxs-lookup"><span data-stu-id="2fc86-136">And for demonstration purposes, this example sets the [BaseShape](https://msdn.microsoft.com/library/42c04f3b-abaa-4197-a3d6-d21677ffb1c0%28Office.15%29.aspx) element to **AllProperties** instead of **IdOnly** to show the additional properties returned.</span></span> <span data-ttu-id="2fc86-137">Задание элемента [басешапе](https://msdn.microsoft.com/library/42c04f3b-abaa-4197-a3d6-d21677ffb1c0%28Office.15%29.aspx) равным **идонли** является [наилучшим методом синхронизации](mailbox-synchronization-and-ews-in-exchange.md#bk_bestpractices).</span><span class="sxs-lookup"><span data-stu-id="2fc86-137">Setting the [BaseShape](https://msdn.microsoft.com/library/42c04f3b-abaa-4197-a3d6-d21677ffb1c0%28Office.15%29.aspx) element to **IdOnly** is a [synchronization best practice](mailbox-synchronization-and-ews-in-exchange.md#bk_bestpractices).</span></span> <span data-ttu-id="2fc86-138">Значение **синкстате** было сокращено для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="2fc86-138">The value of **SyncState** has been shortened for readability.</span></span> 
  
```XML
<?xml version="1.0" encoding="utf-8"?>
<soap:Envelope xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" 
                    xmlns:m="https://schemas.microsoft.com/exchange/services/2006/messages"
                    xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types"
                    xmlns:soap="https://schemas.xmlsoap.org/soap/envelope/">
  <soap:Header>
    <t:RequestServerVersion Version="Exchange2013" />
  </soap:Header>
  <soap:Body>
    <m:SyncFolderHierarchy>
      <m:FolderShape>
        <t:BaseShape>AllProperties</t:BaseShape>
      </m:FolderShape>
      <m:SyncFolderId>
        <t:DistinguishedFolderId Id="root" />
      </m:SyncFolderId>
      <m:SyncState>H4sIAA==</m:SyncState>
    </m:SyncFolderHierarchy>
  </soap:Body>
</soap:Envelope>
```

<span data-ttu-id="2fc86-139">В следующем примере показан ответ XML, возвращенный сервером после обработки запроса [операции SyncFolderHierarchy](https://msdn.microsoft.com/library/b31916b1-bc6c-4451-a475-b7c5417f752d%28Office.15%29.aspx) от клиента.</span><span class="sxs-lookup"><span data-stu-id="2fc86-139">The following example shows the XML response that is returned by the server after it processes the [SyncFolderHierarchy operation](https://msdn.microsoft.com/library/b31916b1-bc6c-4451-a475-b7c5417f752d%28Office.15%29.aspx) request from the client.</span></span> <span data-ttu-id="2fc86-140">Этот ответ указывает на то, что одна папка была обновлена, была создана одна папка и удалена одна папка с момента предыдущей синхронизации.</span><span class="sxs-lookup"><span data-stu-id="2fc86-140">This response indicates that one folder was updated, one folder was created, and one folder was deleted since the prior synchronization.</span></span> <span data-ttu-id="2fc86-141">Значение элемента [синкстате](https://msdn.microsoft.com/library/e5ebaae3-0f07-481d-ac67-d9687a3c7ac3%28Office.15%29.aspx) , атрибуты **ID** и атрибуты **чанжекэй** были сокращены для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="2fc86-141">The value of the [SyncState](https://msdn.microsoft.com/library/e5ebaae3-0f07-481d-ac67-d9687a3c7ac3%28Office.15%29.aspx) element, **Id** attributes, and **ChangeKey** attributes have been shortened for readability.</span></span> 
  
<span data-ttu-id="2fc86-142">Помните, что запрос включал в себя **аллпропертиес**[басешапе](https://msdn.microsoft.com/library/42c04f3b-abaa-4197-a3d6-d21677ffb1c0%28Office.15%29.aspx).</span><span class="sxs-lookup"><span data-stu-id="2fc86-142">Remember that the request included the **AllProperties**[BaseShape](https://msdn.microsoft.com/library/42c04f3b-abaa-4197-a3d6-d21677ffb1c0%28Office.15%29.aspx).</span></span> <span data-ttu-id="2fc86-143">Это только для демонстрационных целей.</span><span class="sxs-lookup"><span data-stu-id="2fc86-143">This is just for demonstration purposes.</span></span> <span data-ttu-id="2fc86-144">Рекомендуется присвоить элементу **басешапе** значение **идонли** в рабочей среде.</span><span class="sxs-lookup"><span data-stu-id="2fc86-144">We recommend that you set the **BaseShape** element to **IdOnly** in production.</span></span> 
  
```XML
<?xml version="1.0" encoding="utf-8"?>
<s:Envelope xmlns:s="https://schemas.xmlsoap.org/soap/envelope/">
  <s:Header>
<h:ServerVersionInfo MajorVersion="15" MinorVersion="0" MajorBuildNumber="745" MinorBuildNumber="21" Version="V2_3" 
           xmlns:h="https://schemas.microsoft.com/exchange/services/2006/types" 
           xmlns="https://schemas.microsoft.com/exchange/services/2006/types" 
           xmlns:xsd="http://www.w3.org/2001/XMLSchema" 
           xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" />
  </s:Header>
  <s:Body xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" xmlns:xsd="http://www.w3.org/2001/XMLSchema">
    <m:SyncFolderHierarchyResponse xmlns:m="https://schemas.microsoft.com/exchange/services/2006/messages" 
            xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types">
      <m:ResponseMessages>
        <m:SyncFolderHierarchyResponseMessage ResponseClass="Success">
          <m:ResponseCode>NoError</m:ResponseCode>
          <m:SyncState>H4sIAAA</m:SyncState>
          <m:IncludesLastFolderInRange>true</m:IncludesLastFolderInRange>
          <m:Changes>
            <t:Update>
              <t:Folder>
                <t:FolderId Id="AAMkADM=" ChangeKey="AQAAABY" />
                <t:ParentFolderId Id="AQMkADMzADI1==" ChangeKey="AQAAAA==" />
                <t:FolderClass>IPF.Note</t:FolderClass>
                <t:DisplayName>Meeting Notes</t:DisplayName>
                <t:TotalCount>3</t:TotalCount>
                <t:ChildFolderCount>0</t:ChildFolderCount>
                <t:EffectiveRights>
                  <t:CreateAssociated>true</t:CreateAssociated>
                  <t:CreateContents>true</t:CreateContents>
                  <t:CreateHierarchy>true</t:CreateHierarchy>
                  <t:Delete>true</t:Delete>
                  <t:Modify>true</t:Modify>
                  <t:Read>true</t:Read>
                  <t:ViewPrivateItems>true</t:ViewPrivateItems>
                </t:EffectiveRights>
                <t:UnreadCount>0</t:UnreadCount>
              </t:Folder>
            </t:Update>
            <t:Create>
              <t:Folder>
                <t:FolderId Id="AAMkADMzM=" ChangeKey="AQAAABYAA" />
                <t:ParentFolderId Id="AQMkO67A==" ChangeKey="AQAAAA==" />
                <t:FolderClass>IPF.Note</t:FolderClass>
                <t:DisplayName>Schedules</t:DisplayName>
                <t:TotalCount>0</t:TotalCount>
                <t:ChildFolderCount>0</t:ChildFolderCount>
                <t:EffectiveRights>
                  <t:CreateAssociated>true</t:CreateAssociated>
                  <t:CreateContents>true</t:CreateContents>
                  <t:CreateHierarchy>true</t:CreateHierarchy>
                  <t:Delete>true</t:Delete>
                  <t:Modify>true</t:Modify>
                  <t:Read>true</t:Read>
                  <t:ViewPrivateItems>true</t:ViewPrivateItems>
                </t:EffectiveRights>
                <t:UnreadCount>0</t:UnreadCount>
              </t:Folder>
            </t:Create>
            <t:Delete>
              <t:FolderId Id="AAMkAD/AAA=" ChangeKey="AQAAAA==" />
            </t:Delete>
          </m:Changes>
        </m:SyncFolderHierarchyResponseMessage>
      </m:ResponseMessages>
    </m:SyncFolderHierarchyResponse>
  </s:Body>
</s:Envelope>

```

## <a name="update-the-client"></a><span data-ttu-id="2fc86-145">Обновление клиента</span><span class="sxs-lookup"><span data-stu-id="2fc86-145">Update the client</span></span>
<span data-ttu-id="2fc86-146"><a name="bk_nextsteps"> </a></span><span class="sxs-lookup"><span data-stu-id="2fc86-146"><a name="bk_nextsteps"> </a></span></span>

<span data-ttu-id="2fc86-147">Если вы используете управляемый API EWS, после получения списка новых или измененных папок используйте метод [Folder. Load](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.folder.load%28v=exchg.80%29.aspx) для получения свойств новых или измененных элементов, сравнения свойств с локальными значениями, а также для обновления или создания папок на клиенте.</span><span class="sxs-lookup"><span data-stu-id="2fc86-147">If you're using the EWS Managed API, after you get the list of new or changed folders, use the [Folder.Load](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.folder.load%28v=exchg.80%29.aspx) method to get properties on the new or changed items, compare the properties to the local values, and update or create the folders on the client.</span></span> 
  
<span data-ttu-id="2fc86-148">Если вы используете EWS, используйте операцию " [операция с папкой](https://msdn.microsoft.com/library/355bcf93-dc71-4493-b177-622afac5fdb9%28Office.15%29.aspx) " для получения свойств новых или измененных папок и обновления или создания папок на клиенте.</span><span class="sxs-lookup"><span data-stu-id="2fc86-148">If you're using EWS, use the [GetFolder operation](https://msdn.microsoft.com/library/355bcf93-dc71-4493-b177-622afac5fdb9%28Office.15%29.aspx) to get properties on the new or changed folders and update or create the folders on the client.</span></span> 
  
## <a name="see-also"></a><span data-ttu-id="2fc86-149">См. также</span><span class="sxs-lookup"><span data-stu-id="2fc86-149">See also</span></span>

- [<span data-ttu-id="2fc86-150">Синхронизация почтового ящика и веб-службах Exchange</span><span class="sxs-lookup"><span data-stu-id="2fc86-150">Mailbox synchronization and EWS in Exchange</span></span>](mailbox-synchronization-and-ews-in-exchange.md)   
- [<span data-ttu-id="2fc86-151">Синхронизация элементов с помощью EWS в Exchange</span><span class="sxs-lookup"><span data-stu-id="2fc86-151">Synchronize items by using EWS in Exchange</span></span>](how-to-synchronize-items-by-using-ews-in-exchange.md)   
- [<span data-ttu-id="2fc86-152">Обработка ошибок, связанных с синхронизацией, в EWS в Exchange</span><span class="sxs-lookup"><span data-stu-id="2fc86-152">Handling synchronization-related errors in EWS in Exchange</span></span>](handling-synchronization-related-errors-in-ews-in-exchange.md)
    

