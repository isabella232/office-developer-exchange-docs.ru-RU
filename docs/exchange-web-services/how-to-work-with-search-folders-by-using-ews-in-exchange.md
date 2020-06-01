---
title: Работайте с папками поиска с помощью EWS в Exchange
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
localization_priority: Normal
ms.assetid: abe703c5-6d85-46d9-bf20-230c34782a9f
description: Узнайте, как создавать, получать, обновлять и удалять папки поиска с помощью управляемого API EWS или EWS в Exchange.
ms.openlocfilehash: 880c14bc99c4f6c674d4f7566036c4b8f5f19e55
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/31/2020
ms.locfileid: "44456369"
---
# <a name="work-with-search-folders-by-using-ews-in-exchange"></a><span data-ttu-id="c7162-103">Работайте с папками поиска с помощью EWS в Exchange</span><span class="sxs-lookup"><span data-stu-id="c7162-103">Work with search folders by using EWS in Exchange</span></span>

<span data-ttu-id="c7162-104">Узнайте, как создавать, получать, обновлять и удалять папки поиска с помощью управляемого API EWS или EWS в Exchange.</span><span class="sxs-lookup"><span data-stu-id="c7162-104">Find out how to create, get, update, and delete search folders by using the EWS Managed API or EWS in Exchange.</span></span>
  
<span data-ttu-id="c7162-105">Папка поиска представляет собой постоянный "постоянный" Поиск в почтовом ящике пользователя.</span><span class="sxs-lookup"><span data-stu-id="c7162-105">A search folder represents a persistent "always-on" search in a user's mailbox.</span></span> <span data-ttu-id="c7162-106">Папка поиска выглядит и действует как обычная папка почтового ящика.</span><span class="sxs-lookup"><span data-stu-id="c7162-106">A search folder looks and acts like a regular mailbox folder.</span></span> <span data-ttu-id="c7162-107">Однако вместо элементов, содержащих элементы, оно содержит "виртуальную" копию элементов из всех папок в ее области поиска, соответствующих критериям поиска, заданным для папки.</span><span class="sxs-lookup"><span data-stu-id="c7162-107">However, instead of containing items, it contains a "virtual" copy of items from any folders in its search scope that match the search criteria set on the folder.</span></span> <span data-ttu-id="c7162-108">Как приложения, так и конечные пользователи могут использовать папки поиска.</span><span class="sxs-lookup"><span data-stu-id="c7162-108">Both applications and end-users can use search folders.</span></span> <span data-ttu-id="c7162-109">Нужно ли приложению выполнять одинаковый Поиск и снова?</span><span class="sxs-lookup"><span data-stu-id="c7162-109">Does your application need to perform the same search over and over?</span></span> <span data-ttu-id="c7162-110">Папки поиска — это отличный инструмент для этой задачи.</span><span class="sxs-lookup"><span data-stu-id="c7162-110">Search folders are a great tool for this task.</span></span> <span data-ttu-id="c7162-111">Или, возможно, вам нужно предоставить пользователям возможность получать доступ к папкам поиска в клиенте и управлять ими.</span><span class="sxs-lookup"><span data-stu-id="c7162-111">Or maybe you just want to give your users the ability to access and manage search folders in your client.</span></span> <span data-ttu-id="c7162-112">Независимо от вашего сценария, управляемый API EWS и EWS позволяют приложению полностью взаимодействовать с папками поиска.</span><span class="sxs-lookup"><span data-stu-id="c7162-112">Whatever your scenario, the EWS Managed API and EWS enable your application to fully interact with search folders.</span></span>

> [!NOTE] 
> <span data-ttu-id="c7162-113">Эта статья относится только к использованию Outlook в интерактивном режиме.</span><span class="sxs-lookup"><span data-stu-id="c7162-113">This article applies only when using Outlook in online mode.</span></span> <span data-ttu-id="c7162-114">Папки поиска не синхронизируются; Поэтому папки поиска, созданные в интерактивном режиме, не будут отображаться в режиме кэширования.</span><span class="sxs-lookup"><span data-stu-id="c7162-114">Search folders do not sync; therefore, search folders created in online mode will not appear in cached mode.</span></span>
  
<span data-ttu-id="c7162-115">**Таблица 1. Методы управляемого API EWS и операции EWS для работы с папками поиска**</span><span class="sxs-lookup"><span data-stu-id="c7162-115">**Table 1. EWS Managed API methods and EWS operations for working with search folders**</span></span>

