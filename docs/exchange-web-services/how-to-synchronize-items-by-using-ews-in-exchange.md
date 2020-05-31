---
title: Синхронизация элементов с помощью EWS в Exchange
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
localization_priority: Normal
ms.assetid: 886e7d35-9096-480b-8a8c-a7db27da06c2
description: Узнайте, как использовать управляемый API EWS или EWS для получения списка всех элементов в папке, или список изменений, произошедших в папке, для синхронизации клиента.
ms.openlocfilehash: 8763c053463e4787741ef992ddb99d29be4192fc
ms.sourcegitcommit: 9061fcf40c218ebe88911783f357b7df278846db
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/28/2018
ms.locfileid: "21353786"
---
# <a name="synchronize-items-by-using-ews-in-exchange"></a><span data-ttu-id="b2fba-103">Синхронизация элементов с помощью EWS в Exchange</span><span class="sxs-lookup"><span data-stu-id="b2fba-103">Synchronize items by using EWS in Exchange</span></span>

<span data-ttu-id="b2fba-104">Узнайте, как использовать управляемый API EWS или EWS для получения списка всех элементов в папке, или список изменений, произошедших в папке, для синхронизации клиента.</span><span class="sxs-lookup"><span data-stu-id="b2fba-104">Find out how to use the EWS Managed API or EWS to get a list of all items in a folder, or a list of changes that have occurred in a folder, in order to synchronize your client.</span></span>
  
<span data-ttu-id="b2fba-105">Служба EWS в Exchange использует синхронизацию элементов и синхронизацию папок для синхронизации содержимого почтовых ящиков между клиентом и сервером.</span><span class="sxs-lookup"><span data-stu-id="b2fba-105">EWS in Exchange uses item synchronization and folder synchronization to sync mailbox content between the client and server.</span></span> <span data-ttu-id="b2fba-106">Синхронизация элементов получает исходный список элементов в папке, а затем получает изменения, внесенные в эти элементы, а также получает новые элементы.</span><span class="sxs-lookup"><span data-stu-id="b2fba-106">Item synchronization gets the initial list of items in a folder and then, over time, gets changes that have been made to those items and gets new items as well.</span></span>
  
