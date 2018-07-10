---
title: Синхронизация папок с помощью веб-служб Exchange в Exchange
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
localization_priority: Normal
ms.assetid: d3bbacd1-8e4b-4fd0-8d27-4cbbc045ec3f
description: Узнайте, как использовать управляемый API EWS или веб-служб Exchange, чтобы получить список папок или список папок, которые были изменены, чтобы синхронизировать вашего клиента.
ms.openlocfilehash: 4b0686134d642da34b2890a0e692e3d03e4a9fb1
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/25/2018
ms.locfileid: "19761124"
---
# <a name="synchronize-folders-by-using-ews-in-exchange"></a><span data-ttu-id="ac35b-103">Синхронизация папок с помощью веб-служб Exchange в Exchange</span><span class="sxs-lookup"><span data-stu-id="ac35b-103">Synchronize folders by using EWS in Exchange</span></span>

<span data-ttu-id="ac35b-104">Узнайте, как использовать управляемый API EWS или веб-служб Exchange, чтобы получить список папок или список папок, которые были изменены, чтобы синхронизировать вашего клиента.</span><span class="sxs-lookup"><span data-stu-id="ac35b-104">Find out how to use the EWS Managed API or EWS to get a list of folders, or a list of folders that have changed, in order to synchronize your client.</span></span>
  
<span data-ttu-id="ac35b-105">ВЕБ-службах Exchange с помощью синхронизации элемента и синхронизации папок для содержимого почтового ящика синхронизации между клиентом и сервером.</span><span class="sxs-lookup"><span data-stu-id="ac35b-105">EWS in Exchange uses item synchronization and folder synchronization to sync mailbox content between the client and server.</span></span> <span data-ttu-id="ac35b-106">Синхронизации папки Получает исходный список папок из корневой папки и затем постепенно, получает изменения, внесенные в эти папки и возвращает также новые папки.</span><span class="sxs-lookup"><span data-stu-id="ac35b-106">Folder synchronization gets the initial list of folders from a root folder and then, over time, gets changes that were made to those folders and gets new folders as well.</span></span>
  