|<span data-ttu-id="c7162-116">Что требуется сделать</span><span class="sxs-lookup"><span data-stu-id="c7162-116">If you want to…</span></span>|<span data-ttu-id="c7162-117">В управляемом API EWS используйте...</span><span class="sxs-lookup"><span data-stu-id="c7162-117">In the EWS Managed API, use…</span></span>|<span data-ttu-id="c7162-118">В EWS используйте...</span><span class="sxs-lookup"><span data-stu-id="c7162-118">In EWS, use…</span></span>|
|:-----|:-----|:-----|
|<span data-ttu-id="c7162-119">Создание папки поиска</span><span class="sxs-lookup"><span data-stu-id="c7162-119">Create a search folder</span></span>  <br/> |[<span data-ttu-id="c7162-120">SearchFolder. Save</span><span class="sxs-lookup"><span data-stu-id="c7162-120">SearchFolder.Save</span></span>](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.searchfolder.save%28v=exchg.80%29.aspx) <br/> |[<span data-ttu-id="c7162-121">Операция CreateFolder</span><span class="sxs-lookup"><span data-stu-id="c7162-121">CreateFolder operation</span></span>](https://msdn.microsoft.com/library/6f6c334c-b190-4e55-8f0a-38f2a018d1b3%28Office.15%29.aspx) <br/> |
|<span data-ttu-id="c7162-122">Получение папки поиска</span><span class="sxs-lookup"><span data-stu-id="c7162-122">Get a search folder</span></span>  <br/> |[<span data-ttu-id="c7162-123">SearchFolder. Bind</span><span class="sxs-lookup"><span data-stu-id="c7162-123">SearchFolder.Bind</span></span>](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.searchfolder.bind%28v=exchg.80%29.aspx) <br/> |[<span data-ttu-id="c7162-124">Операция GetFolder</span><span class="sxs-lookup"><span data-stu-id="c7162-124">GetFolder operation</span></span>](https://msdn.microsoft.com/library/355bcf93-dc71-4493-b177-622afac5fdb9%28Office.15%29.aspx) <br/> |
|<span data-ttu-id="c7162-125">Обновление папки поиска</span><span class="sxs-lookup"><span data-stu-id="c7162-125">Update a search folder</span></span>  <br/> |[<span data-ttu-id="c7162-126">SearchFolder. Update</span><span class="sxs-lookup"><span data-stu-id="c7162-126">SearchFolder.Update</span></span>](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.folder.update%28v=exchg.80%29.aspx) <br/> |[<span data-ttu-id="c7162-127">Операция UpdateFolder</span><span class="sxs-lookup"><span data-stu-id="c7162-127">UpdateFolder operation</span></span>](https://msdn.microsoft.com/library/3494c996-b834-4813-b1ca-d99642d8b4e7%28Office.15%29.aspx) <br/> |
|<span data-ttu-id="c7162-128">Удаление папки поиска</span><span class="sxs-lookup"><span data-stu-id="c7162-128">Delete a search folder</span></span>  <br/> |[<span data-ttu-id="c7162-129">SearchFolder. Delete</span><span class="sxs-lookup"><span data-stu-id="c7162-129">SearchFolder.Delete</span></span>](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.folder.delete%28v=exchg.80%29.aspx) <br/> |[<span data-ttu-id="c7162-130">Операция DeleteFolder</span><span class="sxs-lookup"><span data-stu-id="c7162-130">DeleteFolder operation</span></span>](https://msdn.microsoft.com/library/b0f92682-4895-4bcf-a4a1-e4c2e8403979%28Office.15%29.aspx) <br/> |
   
## <a name="core-concepts-to-know-for-working-with-search-folders"></a><span data-ttu-id="c7162-131">Основные понятия, которые необходимо знать при работе с папками поиска</span><span class="sxs-lookup"><span data-stu-id="c7162-131">Core concepts to know for working with search folders</span></span>
<span data-ttu-id="c7162-132"><a name="bk_CoreConcepts"> </a></span><span class="sxs-lookup"><span data-stu-id="c7162-132"><a name="bk_CoreConcepts"> </a></span></span>

<span data-ttu-id="c7162-133">Перед началом работы с папками поиска необходимо ознакомиться с принципами работы фильтров поиска.</span><span class="sxs-lookup"><span data-stu-id="c7162-133">Before you start working with search folders, you'll want to be familiar with how search filters work.</span></span> <span data-ttu-id="c7162-134">Для выражения критериев в папках поиска используются фильтры поиска.</span><span class="sxs-lookup"><span data-stu-id="c7162-134">Search folders rely on search filters to express their criteria.</span></span> <span data-ttu-id="c7162-135">Фильтры поиска для папок поиска создаются аналогично тем, как создаются [фильтры поиска для операций поиска](how-to-use-search-filters-with-ews-in-exchange.md) .</span><span class="sxs-lookup"><span data-stu-id="c7162-135">Search filters for search folders are constructed in the same way that [search filters for search operations](how-to-use-search-filters-with-ews-in-exchange.md) are constructed.</span></span> 
  
## <a name="create-a-search-folder-by-using-the-ews-managed-api"></a><span data-ttu-id="c7162-136">Создание папки поиска с помощью управляемого API EWS</span><span class="sxs-lookup"><span data-stu-id="c7162-136">Create a search folder by using the EWS Managed API</span></span>
<span data-ttu-id="c7162-137"><a name="bk_CreateEWSMA"> </a></span><span class="sxs-lookup"><span data-stu-id="c7162-137"><a name="bk_CreateEWSMA"> </a></span></span>

<span data-ttu-id="c7162-138">По сути, папка поиска создается с помощью управляемого API EWS так же, как и обычная папка.</span><span class="sxs-lookup"><span data-stu-id="c7162-138">Basically, you create a search folder using the EWS Managed API in the same way that you create a regular folder.</span></span> <span data-ttu-id="c7162-139">Однако вместо [класса Folder](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.folder%28v=exchg.80%29.aspx)используйте [класс SearchFolder](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.searchfolder%28v=exchg.80%29.aspx)и задайте [свойство сеарчпараметерс](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.searchfolder.searchparameters%28v=exchg.80%29.aspx) для настройки условий поиска.</span><span class="sxs-lookup"><span data-stu-id="c7162-139">However, instead of using the [Folder class](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.folder%28v=exchg.80%29.aspx), you use the [SearchFolder class](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.searchfolder%28v=exchg.80%29.aspx), and set the [SearchParameters property](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.searchfolder.searchparameters%28v=exchg.80%29.aspx) to configure the search criteria.</span></span> 
  
<span data-ttu-id="c7162-140">В следующем примере создается папка поиска для поиска всех сообщений в папке "Входящие" и вложенных папках, отправленных руководителем пользователя sadie@contoso.com.</span><span class="sxs-lookup"><span data-stu-id="c7162-140">In the following example, a search folder is created to find all messages in the Inbox and its subfolders that were sent by the user's manager, sadie@contoso.com.</span></span> <span data-ttu-id="c7162-141">Папка создается как дочерний элемент папки "папки поиска" в почтовом ящике пользователя.</span><span class="sxs-lookup"><span data-stu-id="c7162-141">The folder is created as a child of the Search Folders folder in the user's mailbox.</span></span>
  
> [!NOTE]
> <span data-ttu-id="c7162-142">Вы можете создать папку поиска в качестве дочерней для любой папки в почтовом ящике пользователя.</span><span class="sxs-lookup"><span data-stu-id="c7162-142">You can create a search folder as a child of any folder in the user's mailbox.</span></span> <span data-ttu-id="c7162-143">Тем не менее, если вы хотите, чтобы новая папка отображалась в разделе папки поиска в Outlook, создайте ее в папке Поиск папок, используя значение **SearchFolders** [перечисления веллкновнфолдернаме](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.wellknownfoldername%28v=exchg.80%29.aspx).</span><span class="sxs-lookup"><span data-stu-id="c7162-143">However, if you want the newly created folder to show up under Search Folders in Outlook, create it under the Search Folders well-known folder, using the **SearchFolders** value of the [WellKnownFolderName enumeration](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.wellknownfoldername%28v=exchg.80%29.aspx).</span></span> 
  
<span data-ttu-id="c7162-144">В этом примере предполагается, что для объекта **ExchangeService** выполнена инициализация с допустимыми значениями в свойствах [Credentials](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.exchangeservicebase.credentials%28v=exchg.80%29.aspx) и [Url](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.exchangeservice.url%28v=exchg.80%29.aspx).</span><span class="sxs-lookup"><span data-stu-id="c7162-144">This example assumes that the **ExchangeService** object has been initialized with valid values in the [Credentials](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.exchangeservicebase.credentials%28v=exchg.80%29.aspx) and [Url](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.exchangeservice.url%28v=exchg.80%29.aspx) properties.</span></span> 
  
```cs
using Microsoft.Exchange.WebServices.Data;
static void CreateSearchFolder(ExchangeService service)
{
    // Create the folder.
    SearchFolder searchFolder = new SearchFolder(service);
    searchFolder.DisplayName = "From Manager";
    // Create a search filter to express the criteria
    // for the folder.
    EmailAddress manager = new EmailAddress("sadie@contoso.com");
    SearchFilter.IsEqualTo fromManagerFilter =
        new SearchFilter.IsEqualTo(EmailMessageSchema.Sender, manager);
    // Set the search filter.
    searchFolder.SearchParameters.SearchFilter = fromManagerFilter;
    // Set the folder to search.
    searchFolder.SearchParameters.RootFolderIds.Add(WellKnownFolderName.Inbox);
    // Set the search traversal. Deep will search all subfolders.
    searchFolder.SearchParameters.Traversal = SearchFolderTraversal.Deep;
    // Call Save to make the EWS call to create the folder.
    searchFolder.Save(WellKnownFolderName.SearchFolders);
}
```

## <a name="create-a-search-folder-by-using-ews"></a><span data-ttu-id="c7162-145">Создание папки поиска с помощью EWS</span><span class="sxs-lookup"><span data-stu-id="c7162-145">Create a search folder by using EWS</span></span>
<span data-ttu-id="c7162-146"><a name="bk_CreateEWS"> </a></span><span class="sxs-lookup"><span data-stu-id="c7162-146"><a name="bk_CreateEWS"> </a></span></span>

<span data-ttu-id="c7162-147">Если вы используете EWS, используйте [операцию CreateFolder](https://msdn.microsoft.com/library/6f6c334c-b190-4e55-8f0a-38f2a018d1b3%28Office.15%29.aspx) с элементом [SearchFolder](https://msdn.microsoft.com/library/1a7d408b-2e98-4391-8834-085ed6d5757c%28Office.15%29.aspx) для создания папки поиска.</span><span class="sxs-lookup"><span data-stu-id="c7162-147">If you are using EWS, use the [CreateFolder operation](https://msdn.microsoft.com/library/6f6c334c-b190-4e55-8f0a-38f2a018d1b3%28Office.15%29.aspx) with a [SearchFolder](https://msdn.microsoft.com/library/1a7d408b-2e98-4391-8834-085ed6d5757c%28Office.15%29.aspx) element to create a search folder.</span></span> <span data-ttu-id="c7162-148">В следующем примере создается папка поиска для поиска всех сообщений в папке "Входящие" и вложенных папках, отправленных руководителем пользователя sadie@contoso.com.</span><span class="sxs-lookup"><span data-stu-id="c7162-148">In the following request example, a search folder is created to find all messages in the Inbox and its subfolders that were sent by the user's manager, sadie@contoso.com.</span></span> <span data-ttu-id="c7162-149">Папка будет создана в папке "папки поиска" в почтовом ящике пользователя.</span><span class="sxs-lookup"><span data-stu-id="c7162-149">The folder is created in the Search Folders folder in the user's mailbox.</span></span> 
  
> [!NOTE]
> <span data-ttu-id="c7162-150">Вы можете создать папку поиска в качестве дочерней для любой папки в почтовом ящике пользователя.</span><span class="sxs-lookup"><span data-stu-id="c7162-150">You can create a search folder as a child of any folder in the user's mailbox.</span></span> <span data-ttu-id="c7162-151">Тем не менее, если вы хотите, чтобы новая папка отображалась в разделе папки поиска в Outlook, создайте ее в папке "папки поиска", используя значение **searchfolders** в атрибуте **ID** элемента [дистингуишедфолдерид](https://msdn.microsoft.com/library/50018162-2941-4227-8a5b-d6b4686bb32f%28Office.15%29.aspx) .</span><span class="sxs-lookup"><span data-stu-id="c7162-151">However, if you want the newly created folder to show up under Search Folders in Outlook, create it under the Search Folders well-known folder, using the **searchfolders** value in the **Id** attribute of the [DistinguishedFolderId](https://msdn.microsoft.com/library/50018162-2941-4227-8a5b-d6b4686bb32f%28Office.15%29.aspx) element.</span></span> 
  
```XML
<?xml version="1.0" encoding="utf-8"?>
<soap:Envelope xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" 
    xmlns:m="https://schemas.microsoft.com/exchange/services/2006/messages" 
    xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types" 
    xmlns:soap="https://schemas.xmlsoap.org/soap/envelope/">
  <soap:Header>
    <t:RequestServerVersion Version="Exchange2007_SP1" />
    <t:TimeZoneContext>
      <t:TimeZoneDefinition Id="Eastern Standard Time" />
    </t:TimeZoneContext>
  </soap:Header>
  <soap:Body>
    <m:CreateFolder>
      <m:ParentFolderId>
        <t:DistinguishedFolderId Id="searchfolders" />
      </m:ParentFolderId>
      <m:Folders>
        <t:SearchFolder>
          <t:DisplayName>From Manager</t:DisplayName>
          <t:SearchParameters Traversal="Deep">
            <t:Restriction>
              <t:IsEqualTo>
                <t:FieldURI FieldURI="message:Sender" />
                <t:FieldURIOrConstant>
                  <t:Constant Value="sadie@contoso.com" />
                </t:FieldURIOrConstant>
              </t:IsEqualTo>
            </t:Restriction>
            <t:BaseFolderIds>
              <t:DistinguishedFolderId Id="inbox" />
            </t:BaseFolderIds>
          </t:SearchParameters>
        </t:SearchFolder>
      </m:Folders>
    </m:CreateFolder>
  </soap:Body>
</soap:Envelope>
```

<span data-ttu-id="c7162-152">Сервер отвечает сообщением [креатефолдерреспонсе](https://msdn.microsoft.com/library/158adecc-491a-47d9-af73-acc2cd3f8566%28Office.15%29.aspx) , которое содержит значение [респонсекоде](https://msdn.microsoft.com/library/4b84d670-74c9-4d6d-84e7-f0a9f76f0d93%28Office.15%29.aspx) **, указывающее**на успешное выполнение.</span><span class="sxs-lookup"><span data-stu-id="c7162-152">The server responds with a [CreateFolderResponse](https://msdn.microsoft.com/library/158adecc-491a-47d9-af73-acc2cd3f8566%28Office.15%29.aspx) message that includes a [ResponseCode](https://msdn.microsoft.com/library/4b84d670-74c9-4d6d-84e7-f0a9f76f0d93%28Office.15%29.aspx) value of **NoError**, which indicates success.</span></span>
  
## <a name="get-a-search-folder-by-using-the-ews-managed-api"></a><span data-ttu-id="c7162-153">Получение папки поиска с помощью управляемого API EWS</span><span class="sxs-lookup"><span data-stu-id="c7162-153">Get a search folder by using the EWS Managed API</span></span>
<span data-ttu-id="c7162-154"><a name="bk_RetrieveEWSMA"> </a></span><span class="sxs-lookup"><span data-stu-id="c7162-154"><a name="bk_RetrieveEWSMA"> </a></span></span>

<span data-ttu-id="c7162-155">Используйте метод управляемого API [ExchangeService. финдфолдерс](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.exchangeservice.findfolders%28v=exchg.80%29.aspx) EWS для поиска папок поиска.</span><span class="sxs-lookup"><span data-stu-id="c7162-155">Use the [ExchangeService.FindFolders](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.exchangeservice.findfolders%28v=exchg.80%29.aspx) EWS Managed API method to find search folders.</span></span> <span data-ttu-id="c7162-156">Однако обратите внимание, что вы не можете ограничить результаты только папками поиска; при обработке результатов необходимо помнить об этом.</span><span class="sxs-lookup"><span data-stu-id="c7162-156">Note, however, that you can't limit your results to only include search folders; you'll want to keep that in mind when you process the results.</span></span> <span data-ttu-id="c7162-157">Используйте метод [SearchFolder. Bind](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.searchfolder.bind%28v=exchg.80%29.aspx) для получения папок поиска.</span><span class="sxs-lookup"><span data-stu-id="c7162-157">Use the [SearchFolder.Bind](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.searchfolder.bind%28v=exchg.80%29.aspx) method to get search folders.</span></span> 
  
<span data-ttu-id="c7162-158">В следующем примере показано, как найти первые 10 папок в папке "папки поиска".</span><span class="sxs-lookup"><span data-stu-id="c7162-158">The following example finds the first 10 folders in the Search Folders folder.</span></span> <span data-ttu-id="c7162-159">Он проверяет, является ли каждый из них папкой поиска, и если да, то получает папку поиска и отображает количество целевых папок, в которых она выполняется.</span><span class="sxs-lookup"><span data-stu-id="c7162-159">It checks to determine whether each one is a search folder, and if so, it gets the search folder and displays how many target folders it searches.</span></span>
  
```cs
using Microsoft.Exchange.WebServices.Data;
static void GetSearchFolders(ExchangeService service)
{
    FolderView folderView = new FolderView(10);
    folderView.PropertySet = new PropertySet(FolderSchema.DisplayName);
    try
    {
        FindFoldersResults findResults = service.FindFolders(WellKnownFolderName.SearchFolders, folderView);
        foreach (Folder folder in findResults.Folders)
        {
            // You can't request only search folders in 
            // a FindFolders request, so other search folders might also be present.
            if (folder is SearchFolder)
            {
                Console.WriteLine("{0} is a search folder.", folder.DisplayName);
                // In order to access the SearchParameters property,
                // you have to bind to the folder. SearchParameters are not
                // returned in FindFolders results.
                SearchFolder searchFolder = SearchFolder.Bind(service, folder.Id);
                Console.WriteLine("Number of folders searched: {0}.",
                    searchFolder.SearchParameters.RootFolderIds.Count);
            }
            else
            {
                Console.WriteLine("{0} is NOT a search folder.", folder.DisplayName);
            }
        }
    }
    catch (Exception ex)
    {
        Console.WriteLine("Exception while enumerating results: {0}", ex.Message);
    }
}
```

## <a name="get-a-search-folder-by-using-ews"></a><span data-ttu-id="c7162-160">Получение папки поиска с помощью EWS</span><span class="sxs-lookup"><span data-stu-id="c7162-160">Get a search folder by using EWS</span></span>
<span data-ttu-id="c7162-161"><a name="bk_RetrieveEWS"> </a></span><span class="sxs-lookup"><span data-stu-id="c7162-161"><a name="bk_RetrieveEWS"> </a></span></span>

<span data-ttu-id="c7162-162">Если вы используете EWS, используйте [операцию FindFolder](https://msdn.microsoft.com/library/7a9855aa-06cc-45ba-ad2a-645c15b7d031%28Office.15%29.aspx) для поиска папок поиска и [операцию с папкой](https://msdn.microsoft.com/library/355bcf93-dc71-4493-b177-622afac5fdb9%28Office.15%29.aspx) для получения папок поиска.</span><span class="sxs-lookup"><span data-stu-id="c7162-162">If you're using EWS, use the [FindFolder operation](https://msdn.microsoft.com/library/7a9855aa-06cc-45ba-ad2a-645c15b7d031%28Office.15%29.aspx) to find search folders, and the [GetFolder operation](https://msdn.microsoft.com/library/355bcf93-dc71-4493-b177-622afac5fdb9%28Office.15%29.aspx) to get search folders.</span></span> <span data-ttu-id="c7162-163">Успешный ответ на **папку** поиска для папки поиска будет содержать элемент [SearchFolder](https://msdn.microsoft.com/library/1a7d408b-2e98-4391-8834-085ed6d5757c%28Office.15%29.aspx) .</span><span class="sxs-lookup"><span data-stu-id="c7162-163">A successful **GetFolder** response for a search folder will contain a [SearchFolder](https://msdn.microsoft.com/library/1a7d408b-2e98-4391-8834-085ed6d5757c%28Office.15%29.aspx) element.</span></span> <span data-ttu-id="c7162-164">Приведенный ниже пример запроса находит первые 10 папок в папке "папки поиска".</span><span class="sxs-lookup"><span data-stu-id="c7162-164">The following request example finds the first 10 folders in the Search Folders folder.</span></span> 
  
```XML
<?xml version="1.0" encoding="utf-8"?>
<soap:Envelope xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" 
    xmlns:m="https://schemas.microsoft.com/exchange/services/2006/messages" 
    xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types" 
    xmlns:soap="https://schemas.xmlsoap.org/soap/envelope/">
  <soap:Header>
    <t:RequestServerVersion Version="Exchange2007_SP1" />
    <t:TimeZoneContext>
      <t:TimeZoneDefinition Id="Eastern Standard Time" />
    </t:TimeZoneContext>
  </soap:Header>
  <soap:Body>
    <m:FindFolder Traversal="Shallow">
      <m:FolderShape>
        <t:BaseShape>IdOnly</t:BaseShape>
        <t:AdditionalProperties>
          <t:FieldURI FieldURI="folder:DisplayName" />
        </t:AdditionalProperties>
      </m:FolderShape>
      <m:IndexedPageFolderView MaxEntriesReturned="10" Offset="0" BasePoint="Beginning" />
      <m:ParentFolderIds>
        <t:DistinguishedFolderId Id="searchfolders" />
      </m:ParentFolderIds>
    </m:FindFolder>
  </soap:Body>
</soap:Envelope>
```

<span data-ttu-id="c7162-165">Сервер возвращает следующий ответ, в котором показана одна папка поиска.</span><span class="sxs-lookup"><span data-stu-id="c7162-165">The server returns the following response, which shows one search folder.</span></span>
  
```XML
<?xml version="1.0" encoding="utf-8"?>
<s:Envelope xmlns:s="https://schemas.xmlsoap.org/soap/envelope/">
  <s:Header>
    <h:ServerVersionInfo MajorVersion="15" MinorVersion="0" MajorBuildNumber="712" MinorBuildNumber="22" Version="V2_3" 
        xmlns:h="https://schemas.microsoft.com/exchange/services/2006/types" 
        xmlns="https://schemas.microsoft.com/exchange/services/2006/types" 
        xmlns:xsd="http://www.w3.org/2001/XMLSchema" 
        xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" />
  </s:Header>
  <s:Body xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" xmlns:xsd="http://www.w3.org/2001/XMLSchema">
    <m:FindFolderResponse xmlns:m="https://schemas.microsoft.com/exchange/services/2006/messages" 
        xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types">
      <m:ResponseMessages>
        <m:FindFolderResponseMessage ResponseClass="Success">
          <m:ResponseCode>NoError</m:ResponseCode>
          <m:RootFolder IndexedPagingOffset="3" TotalItemsInView="3" IncludesLastItemInRange="true">
            <t:Folders>
              <t:SearchFolder>
                <t:FolderId Id="AAMkAGM2..." ChangeKey="CAAAABYA..." />
                <t:DisplayName>From Manager</t:DisplayName>
              </t:SearchFolder>
            </t:Folders>
          </m:RootFolder>
        </m:FindFolderResponseMessage>
      </m:ResponseMessages>
    </m:FindFolderResponse>
  </s:Body>
</s:Envelope>
```

<span data-ttu-id="c7162-166">В следующем примере запроса для получения папки поиска используется значение элемента [FolderId](https://msdn.microsoft.com/library/00d14e3e-4365-4f21-8f88-eaeea73b9bf7%28Office.15%29.aspx) из предыдущего ответа из предыдущего ответа в запросе операции с **папкой** .</span><span class="sxs-lookup"><span data-stu-id="c7162-166">The following example of a request uses the value of the [FolderId](https://msdn.microsoft.com/library/00d14e3e-4365-4f21-8f88-eaeea73b9bf7%28Office.15%29.aspx) element from the previous response in a **GetFolder** operation request to get the search folder.</span></span> 
  
```XML
<?xml version="1.0" encoding="utf-8"?>
<soap:Envelope xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" 
    xmlns:m="https://schemas.microsoft.com/exchange/services/2006/messages" 
    xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types" 
    xmlns:soap="https://schemas.xmlsoap.org/soap/envelope/">
  <soap:Header>
    <t:RequestServerVersion Version="Exchange2007_SP1" />
    <t:TimeZoneContext>
      <t:TimeZoneDefinition Id="Eastern Standard Time" />
    </t:TimeZoneContext>
  </soap:Header>
  <soap:Body>
    <m:GetFolder>
      <m:FolderShape>
        <t:BaseShape>AllProperties</t:BaseShape>
      </m:FolderShape>
      <m:FolderIds>
        <t:FolderId Id="AAMkAGM2..." ChangeKey="CAAAABYA..." />
      </m:FolderIds>
    </m:GetFolder>
  </soap:Body>
</soap:Envelope>
```

<span data-ttu-id="c7162-167">Сервер возвращает следующий ответ со всеми свойствами первого класса для папки поиска.</span><span class="sxs-lookup"><span data-stu-id="c7162-167">The server returns the following response with all the first-class properties for the search folder.</span></span>
  
```XML
<?xml version="1.0" encoding="utf-8"?>
<s:Envelope xmlns:s="https://schemas.xmlsoap.org/soap/envelope/">
  <s:Header>
    <h:ServerVersionInfo MajorVersion="15" MinorVersion="0" MajorBuildNumber="712" MinorBuildNumber="22" Version="V2_3" 
        xmlns:h="https://schemas.microsoft.com/exchange/services/2006/types" 
        xmlns="https://schemas.microsoft.com/exchange/services/2006/types" 
        xmlns:xsd="http://www.w3.org/2001/XMLSchema" 
        xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" />
  </s:Header>
  <s:Body xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" xmlns:xsd="http://www.w3.org/2001/XMLSchema">
    <m:GetFolderResponse xmlns:m="https://schemas.microsoft.com/exchange/services/2006/messages" 
        xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types">
      <m:ResponseMessages>
        <m:GetFolderResponseMessage ResponseClass="Success">
          <m:ResponseCode>NoError</m:ResponseCode>
          <m:Folders>
            <t:SearchFolder>
              <t:FolderId Id="AAMkAGM2..." ChangeKey="CAAAABYA..." />
              <t:ParentFolderId Id="AQMkAGM2..." ChangeKey="AQAAAA==" />
              <t:FolderClass>IPF.Note</t:FolderClass>
              <t:DisplayName>From Manager</t:DisplayName>
              <t:TotalCount>8</t:TotalCount>
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
              <t:SearchParameters Traversal="Deep">
                <t:Restriction>
                  <t:IsEqualTo>
                    <t:FieldURI FieldURI="message:Sender" />
                    <t:FieldURIOrConstant>
                      <t:Constant Value="/o=First Organization/ou=Exchange Administrative Group (FYDIBOHF23SPDLT)/cn=Recipients/cn=8d84a3f4cbb34d48838a3aecf99795c0-Sadie" />
                    </t:FieldURIOrConstant>
                  </t:IsEqualTo>
                </t:Restriction>
                <t:BaseFolderIds>
                  <t:FolderId Id="AQMkAGM2..." ChangeKey="AQAAAA==" />
                </t:BaseFolderIds>
              </t:SearchParameters>
            </t:SearchFolder>
          </m:Folders>
        </m:GetFolderResponseMessage>
      </m:ResponseMessages>
    </m:GetFolderResponse>
  </s:Body>
</s:Envelope>
```

## <a name="update-a-search-folder-by-using-the-ews-managed-api"></a><span data-ttu-id="c7162-168">Обновление папки поиска с помощью управляемого API EWS</span><span class="sxs-lookup"><span data-stu-id="c7162-168">Update a search folder by using the EWS Managed API</span></span>
<span data-ttu-id="c7162-169"><a name="bk_UpdateEWSMA"> </a></span><span class="sxs-lookup"><span data-stu-id="c7162-169"><a name="bk_UpdateEWSMA"> </a></span></span>

<span data-ttu-id="c7162-170">Используйте метод [Folder. Update](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.folder.update%28v=exchg.80%29.aspx) Managed API EWS для объекта **SearchFolder** , чтобы обновить папку поиска.</span><span class="sxs-lookup"><span data-stu-id="c7162-170">Use the [Folder.Update](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.folder.update%28v=exchg.80%29.aspx) EWS Managed API method on a **SearchFolder** object to update a search folder.</span></span> <span data-ttu-id="c7162-171">В следующем примере обновляются условия поиска для папки поиска с отображаемым именем "из диспетчера".</span><span class="sxs-lookup"><span data-stu-id="c7162-171">The following example updates the search criteria on a search folder with the display name "From Manager".</span></span> 
  
```cs
using Microsoft.Exchange.WebServices.Data;
static void UpdateSearchFolder(ExchangeService service)
{
    FolderView folderView = new FolderView(10);
    folderView.PropertySet = new PropertySet(FolderSchema.DisplayName);
    try
    {
        FindFoldersResults findResults = service.FindFolders(WellKnownFolderName.SearchFolders, folderView);
        foreach (Folder folder in findResults.Folders)
        {
            // You cannot request only search folders in 
            // a FindFolders request, so other search folders might also be present.
            if (folder is SearchFolder &amp;&amp; folder.DisplayName.Equals("From Manager"))
            {
                Console.WriteLine("\"{0}\" folder found.", folder.DisplayName);
                SearchFolder searchFolder = folder as SearchFolder;
                EmailAddress newManager = new EmailAddress("hope@contoso.com");
                SearchFilter.IsEqualTo newManagerFilter =
                    new SearchFilter.IsEqualTo(EmailMessageSchema.Sender, newManager);
                searchFolder.SearchParameters.SearchFilter = newManagerFilter;
                searchFolder.SearchParameters.RootFolderIds.Add(WellKnownFolderName.Inbox);
                searchFolder.SearchParameters.Traversal = SearchFolderTraversal.Deep;
                searchFolder.Update();
                Console.WriteLine("\"{0}\" folder updated.", folder.DisplayName);
            }
        }
    }
    catch (Exception ex)
    {
        Console.WriteLine("Exception while enumerating results: {0}", ex.Message);
    }
}
```

## <a name="update-a-search-folder-by-using-ews"></a><span data-ttu-id="c7162-172">Обновление папки поиска с помощью EWS</span><span class="sxs-lookup"><span data-stu-id="c7162-172">Update a search folder by using EWS</span></span>
<span data-ttu-id="c7162-173"><a name="bk_UpdateEWS"> </a></span><span class="sxs-lookup"><span data-stu-id="c7162-173"><a name="bk_UpdateEWS"> </a></span></span>

<span data-ttu-id="c7162-174">Если вы используете EWS, используйте [операцию операцию UpdateFolder](https://msdn.microsoft.com/library/3494c996-b834-4813-b1ca-d99642d8b4e7%28Office.15%29.aspx) с элементом [SearchFolder](https://msdn.microsoft.com/library/1a7d408b-2e98-4391-8834-085ed6d5757c%28Office.15%29.aspx) для обновления папки поиска.</span><span class="sxs-lookup"><span data-stu-id="c7162-174">If you're using EWS, use the [UpdateFolder operation](https://msdn.microsoft.com/library/3494c996-b834-4813-b1ca-d99642d8b4e7%28Office.15%29.aspx) with a [SearchFolder](https://msdn.microsoft.com/library/1a7d408b-2e98-4391-8834-085ed6d5757c%28Office.15%29.aspx) element to update a search folder.</span></span> <span data-ttu-id="c7162-175">В следующем примере запроса обновляются условия поиска в папке поиска "из диспетчера".</span><span class="sxs-lookup"><span data-stu-id="c7162-175">The following request example updates the search criteria on the "From Manager" search folder.</span></span> 
  
```XML
<?xml version="1.0" encoding="utf-8"?>
<soap:Envelope xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" 
    xmlns:m="https://schemas.microsoft.com/exchange/services/2006/messages" 
    xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types" 
    xmlns:soap="https://schemas.xmlsoap.org/soap/envelope/">
  <soap:Header>
    <t:RequestServerVersion Version="Exchange2007_SP1" />
    <t:TimeZoneContext>
      <t:TimeZoneDefinition Id="Eastern Standard Time" />
    </t:TimeZoneContext>
  </soap:Header>
  <soap:Body>
    <m:UpdateFolder>
      <m:FolderChanges>
        <t:FolderChange>
          <t:FolderId Id="AAMkAGM2..." ChangeKey="CAAAABYA..." />
          <t:Updates>
            <t:SetFolderField>
              <t:FieldURI FieldURI="folder:SearchParameters" />
              <t:SearchFolder>
                <t:SearchParameters Traversal="Deep">
                  <t:Restriction>
                    <t:IsEqualTo>
                      <t:FieldURI FieldURI="message:Sender" />
                      <t:FieldURIOrConstant>
                        <t:Constant Value="hope@contoso.com" />
                      </t:FieldURIOrConstant>
                    </t:IsEqualTo>
                  </t:Restriction>
                  <t:BaseFolderIds>
                    <t:DistinguishedFolderId Id="inbox" />
                  </t:BaseFolderIds>
                </t:SearchParameters>
              </t:SearchFolder>
            </t:SetFolderField>
          </t:Updates>
        </t:FolderChange>
      </m:FolderChanges>
    </m:UpdateFolder>
  </soap:Body>
</soap:Envelope>
```

<span data-ttu-id="c7162-176">Сервер отвечает сообщением [упдатефолдерреспонсе](https://msdn.microsoft.com/library/31f47739-dc9c-46ba-9e3f-cce25dc85e6e%28Office.15%29.aspx) , которое содержит значение [Респонсекоде](https://msdn.microsoft.com/library/4b84d670-74c9-4d6d-84e7-f0a9f76f0d93%28Office.15%29.aspx) , указывающее **об**успешном выполнении.</span><span class="sxs-lookup"><span data-stu-id="c7162-176">The server responds with an [UpdateFolderResponse](https://msdn.microsoft.com/library/31f47739-dc9c-46ba-9e3f-cce25dc85e6e%28Office.15%29.aspx) message that includes a [ResponseCode](https://msdn.microsoft.com/library/4b84d670-74c9-4d6d-84e7-f0a9f76f0d93%28Office.15%29.aspx) value of **NoError**, which indicates success.</span></span>
  
## <a name="delete-a-search-folder-by-using-the-ews-managed-api"></a><span data-ttu-id="c7162-177">Удаление папки поиска с помощью управляемого API EWS</span><span class="sxs-lookup"><span data-stu-id="c7162-177">Delete a search folder by using the EWS Managed API</span></span>
<span data-ttu-id="c7162-178"><a name="bk_DeleteEWSMA"> </a></span><span class="sxs-lookup"><span data-stu-id="c7162-178"><a name="bk_DeleteEWSMA"> </a></span></span>

<span data-ttu-id="c7162-179">Используйте [папку. Delete](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.folder.delete%28v=exchg.80%29.aspx) метод управляемого API EWS для объекта **SearchFolder** , чтобы удалить папку поиска.</span><span class="sxs-lookup"><span data-stu-id="c7162-179">Use the [Folder.Delete](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.folder.delete%28v=exchg.80%29.aspx) EWS Managed API method on a **SearchFolder** object to delete a search folder.</span></span> <span data-ttu-id="c7162-180">В следующем примере удаляется папка поиска с отображаемым именем "из диспетчера".</span><span class="sxs-lookup"><span data-stu-id="c7162-180">The following example deletes a search folder with the display name "From Manager".</span></span> <span data-ttu-id="c7162-181">Удаленная папка поиска перемещается в папку "Удаленные".</span><span class="sxs-lookup"><span data-stu-id="c7162-181">The deleted search folder is moved to the Deleted Items folder.</span></span> 
  
```cs
using Microsoft.Exchange.WebServices.Data;
static void DeleteSearchFolder(ExchangeService service)
{
    FolderView folderView = new FolderView(10);
    folderView.PropertySet = new PropertySet(FolderSchema.DisplayName);
    try
    {
        FindFoldersResults findResults = service.FindFolders(WellKnownFolderName.SearchFolders, folderView);
        foreach (Folder folder in findResults.Folders)
        {
            // You cannot request only search folders in 
            // a FindFolders request, so other folders might also be present.
            if (folder is SearchFolder &amp;&amp; folder.DisplayName.Equals("From Manager"))
            {
                Console.WriteLine("\"{0}\" folder found.", folder.DisplayName);
                folder.Delete(DeleteMode.MoveToDeletedItems);
                Console.WriteLine("\"{0}\" folder deleted.", folder.DisplayName);
            }
        }
    }
    catch (Exception ex)
    {
        Console.WriteLine("Exception while enumerating results: {0}", ex.Message);
    }
}
```

## <a name="delete-a-search-folder-by-using-ews"></a><span data-ttu-id="c7162-182">Удаление папки поиска с помощью EWS</span><span class="sxs-lookup"><span data-stu-id="c7162-182">Delete a search folder by using EWS</span></span>
<span data-ttu-id="c7162-183"><a name="bk_DeleteEWS"> </a></span><span class="sxs-lookup"><span data-stu-id="c7162-183"><a name="bk_DeleteEWS"> </a></span></span>

<span data-ttu-id="c7162-184">Если вы используете EWS, используйте [операцию DeleteFolder](https://msdn.microsoft.com/library/b0f92682-4895-4bcf-a4a1-e4c2e8403979%28Office.15%29.aspx) для удаления папки поиска.</span><span class="sxs-lookup"><span data-stu-id="c7162-184">If you're using EWS, use the [DeleteFolder operation](https://msdn.microsoft.com/library/b0f92682-4895-4bcf-a4a1-e4c2e8403979%28Office.15%29.aspx) to delete a search folder.</span></span> <span data-ttu-id="c7162-185">В следующем примере папка поиска удаляется и перемещается в папку "Удаленные".</span><span class="sxs-lookup"><span data-stu-id="c7162-185">The following example deletes a search folder and moves it to the Deleted Items folder.</span></span> 
  
```XML
<?xml version="1.0" encoding="utf-8"?>
<soap:Envelope xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" 
    xmlns:m="https://schemas.microsoft.com/exchange/services/2006/messages" 
    xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types" 
    xmlns:soap="https://schemas.xmlsoap.org/soap/envelope/">
  <soap:Header>
    <t:RequestServerVersion Version="Exchange2007_SP1" />
    <t:TimeZoneContext>
      <t:TimeZoneDefinition Id="Eastern Standard Time" />
    </t:TimeZoneContext>
  </soap:Header>
  <soap:Body>
    <m:DeleteFolder DeleteType="MoveToDeletedItems">
      <m:FolderIds>
        <t:FolderId Id="AAMkAGM2..." ChangeKey="CAAAABYA..." />
      </m:FolderIds>
    </m:DeleteFolder>
  </soap:Body>
</soap:Envelope>
```

<span data-ttu-id="c7162-186">Сервер отвечает сообщением [делетефолдерреспонсе](https://msdn.microsoft.com/library/27578bda-ef0a-4a33-bccc-2c1bc1735424%28Office.15%29.aspx) , которое содержит значение [респонсекоде](https://msdn.microsoft.com/library/4b84d670-74c9-4d6d-84e7-f0a9f76f0d93%28Office.15%29.aspx) **, указывающее**на успешное выполнение.</span><span class="sxs-lookup"><span data-stu-id="c7162-186">The server responds with a [DeleteFolderResponse](https://msdn.microsoft.com/library/27578bda-ef0a-4a33-bccc-2c1bc1735424%28Office.15%29.aspx) message that includes a [ResponseCode](https://msdn.microsoft.com/library/4b84d670-74c9-4d6d-84e7-f0a9f76f0d93%28Office.15%29.aspx) value of **NoError**, which indicates success.</span></span>
  
## <a name="see-also"></a><span data-ttu-id="c7162-187">См. также</span><span class="sxs-lookup"><span data-stu-id="c7162-187">See also</span></span>

- [<span data-ttu-id="c7162-188">Поиск и веб-службах Exchange</span><span class="sxs-lookup"><span data-stu-id="c7162-188">Search and EWS in Exchange</span></span>](search-and-ews-in-exchange.md)   
- [<span data-ttu-id="c7162-189">Использование фильтров поиска с EWS в Exchange</span><span class="sxs-lookup"><span data-stu-id="c7162-189">Use search filters with EWS in Exchange</span></span>](how-to-use-search-filters-with-ews-in-exchange.md)    
- [<span data-ttu-id="c7162-190">Класс SearchFolder</span><span class="sxs-lookup"><span data-stu-id="c7162-190">SearchFolder class</span></span>](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.searchfolder%28v=exchg.80%29.aspx)    
- [<span data-ttu-id="c7162-191">Операция CreateFolder</span><span class="sxs-lookup"><span data-stu-id="c7162-191">CreateFolder operation</span></span>](https://msdn.microsoft.com/library/6f6c334c-b190-4e55-8f0a-38f2a018d1b3%28Office.15%29.aspx)    
- [<span data-ttu-id="c7162-192">Операция FindFolder</span><span class="sxs-lookup"><span data-stu-id="c7162-192">FindFolder operation</span></span>](https://msdn.microsoft.com/library/7a9855aa-06cc-45ba-ad2a-645c15b7d031%28Office.15%29.aspx)   
- [<span data-ttu-id="c7162-193">Операция GetFolder</span><span class="sxs-lookup"><span data-stu-id="c7162-193">GetFolder operation</span></span>](https://msdn.microsoft.com/library/355bcf93-dc71-4493-b177-622afac5fdb9%28Office.15%29.aspx)    
- [<span data-ttu-id="c7162-194">Операция UpdateFolder</span><span class="sxs-lookup"><span data-stu-id="c7162-194">UpdateFolder operation</span></span>](https://msdn.microsoft.com/library/3494c996-b834-4813-b1ca-d99642d8b4e7%28Office.15%29.aspx)    
- [<span data-ttu-id="c7162-195">Операция DeleteFolder</span><span class="sxs-lookup"><span data-stu-id="c7162-195">DeleteFolder operation</span></span>](https://msdn.microsoft.com/library/b0f92682-4895-4bcf-a4a1-e4c2e8403979%28Office.15%29.aspx)
    