<span data-ttu-id="b2fba-107">Обратите внимание, что перед синхронизацией элементов с клиентом необходимо сначала [синхронизировать иерархию папок](how-to-synchronize-folders-by-using-ews-in-exchange.md).</span><span class="sxs-lookup"><span data-stu-id="b2fba-107">Note that before you can sync items to a client, you first have to [sync the folder hierarchy](how-to-synchronize-folders-by-using-ews-in-exchange.md).</span></span> <span data-ttu-id="b2fba-108">После того как иерархия папок будет размещена в клиенте, если вы выполняете синхронизацию элементов с помощью управляемого API EWS, сначала [получите исходный список элементов в папке "Входящие"](#bk_cesyncongoingewsma) с помощью метода [ExchangeService. SyncFolderItems](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.exchangeservice.syncfolderitems%28v=exchg.80%29.aspx) .</span><span class="sxs-lookup"><span data-stu-id="b2fba-108">After the folder hierarchy is in place on the client, if you're performing item synchronization by using the EWS Managed API, you first [get the initial list of items in the Inbox](#bk_cesyncongoingewsma) by using the [ExchangeService.SyncFolderItems](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.exchangeservice.syncfolderitems%28v=exchg.80%29.aspx) method.</span></span> <span data-ttu-id="b2fba-109">Затем необходимо обновить значение параметра _ксинкстате_ во время последующих вызовов, чтобы получить список измененных элементов в папке "Входящие".</span><span class="sxs-lookup"><span data-stu-id="b2fba-109">You then update the value of the  _cSyncState_ parameter during subsequent calls to get the list of changed items in the Inbox.</span></span> 
  
<span data-ttu-id="b2fba-110">Чтобы выполнить синхронизацию элементов с помощью EWS, после того как вы [синхронизируете иерархию папок](how-to-synchronize-folders-by-using-ews-in-exchange.md), вы запрашиваете [исходный список элементов в папке "Входящие"](#bk_ewsexamplea) с помощью [операции SyncFolderItems](http://msdn.microsoft.com/library/7f0de089-8876-47ec-a871-df118ceae75d%28Office.15%29.aspx), анализируете ответ, а затем в некоторый момент в будущем [получите изменения элементов в почтовом ящике](#bk_ewsexamplec)и проанализируйте ответ.</span><span class="sxs-lookup"><span data-stu-id="b2fba-110">To perform item synchronization by using EWS, after you [sync the folder hierarchy](how-to-synchronize-folders-by-using-ews-in-exchange.md), you request the [initial list of items in the Inbox](#bk_ewsexamplea) by using the [SyncFolderItems operation](http://msdn.microsoft.com/library/7f0de089-8876-47ec-a871-df118ceae75d%28Office.15%29.aspx), parse the response, and then at some point in the future [get the changes to the items in the mailbox](#bk_ewsexamplec), and parse the response.</span></span> <span data-ttu-id="b2fba-111">После того как клиент получит список начальных или измененных элементов, он [вносит обновления локально](#bk_nextsteps).</span><span class="sxs-lookup"><span data-stu-id="b2fba-111">After the client receives the list of initial or changed items, it [makes updates locally](#bk_nextsteps).</span></span> <span data-ttu-id="b2fba-112">Как и когда вы извлечете изменения в будущем, зависит от [шаблона проекта синхронизации](mailbox-synchronization-and-ews-in-exchange.md#bk_syncpatterns) , используемого приложением.</span><span class="sxs-lookup"><span data-stu-id="b2fba-112">How and when you retrieve changes in the future depends on the [synchronization design pattern](mailbox-synchronization-and-ews-in-exchange.md#bk_syncpatterns) your application is using.</span></span> 
  
## <a name="get-the-list-of-all-items-or-changed-items-by-using-the-ews-managed-api"></a><span data-ttu-id="b2fba-113">Получение списка всех элементов или измененных элементов с помощью управляемого API EWS</span><span class="sxs-lookup"><span data-stu-id="b2fba-113">Get the list of all items or changed items by using the EWS Managed API</span></span>
<span data-ttu-id="b2fba-114"><a name="bk_cesyncongoingewsma"> </a></span><span class="sxs-lookup"><span data-stu-id="b2fba-114"><a name="bk_cesyncongoingewsma"> </a></span></span>

<span data-ttu-id="b2fba-115">В приведенном ниже примере кода показано, как получить исходный список всех элементов в папке "Входящие", а затем получить список изменений элементов в папке "Входящие", произошедших с момента предыдущей синхронизации.</span><span class="sxs-lookup"><span data-stu-id="b2fba-115">The following code example shows how to get an initial list of all items in the Inbox folder and then get a list of changes to items in the Inbox folder that have occurred since the previous synchronization.</span></span> <span data-ttu-id="b2fba-116">Во время начального вызова метода [SyncFolderItems](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.exchangeservice.syncfolderitems%28v=exchg.80%29.aspx) задайте для параметра _ксинкстате_ значение null.</span><span class="sxs-lookup"><span data-stu-id="b2fba-116">During the initial call to the [SyncFolderItems](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.exchangeservice.syncfolderitems%28v=exchg.80%29.aspx) method, set the  _cSyncState_ value to null.</span></span> <span data-ttu-id="b2fba-117">После выполнения метода сохраните значение _ксинкстате_ локально, чтобы использовать его в следующем вызове метода **SyncFolderItems** .</span><span class="sxs-lookup"><span data-stu-id="b2fba-117">When the method completes, save the  _cSyncState_ value locally to use in the next **SyncFolderItems** method call.</span></span> <span data-ttu-id="b2fba-118">При первом вызове и последующих вызовах элементы извлекаются в пакетах десяти, с помощью последовательных вызовов метода **SyncFolderItems** , пока не будут сохранены другие изменения.</span><span class="sxs-lookup"><span data-stu-id="b2fba-118">In both the initial call and the subsequent calls, the items are retrieved in batches of ten, by using successive calls to the **SyncFolderItems** method, until no more changes remain.</span></span> 
  
<span data-ttu-id="b2fba-119">В этом примере параметру _Property_ присваивается значение идонли для уменьшения числа вызовов к базе данных Exchange, что является [наилучшим вариантом синхронизации](mailbox-synchronization-and-ews-in-exchange.md#bk_bestpractices).</span><span class="sxs-lookup"><span data-stu-id="b2fba-119">This example sets the  _propertySet_ parameter to IdOnly to reduce calls to the Exchange database, which is a [synchronization best practice](mailbox-synchronization-and-ews-in-exchange.md#bk_bestpractices).</span></span> <span data-ttu-id="b2fba-120">В этом примере предполагается, что **Служба** является допустимой привязкой объекта **ExchangeService** и _ксинкстате_ представляет состояние синхронизации, возвращенное предыдущим вызовом в **SyncFolderItems**.</span><span class="sxs-lookup"><span data-stu-id="b2fba-120">In this example, we assume that **service** is a valid **ExchangeService** object binding and that  _cSyncState_ represents the sync state that was returned by a prior call to **SyncFolderItems**.</span></span> 
  
```cs
// Track whether there are more items available for download on the server.
bool moreChangesAvailable = false;
do
{
    // Get a list of all items in the Inbox by calling SyncFolderHierarchy repeatedly until no more changes are available.
    // The folderId parameter must be set to the root folder to synchronize,
    // and must be same folder ID as used in previous synchronization calls. 
    // The propertySet parameter is set to IdOnly to reduce calls to the Exchange database,
    // because any additional properties result in additional calls to the Exchange database. 
    // The ignoredItemIds parameter is set to null, so that no items are ignored.
    // The maxChangesReturned parameter is set to return a maximum of 10 items (512 is the maximum).
    // The syncScope parameter is set to Normal items, so that associated items will not be returned.
    // The syncState parameter is set to cSyncState, which should be null in the initial call, 
    // and should be set to the sync state returned by the 
    // previous SyncFolderItems call in subsequent calls.
    ChangeCollection<ItemChange> icc = service.SyncFolderItems(new FolderId(WellKnownFolderName.Inbox), PropertySet.IdOnly, null, 10, SyncFolderItemsScope.NormalItems, cSyncState);
    // If the count of changes is zero, there are no changes to synchronize.
    if (icc.Count == 0)
    {
        Console.WriteLine("There are no item changes to synchronize.");
    }
    // Otherwise, write all the changes included in the response 
    // to the console. 
    else
    {
        foreach (ItemChange ic in icc)
        {
            Console.WriteLine("ChangeType: " + ic.ChangeType.ToString());
            Console.WriteLine("ItemId: " + ic.ItemId);
            Console.WriteLine("===========");
        }
    }
    // Save the sync state for use in future SyncFolderContent requests.
    // The sync state is used by the server to determine what changes to report
    // to the client.
    string sSyncState = icc.SyncState;
   // Determine whether more changes are available on the server.
   moreChangesAvailable = icc.MoreChangesAvailable;
}
while (moreChangesAvailable);

```

Метод **SyncFolderItems** аналогичен методу [FindItems](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.exchangeservice.finditems%28v=exchg.80%29.aspx) в том, что он не может возвращать свойства, такие как [текст](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.item.body%28v=exchg.80%29.aspx) или [вложения](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.item.attachments%28v=exchg.80%29.aspx). <span data-ttu-id="b2fba-122">Если требуются свойства, которые не могут быть возвращены методом **SyncFolderItems** , укажите свойство [идонли](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.propertyset.idonly%28v=exchg.80%29.aspx) , заданное при вызове **SyncFolderItems**, а затем используйте метод [ExchangeService. лоадпропертиесфоритемс](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.exchangeservice.loadpropertiesforitems%28v=exchg.80%29.aspx) для получения свойств, которые требуются для элементов, возвращенных методом **SyncFolderItems** .</span><span class="sxs-lookup"><span data-stu-id="b2fba-122">If you need properties that cannot be returned by the **SyncFolderItems** method, specify the [IdOnly](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.propertyset.idonly%28v=exchg.80%29.aspx) property set when you call **SyncFolderItems**, and then use the [ExchangeService.LoadPropertiesForItems](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.exchangeservice.loadpropertiesforitems%28v=exchg.80%29.aspx) method to get the properties you require for the items that were returned by the **SyncFolderItems** method.</span></span> 
  
<span data-ttu-id="b2fba-123">После получения списка новых или измененных элементов на сервере [Создайте или обновите элементы в клиенте](#bk_nextsteps).</span><span class="sxs-lookup"><span data-stu-id="b2fba-123">After you retrieve the list of new or changed items on the server, [create or update the items on the client](#bk_nextsteps).</span></span>
  
## <a name="get-the-initial-list-of-items-by-using-ews"></a><span data-ttu-id="b2fba-124">Получение исходного списка элементов с помощью EWS</span><span class="sxs-lookup"><span data-stu-id="b2fba-124">Get the initial list of items by using EWS</span></span>
<span data-ttu-id="b2fba-125"><a name="bk_ewsexamplea"> </a></span><span class="sxs-lookup"><span data-stu-id="b2fba-125"><a name="bk_ewsexamplea"> </a></span></span>

<span data-ttu-id="b2fba-126">В следующем примере показан XML-запрос для получения исходного списка элементов в папке "Входящие" с помощью [операции SyncFolderItems](http://msdn.microsoft.com/library/7f0de089-8876-47ec-a871-df118ceae75d%28Office.15%29.aspx).</span><span class="sxs-lookup"><span data-stu-id="b2fba-126">The following example shows the XML request to get the initial list of items in the Inbox by using the [SyncFolderItems operation](http://msdn.microsoft.com/library/7f0de089-8876-47ec-a871-df118ceae75d%28Office.15%29.aspx).</span></span> <span data-ttu-id="b2fba-127">Это также запрос XML, который управляемый API EWS отправляет при [получении списка элементов с помощью метода SyncFolderItems](#bk_cesyncongoingewsma).</span><span class="sxs-lookup"><span data-stu-id="b2fba-127">This is also the XML request that the EWS Managed API sends when [retrieving the list of items by using the SyncFolderItems method](#bk_cesyncongoingewsma).</span></span> <span data-ttu-id="b2fba-128">Элемент [синкстате](http://msdn.microsoft.com/library/e5ebaae3-0f07-481d-ac67-d9687a3c7ac3%28Office.15%29.aspx) операции **SyncFolderItems** не включается, так как это начальная синхронизация.</span><span class="sxs-lookup"><span data-stu-id="b2fba-128">The [SyncState](http://msdn.microsoft.com/library/e5ebaae3-0f07-481d-ac67-d9687a3c7ac3%28Office.15%29.aspx) element of the **SyncFolderItems** operation is not included because this is the initial synchronization.</span></span> <span data-ttu-id="b2fba-129">В этом примере для элемента [басешапе](http://msdn.microsoft.com/library/42c04f3b-abaa-4197-a3d6-d21677ffb1c0%28Office.15%29.aspx) задается значение **идонли** для уменьшения числа вызовов к базе данных Exchange, что является [наилучшим вариантом синхронизации](mailbox-synchronization-and-ews-in-exchange.md#bk_bestpractices).</span><span class="sxs-lookup"><span data-stu-id="b2fba-129">This example sets the [BaseShape](http://msdn.microsoft.com/library/42c04f3b-abaa-4197-a3d6-d21677ffb1c0%28Office.15%29.aspx) element to **IdOnly** to reduce calls to the Exchange database, which is a [synchronization best practice](mailbox-synchronization-and-ews-in-exchange.md#bk_bestpractices).</span></span>
  
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
    <m:SyncFolderItems>
      <m:ItemShape>
        <t:BaseShape>IdOnly</t:BaseShape>
      </m:ItemShape>
      <m:SyncFolderId>
        <t:DistinguishedFolderId Id="inbox" />
      </m:SyncFolderId>
      <m:MaxChangesReturned>10</m:MaxChangesReturned>
      <m:SyncScope>NormalItems</m:SyncScope>
    </m:SyncFolderItems>
  </soap:Body>
</soap:Envelope>
```

<span data-ttu-id="b2fba-130"><a name="bk_responsesyncfolderitems"> </a></span><span class="sxs-lookup"><span data-stu-id="b2fba-130"><a name="bk_responsesyncfolderitems"> </a></span></span>

<span data-ttu-id="b2fba-131">В следующем примере показан ответ XML, возвращенный сервером после обработки запроса операции **SyncFolderItems** от клиента.</span><span class="sxs-lookup"><span data-stu-id="b2fba-131">The following example shows the XML response that is returned by the server after it processes the **SyncFolderItems** operation request from the client.</span></span> <span data-ttu-id="b2fba-132">Исходный ответ включает элементы [CREATE](http://msdn.microsoft.com/library/cb5e64a2-66a5-4447-921e-7c13efb8f6bf%28Office.15%29.aspx) для пяти элементов, так как все элементы считаются новыми во время первоначальной синхронизации.</span><span class="sxs-lookup"><span data-stu-id="b2fba-132">The initial response includes [Create](http://msdn.microsoft.com/library/cb5e64a2-66a5-4447-921e-7c13efb8f6bf%28Office.15%29.aspx) elements for five items because all items are considered new during an initial synchronization.</span></span> <span data-ttu-id="b2fba-133">Для удобства значения некоторых атрибутов и элементов были сокращены.</span><span class="sxs-lookup"><span data-stu-id="b2fba-133">The values of some attributes and elements have been shortened for readability.</span></span> 
  
```XML
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
    <m:SyncFolderItemsResponse xmlns:m="http://schemas.microsoft.com/exchange/services/2006/messages"
                               xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types">
      <m:ResponseMessages>
        <m:SyncFolderItemsResponseMessage ResponseClass="Success">
          <m:ResponseCode>NoError</m:ResponseCode>
          <m:SyncState>H4sIAAA==</m:SyncState>
          <m:IncludesLastItemInRange>true</m:IncludesLastItemInRange>
          <m:Changes>
            <t:Create>
              <t:Message>
                <t:ItemId Id="q04QAAAA=="
                          ChangeKey="CQAAABYAAABhFfgM7MNwSYx0VZ0GoBMJAAAATVdC"/>
              </t:Message>
            </t:Create>
            <t:Create>
              <t:Message>
                <t:ItemId Id="q07AAAAA=="
                          ChangeKey="CQAAABYAAABhFfgM7MNwSYx0VZ0GoBMJAAAATVdB"/>
              </t:Message>
            </t:Create>
            <t:Create>
              <t:Message>
                <t:ItemId Id="q1AwAAAA=="
                          ChangeKey="CQAAABYAAABhFfgM7MNwSYx0VZ0GoBMJAAAATVdA"/>
              </t:Message>
            </t:Create>
            <t:Create>
              <t:Message>
                <t:ItemId Id="AAMkADBh=="
                          ChangeKey="CQAAABYAAABhFfgM7MNwSYx0VZ0GoBMJAAAATVc5"/>
              </t:Message>
            </t:Create>
            <t:Create>
              <t:Message>
                <t:ItemId Id="AAMkADBh=="
                          ChangeKey="CQAAABYAAABhFfgM7MNwSYx0VZ0GoBMJAAAATVc4"/>
              </t:Message>
            </t:Create>
          </m:Changes>
        </m:SyncFolderItemsResponseMessage>
      </m:ResponseMessages>
    </m:SyncFolderItemsResponse>
  </s:Body>
</s:Envelope>
```

<span data-ttu-id="b2fba-134">После получения списка новых элементов на сервере [Создайте элементы на клиенте](#bk_nextsteps).</span><span class="sxs-lookup"><span data-stu-id="b2fba-134">After you retrieve the list of new items on the server, [create the items on the client](#bk_nextsteps).</span></span>
  
## <a name="get-the-changes-since-the-last-sync-by-using-ews"></a><span data-ttu-id="b2fba-135">Получение изменений с момента последней синхронизации с помощью EWS</span><span class="sxs-lookup"><span data-stu-id="b2fba-135">Get the changes since the last sync by using EWS</span></span>
<span data-ttu-id="b2fba-136"><a name="bk_ewsexamplec"> </a></span><span class="sxs-lookup"><span data-stu-id="b2fba-136"><a name="bk_ewsexamplec"> </a></span></span>

<span data-ttu-id="b2fba-137">В следующем примере показан XML-запрос для получения списка изменений элементов в папке "Входящие" с помощью операции [SyncFolderItems](http://msdn.microsoft.com/library/7f0de089-8876-47ec-a871-df118ceae75d%28Office.15%29.aspx) .</span><span class="sxs-lookup"><span data-stu-id="b2fba-137">The following example shows the XML request to get the list of changes to items in the Inbox by using the [SyncFolderItems](http://msdn.microsoft.com/library/7f0de089-8876-47ec-a871-df118ceae75d%28Office.15%29.aspx) operation.</span></span> <span data-ttu-id="b2fba-138">Это также запрос XML, который отправляет управляемый API EWS при [получении списка изменений в папке "Входящие"](#bk_cesyncongoingewsma).</span><span class="sxs-lookup"><span data-stu-id="b2fba-138">This is also the XML request that the EWS Managed API sends when [retrieving the list of changes to the Inbox](#bk_cesyncongoingewsma).</span></span> <span data-ttu-id="b2fba-139">В этом примере для элемента [синкстате](http://msdn.microsoft.com/library/e5ebaae3-0f07-481d-ac67-d9687a3c7ac3%28Office.15%29.aspx) задается значение, возвращенное в [предыдущем ответе](#bk_responsesyncfolderitems).</span><span class="sxs-lookup"><span data-stu-id="b2fba-139">This example sets the [SyncState](http://msdn.microsoft.com/library/e5ebaae3-0f07-481d-ac67-d9687a3c7ac3%28Office.15%29.aspx) element value to the value returned in the [previous response](#bk_responsesyncfolderitems).</span></span> <span data-ttu-id="b2fba-140">Для демонстрационных целей в этом примере для элемента [басешапе](http://msdn.microsoft.com/library/42c04f3b-abaa-4197-a3d6-d21677ffb1c0%28Office.15%29.aspx) задается значение **аллпропертиес** вместо **идонли** для отображения возвращаемых дополнительных свойств.</span><span class="sxs-lookup"><span data-stu-id="b2fba-140">And for demonstration purposes, this example sets the [BaseShape](http://msdn.microsoft.com/library/42c04f3b-abaa-4197-a3d6-d21677ffb1c0%28Office.15%29.aspx) element to **AllProperties** instead of **IdOnly** to show the additional properties returned.</span></span> <span data-ttu-id="b2fba-141">Задание элемента [басешапе](http://msdn.microsoft.com/library/42c04f3b-abaa-4197-a3d6-d21677ffb1c0%28Office.15%29.aspx) равным **идонли** является [наилучшим методом синхронизации](mailbox-synchronization-and-ews-in-exchange.md#bk_bestpractices).</span><span class="sxs-lookup"><span data-stu-id="b2fba-141">Setting the [BaseShape](http://msdn.microsoft.com/library/42c04f3b-abaa-4197-a3d6-d21677ffb1c0%28Office.15%29.aspx) element to **IdOnly** is a [synchronization best practice](mailbox-synchronization-and-ews-in-exchange.md#bk_bestpractices).</span></span> <span data-ttu-id="b2fba-142">Значение **синкстате** было сокращено для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="b2fba-142">The value of **SyncState** has been shortened for readability.</span></span> 
  
```XML
<?xml version="1.0" encoding="utf-8"?>
<soap:Envelope xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" 
               xmlns:m="http://schemas.microsoft.com/exchange/services/2006/messages"
               xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types"
               xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/">
  <soap:Header>
      <t:RequestServerVersion Version="Exchange2010_SP2" />
  </soap:Header>
  <soap:Body>
    <m:SyncFolderItems>
      <m:ItemShape>
        <t:BaseShape>AllProperties</t:BaseShape>
      </m:ItemShape>
      <m:SyncFolderId>
        <t:DistinguishedFolderId Id="inbox" />
      </m:SyncFolderId>
      <m:SyncState>H4sIAAA==</m:SyncState>
      <m:MaxChangesReturned>10</m:MaxChangesReturned>
      <m:SyncScope>NormalItems</m:SyncScope>
    </m:SyncFolderItems>
  </soap:Body>
</soap:Envelope>
```

<span data-ttu-id="b2fba-143">В следующем примере показан ответ XML, возвращенный сервером после обработки запроса операции **SyncFolderItems** от клиента.</span><span class="sxs-lookup"><span data-stu-id="b2fba-143">The following example shows the XML response that is returned by the server after it processes the **SyncFolderItems** operation request from the client.</span></span> <span data-ttu-id="b2fba-144">Этот ответ указывает на то, что один элемент был обновлен, были созданы два элемента, был изменен флаг чтения одного элемента, и один элемент был удален с момента предыдущей синхронизации.</span><span class="sxs-lookup"><span data-stu-id="b2fba-144">This response indicates that one item was updated, two items were created, the read flag of one item was changed, and one item was deleted since the prior synchronization.</span></span> <span data-ttu-id="b2fba-145">Для удобства значения некоторых атрибутов и элементов были сокращены.</span><span class="sxs-lookup"><span data-stu-id="b2fba-145">The values of some attributes and elements have been shortened for readability.</span></span> 
  
```XML
<?xml version="1.0" encoding="utf-8"?>
<s:Envelope xmlns:s="http://schemas.xmlsoap.org/soap/envelope/">
  <s:Header>
    <h:ServerVersionInfo MajorVersion="15" MinorVersion="0" MajorBuildNumber="731" MinorBuildNumber="10" Version="V2_3"
                 xmlns:h="http://schemas.microsoft.com/exchange/services/2006/types"
                 xmlns="http://schemas.microsoft.com/exchange/services/2006/types"
                 xmlns:xsd="http://www.w3.org/2001/XMLSchema" 
                 xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" />
  </s:Header>
  <s:Body xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" xmlns:xsd="http://www.w3.org/2001/XMLSchema">
    <m:SyncFolderItemsResponse xmlns:m="http://schemas.microsoft.com/exchange/services/2006/messages" xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types">
      <m:ResponseMessages>
        <m:SyncFolderItemsResponseMessage ResponseClass="Success">
          <m:ResponseCode>NoError</m:ResponseCode>
          <m:SyncState>H4sIAAAAAAAEAO29B2AcSZY==</m:SyncState>
          <m:IncludesLastItemInRange>true</m:IncludesLastItemInRange>
          <m:Changes>
            <t:Update>
                <t:Message>
                  <t:ItemId Id="q04QAAAA==" ChangeKey="CQAAABYAAADZGACZQpSgSpyNkexYe2b7AAAAird/" />
                  <t:ParentFolderId Id=" AgENAAAA" ChangeKey="AQAAAA==" />
                  <t:ItemClass>IPM.Note</t:ItemClass>
                  <t:Subject>RE: Company Soccer Team</t:Subject>
                  <t:Sensitivity>Normal</t:Sensitivity>
                  <t:DateTimeReceived>2013-08-29T15:22:10Z</t:DateTimeReceived>
                  <t:Size>23110</t:Size>
                  <t:Importance>Normal</t:Importance>
                  <t:InReplyTo>&amp;lt;8e084ea1a5b64f97b95fa8a863a5869d@CH1SR01MB001.namsdf01.sdf.contoso.com&amp;gt;</t:InReplyTo>
                  <t:IsSubmitted>false</t:IsSubmitted>
                  <t:IsDraft>false</t:IsDraft>
                  <t:IsFromMe>false</t:IsFromMe>
                  <t:IsResend>false</t:IsResend>
                  <t:IsUnmodified>false</t:IsUnmodified>
                  <t:DateTimeSent>2013-08-29T15:22:10Z</t:DateTimeSent>
                  <t:DateTimeCreated>2013-08-28T04:07:38Z</t:DateTimeCreated>
                  <t:DisplayCc />
                  <t:DisplayTo>All Employees</t:DisplayTo>
                  <t:HasAttachments>false</t:HasAttachments>
                  <t:Culture>en-US</t:Culture>
                  <t:EffectiveRights>
                    <t:CreateAssociated>false</t:CreateAssociated>
                    <t:CreateContents>false</t:CreateContents>
                    <t:CreateHierarchy>false</t:CreateHierarchy>
                    <t:Delete>true</t:Delete>
                    <t:Modify>true</t:Modify>
                    <t:Read>true</t:Read>
                    <t:ViewPrivateItems>true</t:ViewPrivateItems>
                  </t:EffectiveRights>
                  <t:LastModifiedName>Mara  Whitley</t:LastModifiedName>
                  <t:LastModifiedTime>2013-08-28T16:53:35Z</t:LastModifiedTime>
                  <t:IsAssociated>false</t:IsAssociated>
                  <t:WebClientReadFormQueryString>?ae=Item&amp;amp;a=Open&amp;amp;t=IPM.Note&amp;amp;id=&amp;amp;exvsurl=1</t:WebClientReadFormQueryString>
                  <t:ConversationId Id="AAQkADkzNjJjODUzLWZhMDMtNDVkMS05ZDdjLWVmMDlkYjQ1Zjc4MwAQACAi+NTh0F5Eg5YDwpJsXPE=" />
                  <t:Sender>
                    <t:Mailbox>
                      <t:Name>Alfred  Welker </t:Name>
                      <t:EmailAddress>Alfred.Welker@contoso.com</t:EmailAddress>
                      <t:RoutingType>SMTP</t:RoutingType>
                      <t:MailboxType>Mailbox</t:MailboxType>
                    </t:Mailbox>
                  </t:Sender>
                  <t:IsReadReceiptRequested>false</t:IsReadReceiptRequested>
                  <t:ConversationIndex>AQHM5V/ZICL41OHQXkSDlgPCkmxc8ZYxA3I4gAAP5UeAANHpbIAAEE+0gAABYhSAACGYTIAAA2+vgAAE81qAkhv0Eg==</t:ConversationIndex>
                  <t:ConversationTopic>Company Soccer Team</t:ConversationTopic>
                  <t:From>
                    <t:Mailbox>
                      <t:Name>Alfred  Welker </t:Name>
                      <t:EmailAddress>Alfred.Welker@contoso.com</t:EmailAddress>
                      <t:RoutingType>SMTP</t:RoutingType>
                      <t:MailboxType>Mailbox</t:MailboxType>
                    </t:Mailbox>
                  </t:From>
                  <t:InternetMessageId>&amp;lt;e5919a09c8fc4d64b6ffd3542e194fc3@BY2SR01MB609.contoso.com&amp;gt;</t:InternetMessageId>
                  <t:IsRead>true</t:IsRead>
                  <t:References>namsdf01.sdf.contoso.com&amp;gt;</t:References>
                </t:Message>
            </t:Update>
            <t:Create>
              <t:Message>
                <t:ItemId Id="AQMkAD+" />
                <t:ParentFolderId Id="AQMkA==" ChangeKey="AQAAAA==" />
                <t:ItemClass>IPM.Note</t:ItemClass>
                  <t:Subject>RE: Review Proposal for Contoso</t:Subject>
                  <t:Sensitivity>Normal</t:Sensitivity>
                  <t:DateTimeReceived>2013-08-29T16:20:10Z</t:DateTimeReceived>
                  <t:Size>32515</t:Size>
                  <t:Importance>Normal</t:Importance>
                  <t:InReplyTo>&amp;lt;e52a4de6b98d484887e141da094a2ce6@SN2SR01MB006.contoso.com&amp;gt;</t:InReplyTo>
                  <t:IsSubmitted>false</t:IsSubmitted>
                  <t:IsDraft>false</t:IsDraft>
                  <t:IsFromMe>false</t:IsFromMe>
                  <t:IsResend>false</t:IsResend>
                  <t:IsUnmodified>false</t:IsUnmodified>
                  <t:DateTimeSent>2013-08-29T16:20:10Z</t:DateTimeSent>
                  <t:DateTimeCreated>2013-08-28T04:07:33Z</t:DateTimeCreated>
                  <t:DisplayCc />
                  <t:DisplayTo>Legal Team; Executives</t:DisplayTo>
                  <t:HasAttachments>false</t:HasAttachments>
                  <t:Culture>en-US</t:Culture>
                  <t:EffectiveRights>
                    <t:CreateAssociated>false</t:CreateAssociated>
                    <t:CreateContents>false</t:CreateContents>
                    <t:CreateHierarchy>false</t:CreateHierarchy>
                    <t:Delete>true</t:Delete>
                    <t:Modify>true</t:Modify>
                    <t:Read>true</t:Read>
                    <t:ViewPrivateItems>true</t:ViewPrivateItems>
                  </t:EffectiveRights>
                  <t:LastModifiedName>Mara  Whitley</t:LastModifiedName>
                  <t:LastModifiedTime>2013-08-28T04:07:35Z</t:LastModifiedTime>
                  <t:IsAssociated>false</t:IsAssociated>
                  <t:WebClientReadFormQueryString>?ae=Item&amp;amp;a=Open&amp;amp;t=IPM.Note&amp;amp;id=&amp;amp;exvsurl=1</t:WebClientReadFormQueryString>
                  <t:ConversationId Id="AAQkADkzNjJjODUzLWZhMDMtNDVkMS05ZDdjLWVmMDlkYjQ1Zjc4MwAQAIsBEZp25UpElByLLUQFH6Q=" />
                  <t:Sender>
                    <t:Mailbox>
                      <t:Name>Hope Gross</t:Name>
                      <t:EmailAddress>Hope.Gross@contoso.com</t:EmailAddress>
                      <t:RoutingType>SMTP</t:RoutingType>
                      <t:MailboxType>Mailbox</t:MailboxType>
                    </t:Mailbox>
                  </t:Sender>
                  <t:IsReadReceiptRequested>false</t:IsReadReceiptRequested>
                  <t:ConversationIndex>AQHM5WBRiwERmnblSkSUHIstRAUfpJYw9fbSgAAAdm2AAAB6koAAAHTDgAADl6+AAAbxCYAABm5PgAACSA+AANx034AAEKGQgAAAfsiAAB7m3IAABG+ngAABPZyAAASUzoAAA2DNgAAAfKE=</t:ConversationIndex>
                  <t:ConversationTopic>Review Proposal for Contoso</t:ConversationTopic>
                  <t:From>
                    <t:Mailbox>
                      <t:Name>Hope Gross</t:Name>
                      <t:EmailAddress>Hope.Gross@contoso.com</t:EmailAddress>
                      <t:RoutingType>SMTP</t:RoutingType>
                      <t:MailboxType>Mailbox</t:MailboxType>
                    </t:Mailbox>
                  </t:From>
                  <t:InternetMessageId>&amp;lt;bcdb185495834370a874a1e7ebedbb96@SN2SR01MB005.namsdf01.sdf.contoso.com&amp;gt;</t:InternetMessageId>
                  <t:IsRead>true</t:IsRead>
                  <t:References>&amp;lt;2d4d7d…</t:References>
                </t:Message>
              </t:Create>
              <t:Create>
                <t:Message>
                  <t:ItemId Id="Q04AAAAA==" ChangeKey="AAAirbnd" />
                  <t:ParentFolderId Id="AgENAAAA" ChangeKey="AQAAAA==" />
                  <t:ItemClass>IPM.Note</t:ItemClass>
                  <t:Subject>RE: Review Proposal for Contoso</t:Subject>
                  <t:Sensitivity>Normal</t:Sensitivity>
                  <t:DateTimeReceived>2013-08-29T15:30:10Z</t:DateTimeReceived>
                  <t:Size>29518</t:Size>
                  <t:Importance>Normal</t:Importance>
                  <t:InReplyTo>&amp;lt;f0db3ead01db4fe087d98022149aa16f@SN2SR01MB001.namsdf01.sdf.contoso.com&amp;gt;</t:InReplyTo>
                  <t:IsSubmitted>false</t:IsSubmitted>
                  <t:IsDraft>false</t:IsDraft>
                  <t:IsFromMe>false</t:IsFromMe>
                  <t:IsResend>false</t:IsResend>
                  <t:IsUnmodified>false</t:IsUnmodified>
                  <t:DateTimeSent>2013-08-29T15:30:10Z</t:DateTimeSent>
                  <t:DateTimeCreated>2013-08-28T04:07:36Z</t:DateTimeCreated>
                  <t:DisplayCc />
                  <t:DisplayTo>Legal Team; Executives</t:DisplayTo>
                  <t:HasAttachments>false</t:HasAttachments>
                  <t:Culture>en-US</t:Culture>
                  <t:EffectiveRights>
                    <t:CreateAssociated>false</t:CreateAssociated>
                    <t:CreateContents>false</t:CreateContents>
                    <t:CreateHierarchy>false</t:CreateHierarchy>
                    <t:Delete>true</t:Delete>
                    <t:Modify>true</t:Modify>
                    <t:Read>true</t:Read>
                    <t:ViewPrivateItems>true</t:ViewPrivateItems>
                  </t:EffectiveRights>
                  <t:LastModifiedName>Mara Whitley</t:LastModifiedName>
                  <t:LastModifiedTime>2013-08-28T04:07:38Z</t:LastModifiedTime>
                  <t:IsAssociated>false</t:IsAssociated>
                  <t:WebClientReadFormQueryString>?ae=Item&amp;amp;a=Open&amp;amp;t=IPM.Note&amp;amp;id=&amp;amp;exvsurl=1</t:WebClientReadFormQueryString>
                  <t:ConversationId Id="AAQkADkzNjJjODUzLWZhMDMtNDVkMS05ZDdjLWVmMDlkYjQ1Zjc4MwAQAIsBEZp25UpElByLLUQFH6Q=" />
                  <t:Sender>
                    <t:Mailbox>
                      <t:Name>Mack Chaves</t:Name>
                      <t:EmailAddress>Mack.Chaves@contoso.com</t:EmailAddress>
                      <t:RoutingType>SMTP</t:RoutingType>
                      <t:MailboxType>Mailbox</t:MailboxType>
                    </t:Mailbox>
                  </t:Sender>
                  <t:IsReadReceiptRequested>false</t:IsReadReceiptRequested>
                  <t:ConversationIndex>AQHM5WBRiwERmnblSkSUHIstRAUfpJYw9fbSgAAAdm2AAAB6koAAAHTDgAADl6+AAAbxCYAABm5PgAACSA+AANx034AAEKGQgAAAfsiAAB7m3IAABG+ngAABPZyAAASUzoAAA2DN</t:ConversationIndex>
                  <t:ConversationTopic>Review Proposal for Contoso</t:ConversationTopic>
                  <t:From>
                    <t:Mailbox>
                      <t:Name>Mack Chaves</t:Name>
                      <t:EmailAddress>Mack.Chaves@contoso.com</t:EmailAddress>
                      <t:RoutingType>SMTP</t:RoutingType>
                      <t:MailboxType>Mailbox</t:MailboxType>
                    </t:Mailbox>
                  </t:From>
                  <t:InternetMessageId>&amp;lt;e52a4de6b98d484887e141da094a2ce6@SN2SR01MB006.namsdf01.sdf.contoso.com&amp;gt;</t:InternetMessageId>
                  <t:IsRead>true</t:IsRead>
                  <t:References>namsdf01.sdf.contoso.com&amp;gt;</t:References>
                </t:Message>
              </t:Create>
              <t:ReadFlagChange>
                <t:ItemId Id=" q07AAAAA==" ChangeKey="CQAAAA==" />
                <t:IsRead>true</t:IsRead>
              </t:ReadFlagChange>
              <t:Delete>
                <t:ItemId Id=" q1AwAAAA==" ChangeKey="CQAAAA==" />
              </t:Delete>
          </m:Changes>
        </m:SyncFolderItemsResponseMessage>
      </m:ResponseMessages>
    </m:SyncFolderItemsResponse>
  </s:Body>
</s:Envelope>
```

Операция **SyncFolderItems** аналогична методу [FindItems](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.exchangeservice.finditems%28v=exchg.80%29.aspx) в том, что он не может возвращать элементы, такие как [текст](http://msdn.microsoft.com/library/7851ea9b-9f87-4adc-a26f-7a27df4a9bca%28Office.15%29.aspx) или элементы [вложения](http://msdn.microsoft.com/library/b470e614-34bb-44f0-8790-7ddbdcbbd29d%28Office.15%29.aspx) . <span data-ttu-id="b2fba-147">Если требуются свойства, которые не могут быть возвращены операцией **SyncFolderItems** , установите значение элемента [басешапе](http://msdn.microsoft.com/library/42c04f3b-abaa-4197-a3d6-d21677ffb1c0%28Office.15%29.aspx) в Идонли при вызове **SyncFolderItems**, а затем используйте [операцию GetItem](http://msdn.microsoft.com/library/e3590b8b-c2a7-4dad-a014-6360197b68e4%28Office.15%29.aspx) для получения свойств, необходимых для элементов, возвращенных операцией **SyncFolderItems** .</span><span class="sxs-lookup"><span data-stu-id="b2fba-147">If you need properties that cannot be returned by the **SyncFolderItems** operation, set the value of the [BaseShape](http://msdn.microsoft.com/library/42c04f3b-abaa-4197-a3d6-d21677ffb1c0%28Office.15%29.aspx) element to IdOnly when you call **SyncFolderItems**, and then use the [GetItem operation](http://msdn.microsoft.com/library/e3590b8b-c2a7-4dad-a014-6360197b68e4%28Office.15%29.aspx) to get the properties you require for the items that were returned by the **SyncFolderItems** operation.</span></span> 
  
<span data-ttu-id="b2fba-148">После получения списка измененных элементов на сервере [Обновите элементы на клиенте](#bk_nextsteps).</span><span class="sxs-lookup"><span data-stu-id="b2fba-148">After you retrieve the list of changed items on the server, [update the items on the client](#bk_nextsteps).</span></span>
  
## <a name="update-the-client"></a><span data-ttu-id="b2fba-149">Обновление клиента</span><span class="sxs-lookup"><span data-stu-id="b2fba-149">Update the client</span></span>
<span data-ttu-id="b2fba-150"><a name="bk_nextsteps"> </a></span><span class="sxs-lookup"><span data-stu-id="b2fba-150"><a name="bk_nextsteps"> </a></span></span>

<span data-ttu-id="b2fba-151">Если вы используете управляемый API EWS, после получения списка новых или измененных элементов используйте метод [лоадпропертиесфоритемс](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.exchangeservice.loadpropertiesforitems%28v=exchg.80%29.aspx) , чтобы получить свойства для новых или измененных элементов, сравнить свойства с локальными значениями и обновить элементы в клиенте.</span><span class="sxs-lookup"><span data-stu-id="b2fba-151">If you're using the EWS Managed API, after you get the list of new or changed items, use the [LoadPropertiesForItems](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.exchangeservice.loadpropertiesforitems%28v=exchg.80%29.aspx) method to get properties on the new or changed items, compare the properties to the local values, and update the items on the client.</span></span> 
  
<span data-ttu-id="b2fba-152">Если вы используете EWS, используйте [операцию GetItem](http://msdn.microsoft.com/library/e3590b8b-c2a7-4dad-a014-6360197b68e4%28Office.15%29.aspx) для получения свойств новых или измененных элементов и обновления элементов на клиенте.</span><span class="sxs-lookup"><span data-stu-id="b2fba-152">If you're using EWS, use the [GetItem operation](http://msdn.microsoft.com/library/e3590b8b-c2a7-4dad-a014-6360197b68e4%28Office.15%29.aspx) to get properties on the new or changed items and update the items on the client.</span></span> 
  
## <a name="see-also"></a><span data-ttu-id="b2fba-153">См. также</span><span class="sxs-lookup"><span data-stu-id="b2fba-153">See also</span></span>


- [<span data-ttu-id="b2fba-154">Синхронизация почтового ящика и веб-службах Exchange</span><span class="sxs-lookup"><span data-stu-id="b2fba-154">Mailbox synchronization and EWS in Exchange</span></span>](mailbox-synchronization-and-ews-in-exchange.md)
    
- [<span data-ttu-id="b2fba-155">Синхронизация папок с помощью EWS в Exchange</span><span class="sxs-lookup"><span data-stu-id="b2fba-155">Synchronize folders by using EWS in Exchange</span></span>](how-to-synchronize-folders-by-using-ews-in-exchange.md)
    
- [<span data-ttu-id="b2fba-156">Обработка ошибок, связанных с синхронизацией, в EWS в Exchange</span><span class="sxs-lookup"><span data-stu-id="b2fba-156">Handling synchronization-related errors in EWS in Exchange</span></span>](handling-synchronization-related-errors-in-ews-in-exchange.md)
    
- [<span data-ttu-id="b2fba-157">Подписки на уведомления, события почтовых ящиков и службы EWS в Exchange</span><span class="sxs-lookup"><span data-stu-id="b2fba-157">Notification subscriptions, mailbox events, and EWS in Exchange</span></span>](notification-subscriptions-mailbox-events-and-ews-in-exchange.md)
    