<span data-ttu-id="ac35b-107">При выполнении синхронизации папок с помощью управляемого API EWS, вы первый [получить исходный список папок, расположенных в корневую папку](how-to-synchronize-folders-by-using-ews-in-exchange.md#bk_cesyncinitialewsma) с помощью метода [ExchangeService.SyncFolderHierarchy](http://msdn.microsoft.com/ru-ru/library/microsoft.exchange.webservices.data.exchangeservice.syncfolderhierarchy%28v=exchg.80%29.aspx) .</span><span class="sxs-lookup"><span data-stu-id="ac35b-107">If you're performing folder synchronization by using the EWS Managed API, you first [get the initial list of folders in the root folder](how-to-synchronize-folders-by-using-ews-in-exchange.md#bk_cesyncinitialewsma) by using the [ExchangeService.SyncFolderHierarchy](http://msdn.microsoft.com/ru-ru/library/microsoft.exchange.webservices.data.exchangeservice.syncfolderhierarchy%28v=exchg.80%29.aspx) method.</span></span> <span data-ttu-id="ac35b-108">Затем обновите значение параметра _cSyncState_ во время последующих вызовов, чтобы получить список папок, новые и измененные.</span><span class="sxs-lookup"><span data-stu-id="ac35b-108">You then update the value of the  _cSyncState_ parameter during subsequent calls to get the list of new and changed folders.</span></span> 
  
<span data-ttu-id="ac35b-109">Для выполнения синхронизации папки с помощью веб-служб Exchange, запрос [исходный список папок, расположенных в корневую папку](how-to-synchronize-folders-by-using-ews-in-exchange.md#bk_cesyncewsrequest) с помощью операции [SyncFolderHierarchy](http://msdn.microsoft.com/library/b31916b1-bc6c-4451-a475-b7c5417f752d%28Office.15%29.aspx) , проанализировать ответ и к определенному моменту в будущем [внесения изменений в папки в корневой](how-to-synchronize-folders-by-using-ews-in-exchange.md#bk_cesyncrespews)и разбор ответа.</span><span class="sxs-lookup"><span data-stu-id="ac35b-109">To perform folder synchronization by using EWS, you request the [initial list of folders in the root folder](how-to-synchronize-folders-by-using-ews-in-exchange.md#bk_cesyncewsrequest) by using the [SyncFolderHierarchy](http://msdn.microsoft.com/library/b31916b1-bc6c-4451-a475-b7c5417f752d%28Office.15%29.aspx) operation, parse the response, and then at some point in the future [get the changes to the folders in the root](how-to-synchronize-folders-by-using-ews-in-exchange.md#bk_cesyncrespews), and parse the response.</span></span> <span data-ttu-id="ac35b-110">После получения список папок, начальной или измененные, оно [делает обновления локально](how-to-synchronize-folders-by-using-ews-in-exchange.md#bk_nextsteps).</span><span class="sxs-lookup"><span data-stu-id="ac35b-110">After the client receives the list of initial or changed folders, it [makes updates locally](how-to-synchronize-folders-by-using-ews-in-exchange.md#bk_nextsteps).</span></span> <span data-ttu-id="ac35b-111">Как и когда в будущем извлечения изменений, зависит от [шаблона разработки синхронизации](mailbox-synchronization-and-ews-in-exchange.md#bk_syncpatterns) с помощью приложения.</span><span class="sxs-lookup"><span data-stu-id="ac35b-111">How and when you retrieve changes in the future depends on the [synchronization design pattern](mailbox-synchronization-and-ews-in-exchange.md#bk_syncpatterns) your application is using.</span></span> 
  
## <a name="get-the-list-of-all-folders-or-changed-folders-by-using-the-ews-managed-api"></a><span data-ttu-id="ac35b-112">Получение списка всех папок и папок, измененные с помощью управляемого интерфейса API веб-служб Exchange</span><span class="sxs-lookup"><span data-stu-id="ac35b-112">Get the list of all folders or changed folders by using the EWS Managed API</span></span>
<span data-ttu-id="ac35b-113"><a name="bk_cesyncinitialewsma"> </a></span><span class="sxs-lookup"><span data-stu-id="ac35b-113"></span></span>

<span data-ttu-id="ac35b-114">В следующем примере кода показано, как получить исходный список папок, расположенных в корневую папку и затем получите список изменений в папки в корневой папке, произошедшие с момента предыдущей синхронизации.</span><span class="sxs-lookup"><span data-stu-id="ac35b-114">The following code example shows how to get an initial list of folders in a root folder and then get a list of changes to folders in the root folder that have occurred since the previous synchronization.</span></span> <span data-ttu-id="ac35b-115">Во время первого вызова метода [ExchangeService.SyncFolderHierarchy](http://msdn.microsoft.com/ru-ru/library/microsoft.exchange.webservices.data.exchangeservice.syncfolderhierarchy%28v=exchg.80%29.aspx) задайте значение _cSyncState_ значения NULL.</span><span class="sxs-lookup"><span data-stu-id="ac35b-115">During the initial call to the [ExchangeService.SyncFolderHierarchy](http://msdn.microsoft.com/ru-ru/library/microsoft.exchange.webservices.data.exchangeservice.syncfolderhierarchy%28v=exchg.80%29.aspx) method, set the  _cSyncState_ value to null.</span></span> <span data-ttu-id="ac35b-116">После завершения работы метода, сохраните значение _cSyncState_ локально для использования в следующем вызове метода **SyncFolderHierarchy** .</span><span class="sxs-lookup"><span data-stu-id="ac35b-116">When the method completes, save the  _cSyncState_ value locally to use in the next **SyncFolderHierarchy** method call.</span></span> <span data-ttu-id="ac35b-117">В первого вызова и последующих вызовов папок извлекаются в пакетах десять, с помощью успешные вызовы метода **SyncFolderHierarchy** , пока остаются больше нет изменений.</span><span class="sxs-lookup"><span data-stu-id="ac35b-117">In both the initial call and the subsequent calls, the folders are retrieved in batches of ten, by using successive calls to the **SyncFolderHierarchy** method, until no more changes remain.</span></span> <span data-ttu-id="ac35b-118">В этом примере задается параметр _propertySet_ IdOnly для уменьшения обращений к базе данных Exchange, который является [Рекомендация синхронизации](mailbox-synchronization-and-ews-in-exchange.md#bk_bestpractices).</span><span class="sxs-lookup"><span data-stu-id="ac35b-118">This example sets the  _propertySet_ parameter to IdOnly to reduce calls to the Exchange database, which is a [synchronization best practice](mailbox-synchronization-and-ews-in-exchange.md#bk_bestpractices).</span></span> <span data-ttu-id="ac35b-119">В этом примере предполагается, что **Служба** — допустимый объект привязки **ExchangeService** и _cSyncState_ , представляющий состояние синхронизации, возвращаемые предыдущего вызова **SyncFolderHierarchy**.</span><span class="sxs-lookup"><span data-stu-id="ac35b-119">In this example, we assume that **service** is a valid **ExchangeService** object binding and that  _cSyncState_ represents the sync state that was returned by a prior call to **SyncFolderHierarchy**.</span></span> 
  
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

<span data-ttu-id="ac35b-120">После можно получить список новые или измененные папок на сервере, [Создайте или обновите папок на стороне клиента](how-to-synchronize-folders-by-using-ews-in-exchange.md#bk_nextsteps).</span><span class="sxs-lookup"><span data-stu-id="ac35b-120">After you retrieve the list of new or changed folders on the server, [create or update the folders on the client](how-to-synchronize-folders-by-using-ews-in-exchange.md#bk_nextsteps).</span></span>
  
## <a name="get-the-initial-list-of-folders-by-using-ews"></a><span data-ttu-id="ac35b-121">Получение исходный список папок с помощью веб-служб Exchange</span><span class="sxs-lookup"><span data-stu-id="ac35b-121">Get the initial list of folders by using EWS</span></span>
<span data-ttu-id="ac35b-122"><a name="bk_cesyncewsrequest"> </a></span><span class="sxs-lookup"><span data-stu-id="ac35b-122"></span></span>

<span data-ttu-id="ac35b-123">В следующем примере показано XML-запрос для получения иерархии начальной папки с помощью операции [SyncFolderHierarchy](http://msdn.microsoft.com/library/b31916b1-bc6c-4451-a475-b7c5417f752d%28Office.15%29.aspx) .</span><span class="sxs-lookup"><span data-stu-id="ac35b-123">The following example shows an XML request to get the initial folder hierarchy by using the [SyncFolderHierarchy](http://msdn.microsoft.com/library/b31916b1-bc6c-4451-a475-b7c5417f752d%28Office.15%29.aspx) operation.</span></span> <span data-ttu-id="ac35b-124">Это также запроса XML, что управляемый API EWS отправляет при [получении списка начальной папки с помощью метода SyncFolderHierarchy](how-to-synchronize-folders-by-using-ews-in-exchange.md#bk_cesyncinitialewsma).</span><span class="sxs-lookup"><span data-stu-id="ac35b-124">This is also the XML request that the EWS Managed API sends when [retrieving the list of initial folders by using the SyncFolderHierarchy method](how-to-synchronize-folders-by-using-ews-in-exchange.md#bk_cesyncinitialewsma).</span></span> <span data-ttu-id="ac35b-125">Элемент [состояние](http://msdn.microsoft.com/library/e5ebaae3-0f07-481d-ac67-d9687a3c7ac3%28Office.15%29.aspx) операции [SyncFolderHierarchy](http://msdn.microsoft.com/library/7f0de089-8876-47ec-a871-df118ceae75d%28Office.15%29.aspx) не включена, так как это начальная синхронизация.</span><span class="sxs-lookup"><span data-stu-id="ac35b-125">The [SyncState](http://msdn.microsoft.com/library/e5ebaae3-0f07-481d-ac67-d9687a3c7ac3%28Office.15%29.aspx) element of the [SyncFolderHierarchy](http://msdn.microsoft.com/library/7f0de089-8876-47ec-a871-df118ceae75d%28Office.15%29.aspx) operation is not included because this is the initial synchronization.</span></span> <span data-ttu-id="ac35b-126">В этом примере задается элемент [BaseShape](http://msdn.microsoft.com/library/42c04f3b-abaa-4197-a3d6-d21677ffb1c0%28Office.15%29.aspx) **IdOnly** для уменьшения обращений к базе данных Exchange, который является [Рекомендация синхронизации](mailbox-synchronization-and-ews-in-exchange.md#bk_bestpractices).</span><span class="sxs-lookup"><span data-stu-id="ac35b-126">This example sets the [BaseShape](http://msdn.microsoft.com/library/42c04f3b-abaa-4197-a3d6-d21677ffb1c0%28Office.15%29.aspx) element to **IdOnly** to reduce calls to the Exchange database, which is a [synchronization best practice](mailbox-synchronization-and-ews-in-exchange.md#bk_bestpractices).</span></span>
  
```XML
<?xml version="1.0" encoding="utf-8"?>
<soap:Envelope xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" 
                    xmlns:m="http://schemas.microsoft.com/exchange/services/2006/messages"
                    xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types"
                    xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/">
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

<span data-ttu-id="ac35b-127">В следующем примере показано XML-ответ, возвращенный сервером, после обработки запроса операции [SyncFolderHierarchy](http://msdn.microsoft.com/library/b31916b1-bc6c-4451-a475-b7c5417f752d%28Office.15%29.aspx) .</span><span class="sxs-lookup"><span data-stu-id="ac35b-127">The following example shows the XML response that is returned by the server after it processes the [SyncFolderHierarchy](http://msdn.microsoft.com/library/b31916b1-bc6c-4451-a475-b7c5417f752d%28Office.15%29.aspx) operation request.</span></span> <span data-ttu-id="ac35b-128">Первоначального отклика включает [Создать](http://msdn.microsoft.com/library/6b463d0a-70e9-40c5-ade4-c7d9a5f36bc1%28Office.15%29.aspx) элементы для всех папок, так как все папках считаются new во время начальной синхронизации.</span><span class="sxs-lookup"><span data-stu-id="ac35b-128">The initial response includes [Create](http://msdn.microsoft.com/library/6b463d0a-70e9-40c5-ade4-c7d9a5f36bc1%28Office.15%29.aspx) elements for all folders because all folders are considered new during an initial synchronization.</span></span> <span data-ttu-id="ac35b-129">Значения некоторые атрибуты и элементы URL были сокращены для удобства чтения и некоторые блоки **Создать** элемент были удалены для краткости.</span><span class="sxs-lookup"><span data-stu-id="ac35b-129">The values of some attributes and elements have been shortened for readability, and some **Create** element blocks were removed for brevity.</span></span> 
  
```xml
<?xml version="1.0" encoding="utf-8"?>
<s:Envelope xmlns:s="http://schemas.xmlsoap.org/soap/envelope/">
  <s:Header>
    <h:ServerVersionInfo MajorVersion="15"
                         MinorVersion="0"
                         MajorBuildNumber="785"
                         MinorBuildNumber="6"
                         Version="V2_6"
                         xmlns:h="http://schemas.microsoft.com/exchange/services/2006/types"
                         xmlns="http://schemas.microsoft.com/exchange/services/2006/types"
                         xmlns:xsd="http://www.w3.org/2001/XMLSchema"
                         xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance"/>
  </s:Header>
  <s:Body xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance"
          xmlns:xsd="http://www.w3.org/2001/XMLSchema">
    <m:SyncFolderHierarchyResponse xmlns:m="http://schemas.microsoft.com/exchange/services/2006/messages"
                                   xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types">
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

<span data-ttu-id="ac35b-130">После можно извлечь список новые папки на сервере, [Создайте папки на стороне клиента](how-to-synchronize-folders-by-using-ews-in-exchange.md#bk_nextsteps).</span><span class="sxs-lookup"><span data-stu-id="ac35b-130">After you retrieve the list of new folders on the server, [create the folders on the client](how-to-synchronize-folders-by-using-ews-in-exchange.md#bk_nextsteps).</span></span>
  
## <a name="get-the-changes-since-the-last-sync-by-using-ews"></a><span data-ttu-id="ac35b-131">Получение изменений с момента последней синхронизации с помощью веб-служб Exchange</span><span class="sxs-lookup"><span data-stu-id="ac35b-131">Get the changes since the last sync by using EWS</span></span>
<span data-ttu-id="ac35b-132"><a name="bk_cesyncrespews"> </a></span><span class="sxs-lookup"><span data-stu-id="ac35b-132"></span></span>

<span data-ttu-id="ac35b-133">В следующем примере показано запроса XML для получения списка изменения папки в корневую папку с помощью операции [SyncFolderHierarchy](http://msdn.microsoft.com/library/b31916b1-bc6c-4451-a475-b7c5417f752d%28Office.15%29.aspx) .</span><span class="sxs-lookup"><span data-stu-id="ac35b-133">The following example shows the XML request to get the list of changes to folders in the root folder by using the [SyncFolderHierarchy](http://msdn.microsoft.com/library/b31916b1-bc6c-4451-a475-b7c5417f752d%28Office.15%29.aspx) operation.</span></span> <span data-ttu-id="ac35b-134">Это также запроса XML, что управляемый API EWS отправляет при [получении списка изменений в корневую папку](how-to-synchronize-folders-by-using-ews-in-exchange.md#bk_cesyncinitialewsma).</span><span class="sxs-lookup"><span data-stu-id="ac35b-134">This is also the XML request that the EWS Managed API sends when [retrieving the list of changes to the root folder](how-to-synchronize-folders-by-using-ews-in-exchange.md#bk_cesyncinitialewsma).</span></span> <span data-ttu-id="ac35b-135">В этом примере задается значение элемента [состояние](http://msdn.microsoft.com/library/e5ebaae3-0f07-481d-ac67-d9687a3c7ac3%28Office.15%29.aspx) значению, возвращенному в предыдущем ответе.</span><span class="sxs-lookup"><span data-stu-id="ac35b-135">This example sets the [SyncState](http://msdn.microsoft.com/library/e5ebaae3-0f07-481d-ac67-d9687a3c7ac3%28Office.15%29.aspx) element value to the value returned in the previous response.</span></span> <span data-ttu-id="ac35b-136">И в целях демонстрации в этом примере задается элемент [BaseShape](http://msdn.microsoft.com/library/42c04f3b-abaa-4197-a3d6-d21677ffb1c0%28Office.15%29.aspx) **AllProperties** вместо **IdOnly** для отображения возвращаемые дополнительные свойства.</span><span class="sxs-lookup"><span data-stu-id="ac35b-136">And for demonstration purposes, this example sets the [BaseShape](http://msdn.microsoft.com/library/42c04f3b-abaa-4197-a3d6-d21677ffb1c0%28Office.15%29.aspx) element to **AllProperties** instead of **IdOnly** to show the additional properties returned.</span></span> <span data-ttu-id="ac35b-137">Установка для элемента [BaseShape](http://msdn.microsoft.com/library/42c04f3b-abaa-4197-a3d6-d21677ffb1c0%28Office.15%29.aspx) **IdOnly** является [Рекомендация синхронизации](mailbox-synchronization-and-ews-in-exchange.md#bk_bestpractices).</span><span class="sxs-lookup"><span data-stu-id="ac35b-137">Setting the [BaseShape](http://msdn.microsoft.com/library/42c04f3b-abaa-4197-a3d6-d21677ffb1c0%28Office.15%29.aspx) element to **IdOnly** is a [synchronization best practice](mailbox-synchronization-and-ews-in-exchange.md#bk_bestpractices).</span></span> <span data-ttu-id="ac35b-138">Для удобства чтения был усечен значение **состояние** .</span><span class="sxs-lookup"><span data-stu-id="ac35b-138">The value of **SyncState** has been shortened for readability.</span></span> 
  
```XML
<?xml version="1.0" encoding="utf-8"?>
<soap:Envelope xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" 
                    xmlns:m="http://schemas.microsoft.com/exchange/services/2006/messages"
                    xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types"
                    xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/">
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

<span data-ttu-id="ac35b-139">В следующем примере показано XML-ответ, возвращенный сервером, после обработки запроса [операции SyncFolderHierarchy](http://msdn.microsoft.com/library/b31916b1-bc6c-4451-a475-b7c5417f752d%28Office.15%29.aspx) от клиента.</span><span class="sxs-lookup"><span data-stu-id="ac35b-139">The following example shows the XML response that is returned by the server after it processes the [SyncFolderHierarchy operation](http://msdn.microsoft.com/library/b31916b1-bc6c-4451-a475-b7c5417f752d%28Office.15%29.aspx) request from the client.</span></span> <span data-ttu-id="ac35b-140">Этот ответ указывает, что были добавлены в одной папке, один папка была создана и один папка была удалена с момента предыдущей синхронизации.</span><span class="sxs-lookup"><span data-stu-id="ac35b-140">This response indicates that one folder was updated, one folder was created, and one folder was deleted since the prior synchronization.</span></span> <span data-ttu-id="ac35b-141">Значение элемента [состояние](http://msdn.microsoft.com/library/e5ebaae3-0f07-481d-ac67-d9687a3c7ac3%28Office.15%29.aspx) , **идентификатор** атрибуты и атрибуты **ChangeKey** URL-были сокращены для удобства чтения.</span><span class="sxs-lookup"><span data-stu-id="ac35b-141">The value of the [SyncState](http://msdn.microsoft.com/library/e5ebaae3-0f07-481d-ac67-d9687a3c7ac3%28Office.15%29.aspx) element, **Id** attributes, and **ChangeKey** attributes have been shortened for readability.</span></span> 
  
<span data-ttu-id="ac35b-142">Имейте в виду, что запрос включены **AllProperties**[BaseShape](http://msdn.microsoft.com/library/42c04f3b-abaa-4197-a3d6-d21677ffb1c0%28Office.15%29.aspx).</span><span class="sxs-lookup"><span data-stu-id="ac35b-142">Remember that the request included the **AllProperties**[BaseShape](http://msdn.microsoft.com/library/42c04f3b-abaa-4197-a3d6-d21677ffb1c0%28Office.15%29.aspx).</span></span> <span data-ttu-id="ac35b-143">Это только в целях демонстрации.</span><span class="sxs-lookup"><span data-stu-id="ac35b-143">This is just for demonstration purposes.</span></span> <span data-ttu-id="ac35b-144">Рекомендуется устанавливать элемент **BaseShape** в **IdOnly** в рабочей среде.</span><span class="sxs-lookup"><span data-stu-id="ac35b-144">We recommend that you set the **BaseShape** element to **IdOnly** in production.</span></span> 
  
```XML
<?xml version="1.0" encoding="utf-8"?>
<s:Envelope xmlns:s="http://schemas.xmlsoap.org/soap/envelope/">
  <s:Header>
<h:ServerVersionInfo MajorVersion="15" MinorVersion="0" MajorBuildNumber="745" MinorBuildNumber="21" Version="V2_3" 
           xmlns:h="http://schemas.microsoft.com/exchange/services/2006/types" 
           xmlns="http://schemas.microsoft.com/exchange/services/2006/types" 
           xmlns:xsd="http://www.w3.org/2001/XMLSchema" 
           xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" />
  </s:Header>
  <s:Body xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" xmlns:xsd="http://www.w3.org/2001/XMLSchema">
    <m:SyncFolderHierarchyResponse xmlns:m="http://schemas.microsoft.com/exchange/services/2006/messages" 
            xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types">
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

## <a name="update-the-client"></a><span data-ttu-id="ac35b-145">Обновление клиента</span><span class="sxs-lookup"><span data-stu-id="ac35b-145">Update the client</span></span>
<span data-ttu-id="ac35b-146"><a name="bk_nextsteps"> </a></span><span class="sxs-lookup"><span data-stu-id="ac35b-146"></span></span>

<span data-ttu-id="ac35b-147">Если вы используете управляемый API веб-служб Exchange, после получить список папок, новые или измененные, используйте метод [Folder.Load](http://msdn.microsoft.com/ru-ru/library/microsoft.exchange.webservices.data.folder.load%28v=exchg.80%29.aspx) на получение свойств для новых и измененных элементов, сравните свойства в локальном значения и обновление или создание папок на стороне клиента.</span><span class="sxs-lookup"><span data-stu-id="ac35b-147">If you're using the EWS Managed API, after you get the list of new or changed folders, use the [Folder.Load](http://msdn.microsoft.com/ru-ru/library/microsoft.exchange.webservices.data.folder.load%28v=exchg.80%29.aspx) method to get properties on the new or changed items, compare the properties to the local values, and update or create the folders on the client.</span></span> 
  
<span data-ttu-id="ac35b-148">Если вы используете веб-служб Exchange, с помощью [операции GetFolder](http://msdn.microsoft.com/library/355bcf93-dc71-4493-b177-622afac5fdb9%28Office.15%29.aspx) для получения свойств папки новые или измененные и обновления или создания папки на стороне клиента.</span><span class="sxs-lookup"><span data-stu-id="ac35b-148">If you're using EWS, use the [GetFolder operation](http://msdn.microsoft.com/library/355bcf93-dc71-4493-b177-622afac5fdb9%28Office.15%29.aspx) to get properties on the new or changed folders and update or create the folders on the client.</span></span> 
  
## <a name="see-also"></a><span data-ttu-id="ac35b-149">См. также</span><span class="sxs-lookup"><span data-stu-id="ac35b-149">See also</span></span>

- [<span data-ttu-id="ac35b-150">Синхронизация почтового ящика и веб-службах Exchange</span><span class="sxs-lookup"><span data-stu-id="ac35b-150">Mailbox synchronization and EWS in Exchange</span></span>](mailbox-synchronization-and-ews-in-exchange.md)   
- [<span data-ttu-id="ac35b-151">Синхронизация элементов с помощью веб-служб Exchange в Exchange</span><span class="sxs-lookup"><span data-stu-id="ac35b-151">Synchronize items by using EWS in Exchange</span></span>](how-to-synchronize-items-by-using-ews-in-exchange.md)   
- [<span data-ttu-id="ac35b-152">Обработка ошибок, связанных с синхронизации в веб-служб Exchange в Exchange</span><span class="sxs-lookup"><span data-stu-id="ac35b-152">Handling synchronization-related errors in EWS in Exchange</span></span>](handling-synchronization-related-errors-in-ews-in-exchange.md)
    

