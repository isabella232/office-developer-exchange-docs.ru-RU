---
title: Работа с папками поиска с помощью веб-служб Exchange в Exchange
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
localization_priority: Normal
ms.assetid: abe703c5-6d85-46d9-bf20-230c34782a9f
description: Узнайте, как создавать, получение, обновление и удаление папок поиска с помощью управляемого интерфейса API веб-служб Exchange или веб-служб Exchange в Exchange.
ms.openlocfilehash: e38ff50fcdb5e42cea3f4b2e25345375f84ae6eb
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/11/2018
ms.locfileid: "19761163"
---
# <a name="work-with-search-folders-by-using-ews-in-exchange"></a><span data-ttu-id="591e8-103">Работа с папками поиска с помощью веб-служб Exchange в Exchange</span><span class="sxs-lookup"><span data-stu-id="591e8-103">Work with search folders by using EWS in Exchange</span></span>

<span data-ttu-id="591e8-104">Узнайте, как создавать, получение, обновление и удаление папок поиска с помощью управляемого интерфейса API веб-служб Exchange или веб-служб Exchange в Exchange.</span><span class="sxs-lookup"><span data-stu-id="591e8-104">Find out how to create, get, update, and delete search folders by using the EWS Managed API or EWS in Exchange.</span></span>
  
<span data-ttu-id="591e8-105">Папки поиска представляет сохраняемого поиска «всегда на» в почтовом ящике пользователя.</span><span class="sxs-lookup"><span data-stu-id="591e8-105">A search folder represents a persistent "always-on" search in a user's mailbox.</span></span> <span data-ttu-id="591e8-106">Папки поиска выглядит и действует как папка регулярных почтового ящика.</span><span class="sxs-lookup"><span data-stu-id="591e8-106">A search folder looks and acts like a regular mailbox folder.</span></span> <span data-ttu-id="591e8-107">Тем не менее а не содержит элементы, содержит «виртуальный» копию элементов из любой папки в его области поиска, которые соответствуют критериям поиска, заданным в общей папке.</span><span class="sxs-lookup"><span data-stu-id="591e8-107">However, instead of containing items, it contains a "virtual" copy of items from any folders in its search scope that match the search criteria set on the folder.</span></span> <span data-ttu-id="591e8-108">Папки поиска можно использовать приложений и конечных пользователей.</span><span class="sxs-lookup"><span data-stu-id="591e8-108">Both applications and end-users can use search folders.</span></span> <span data-ttu-id="591e8-109">Требуется ли приложение для поиска одни и те же?</span><span class="sxs-lookup"><span data-stu-id="591e8-109">Does your application need to perform the same search over and over?</span></span> <span data-ttu-id="591e8-110">Папки поиска — это превосходное средство для этой задачи.</span><span class="sxs-lookup"><span data-stu-id="591e8-110">Search folders are a great tool for this task.</span></span> <span data-ttu-id="591e8-111">Или, возможно, вам нужно предоставить пользователям возможность доступа и управления папок поиска в клиенте.</span><span class="sxs-lookup"><span data-stu-id="591e8-111">Or maybe you just want to give your users the ability to access and manage search folders in your client.</span></span> <span data-ttu-id="591e8-112">Все, что сценарий, управляемый API EWS и веб-служб Exchange позволяют приложению полностью взаимодействовать с папок поиска.</span><span class="sxs-lookup"><span data-stu-id="591e8-112">Whatever your scenario, the EWS Managed API and EWS enable your application to fully interact with search folders.</span></span>
  
<span data-ttu-id="591e8-113">**В таблице 1. Управляемый API EWS методы и операции веб-служб Exchange для работы с папки поиска**</span><span class="sxs-lookup"><span data-stu-id="591e8-113">**Table 1. EWS Managed API methods and EWS operations for working with search folders**</span></span>

|<span data-ttu-id="591e8-114">**Если вы хотите...**</span><span class="sxs-lookup"><span data-stu-id="591e8-114">**If you want to…**</span></span>|<span data-ttu-id="591e8-115">**В управляемый API веб-служб Exchange используйте...**</span><span class="sxs-lookup"><span data-stu-id="591e8-115">**In the EWS Managed API, use…**</span></span>|<span data-ttu-id="591e8-116">**В веб-служб Exchange используйте...**</span><span class="sxs-lookup"><span data-stu-id="591e8-116">**In EWS, use…**</span></span>|
|:-----|:-----|:-----|
|<span data-ttu-id="591e8-117">Создание папки поиска</span><span class="sxs-lookup"><span data-stu-id="591e8-117">Create a search folder</span></span>  <br/> |[<span data-ttu-id="591e8-118">SearchFolder.Save</span><span class="sxs-lookup"><span data-stu-id="591e8-118">SearchFolder.Save</span></span>](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.searchfolder.save%28v=exchg.80%29.aspx) <br/> |[<span data-ttu-id="591e8-119">CreateFolder Operation</span><span class="sxs-lookup"><span data-stu-id="591e8-119">CreateFolder operation</span></span>](http://msdn.microsoft.com/library/6f6c334c-b190-4e55-8f0a-38f2a018d1b3%28Office.15%29.aspx) <br/> |
|<span data-ttu-id="591e8-120">Получение папки поиска</span><span class="sxs-lookup"><span data-stu-id="591e8-120">Get a search folder</span></span>  <br/> |[<span data-ttu-id="591e8-121">SearchFolder.Bind</span><span class="sxs-lookup"><span data-stu-id="591e8-121">SearchFolder.Bind</span></span>](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.searchfolder.bind%28v=exchg.80%29.aspx) <br/> |[<span data-ttu-id="591e8-122">GetFolder Operation</span><span class="sxs-lookup"><span data-stu-id="591e8-122">GetFolder operation</span></span>](http://msdn.microsoft.com/library/355bcf93-dc71-4493-b177-622afac5fdb9%28Office.15%29.aspx) <br/> |
|<span data-ttu-id="591e8-123">Изменение папки поиска</span><span class="sxs-lookup"><span data-stu-id="591e8-123">Update a search folder</span></span>  <br/> |[<span data-ttu-id="591e8-124">SearchFolder.Update</span><span class="sxs-lookup"><span data-stu-id="591e8-124">SearchFolder.Update</span></span>](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.folder.update%28v=exchg.80%29.aspx) <br/> |[<span data-ttu-id="591e8-125">Операцию UpdateFolder</span><span class="sxs-lookup"><span data-stu-id="591e8-125">UpdateFolder operation</span></span>](http://msdn.microsoft.com/library/3494c996-b834-4813-b1ca-d99642d8b4e7%28Office.15%29.aspx) <br/> |
|<span data-ttu-id="591e8-126">Удаление папки поиска</span><span class="sxs-lookup"><span data-stu-id="591e8-126">Delete a search folder</span></span>  <br/> |[<span data-ttu-id="591e8-127">SearchFolder.Delete</span><span class="sxs-lookup"><span data-stu-id="591e8-127">SearchFolder.Delete</span></span>](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.folder.delete%28v=exchg.80%29.aspx) <br/> |[<span data-ttu-id="591e8-128">Операция DeleteFolder</span><span class="sxs-lookup"><span data-stu-id="591e8-128">DeleteFolder operation</span></span>](http://msdn.microsoft.com/library/b0f92682-4895-4bcf-a4a1-e4c2e8403979%28Office.15%29.aspx) <br/> |
   
## <a name="core-concepts-to-know-for-working-with-search-folders"></a><span data-ttu-id="591e8-129">Основные понятия, которые необходимо знать при работе с папками поиска</span><span class="sxs-lookup"><span data-stu-id="591e8-129">Core concepts to know for working with search folders</span></span>
<span data-ttu-id="591e8-130"><a name="bk_CoreConcepts"> </a></span><span class="sxs-lookup"><span data-stu-id="591e8-130"></span></span>

<span data-ttu-id="591e8-131">Перед началом работы со папок поиска необходимо ознакомиться с как работают фильтры поиска.</span><span class="sxs-lookup"><span data-stu-id="591e8-131">Before you start working with search folders, you'll want to be familiar with how search filters work.</span></span> <span data-ttu-id="591e8-132">Папки поиска используют фильтры поиска для выражения своих критериев.</span><span class="sxs-lookup"><span data-stu-id="591e8-132">Search folders rely on search filters to express their criteria.</span></span> <span data-ttu-id="591e8-133">Фильтры поиска для папок поиска, созданные в таким же образом составляются этого [поисковых фильтров для операции поиска](how-to-use-search-filters-with-ews-in-exchange.md) .</span><span class="sxs-lookup"><span data-stu-id="591e8-133">Search filters for search folders are constructed in the same way that [search filters for search operations](how-to-use-search-filters-with-ews-in-exchange.md) are constructed.</span></span> 
  
## <a name="create-a-search-folder-by-using-the-ews-managed-api"></a><span data-ttu-id="591e8-134">Создание папки поиска с помощью управляемого интерфейса API веб-служб Exchange</span><span class="sxs-lookup"><span data-stu-id="591e8-134">Create a search folder by using the EWS Managed API</span></span>
<span data-ttu-id="591e8-135"><a name="bk_CreateEWSMA"> </a></span><span class="sxs-lookup"><span data-stu-id="591e8-135"></span></span>

<span data-ttu-id="591e8-136">По сути Создание папки поиска с помощью управляемого интерфейса API EWS так же, как создавать регулярные папки.</span><span class="sxs-lookup"><span data-stu-id="591e8-136">Basically, you create a search folder using the EWS Managed API in the same way that you create a regular folder.</span></span> <span data-ttu-id="591e8-137">Тем не менее вместо использования [класса папки](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.folder%28v=exchg.80%29.aspx), следует использовать [класс SearchFolder](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.searchfolder%28v=exchg.80%29.aspx)и устанавливать [SearchParameters свойство](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.searchfolder.searchparameters%28v=exchg.80%29.aspx) для настройки условия поиска.</span><span class="sxs-lookup"><span data-stu-id="591e8-137">However, instead of using the [Folder class](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.folder%28v=exchg.80%29.aspx), you use the [SearchFolder class](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.searchfolder%28v=exchg.80%29.aspx), and set the [SearchParameters property](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.searchfolder.searchparameters%28v=exchg.80%29.aspx) to configure the search criteria.</span></span> 
  
<span data-ttu-id="591e8-138">В следующем примере создается папка поиска для поиска всех сообщений в папке "Входящие" и ее вложенных папок, которые были отправлены менеджера пользователя sadie@contoso.com.</span><span class="sxs-lookup"><span data-stu-id="591e8-138">In the following example, a search folder is created to find all messages in the Inbox and its subfolders that were sent by the user's manager, sadie@contoso.com.</span></span> <span data-ttu-id="591e8-139">Папка создается как дочерний папке папки поиска в почтовом ящике пользователя.</span><span class="sxs-lookup"><span data-stu-id="591e8-139">The folder is created as a child of the Search Folders folder in the user's mailbox.</span></span>
  
> [!NOTE]
> <span data-ttu-id="591e8-140">Можно создать папку поиска как дочерний любой папки в почтовом ящике пользователя.</span><span class="sxs-lookup"><span data-stu-id="591e8-140">You can create a search folder as a child of any folder in the user's mailbox.</span></span> <span data-ttu-id="591e8-141">Тем не менее если необходимо, чтобы только что созданная папка отображается в разделе папки поиска в Outlook, создайте в папке папки поиска известных, с помощью **SearchFolders** значение [перечисления WellKnownFolderName](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.wellknownfoldername%28v=exchg.80%29.aspx).</span><span class="sxs-lookup"><span data-stu-id="591e8-141">However, if you want the newly created folder to show up under Search Folders in Outlook, create it under the Search Folders well-known folder, using the **SearchFolders** value of the [WellKnownFolderName enumeration](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.wellknownfoldername%28v=exchg.80%29.aspx).</span></span> 
  
<span data-ttu-id="591e8-142">В этом примере предполагается, что объект **ExchangeService** была ли инициализирована с допустимые значения для свойства [URL-адреса](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.exchangeservice.url%28v=exchg.80%29.aspx) и [учетных данных](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.exchangeservicebase.credentials%28v=exchg.80%29.aspx) .</span><span class="sxs-lookup"><span data-stu-id="591e8-142">This example assumes that the **ExchangeService** object has been initialized with valid values in the [Credentials](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.exchangeservicebase.credentials%28v=exchg.80%29.aspx) and [Url](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.exchangeservice.url%28v=exchg.80%29.aspx) properties.</span></span> 
  
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

## <a name="create-a-search-folder-by-using-ews"></a><span data-ttu-id="591e8-143">Создание папки поиска с помощью веб-служб Exchange</span><span class="sxs-lookup"><span data-stu-id="591e8-143">Create a search folder by using EWS</span></span>
<span data-ttu-id="591e8-144"><a name="bk_CreateEWS"> </a></span><span class="sxs-lookup"><span data-stu-id="591e8-144"></span></span>

<span data-ttu-id="591e8-145">При использовании веб-служб Exchange с помощью [операции CreateFolder](http://msdn.microsoft.com/library/6f6c334c-b190-4e55-8f0a-38f2a018d1b3%28Office.15%29.aspx) с элементом [SearchFolder](http://msdn.microsoft.com/library/1a7d408b-2e98-4391-8834-085ed6d5757c%28Office.15%29.aspx) для создания папки поиска.</span><span class="sxs-lookup"><span data-stu-id="591e8-145">If you are using EWS, use the [CreateFolder operation](http://msdn.microsoft.com/library/6f6c334c-b190-4e55-8f0a-38f2a018d1b3%28Office.15%29.aspx) with a [SearchFolder](http://msdn.microsoft.com/library/1a7d408b-2e98-4391-8834-085ed6d5757c%28Office.15%29.aspx) element to create a search folder.</span></span> <span data-ttu-id="591e8-146">В следующем примере запрос создания папки поиска для поиска всех сообщений в папке "Входящие" и ее вложенных папок, которые были отправлены менеджера пользователя sadie@contoso.com.</span><span class="sxs-lookup"><span data-stu-id="591e8-146">In the following request example, a search folder is created to find all messages in the Inbox and its subfolders that were sent by the user's manager, sadie@contoso.com.</span></span> <span data-ttu-id="591e8-147">Чтобы создать папку, в папке папки поиска в почтовом ящике пользователя.</span><span class="sxs-lookup"><span data-stu-id="591e8-147">The folder is created in the Search Folders folder in the user's mailbox.</span></span> 
  
> [!NOTE]
> <span data-ttu-id="591e8-148">Можно создать папку поиска как дочерний любой папки в почтовом ящике пользователя.</span><span class="sxs-lookup"><span data-stu-id="591e8-148">You can create a search folder as a child of any folder in the user's mailbox.</span></span> <span data-ttu-id="591e8-149">Тем не менее если требуется только что созданная папка отображается в разделе папки поиска в Outlook, создайте его в папке папки поиска известных, с использованием значения **searchfolders** в атрибуте **Id** элемента [DistinguishedFolderId](http://msdn.microsoft.com/library/50018162-2941-4227-8a5b-d6b4686bb32f%28Office.15%29.aspx) .</span><span class="sxs-lookup"><span data-stu-id="591e8-149">However, if you want the newly created folder to show up under Search Folders in Outlook, create it under the Search Folders well-known folder, using the **searchfolders** value in the **Id** attribute of the [DistinguishedFolderId](http://msdn.microsoft.com/library/50018162-2941-4227-8a5b-d6b4686bb32f%28Office.15%29.aspx) element.</span></span> 
  
```XML
<?xml version="1.0" encoding="utf-8"?>
<soap:Envelope xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" 
    xmlns:m="http://schemas.microsoft.com/exchange/services/2006/messages" 
    xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types" 
    xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/">
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

<span data-ttu-id="591e8-150">Сервер отвечает кодом [CreateFolderResponse](http://msdn.microsoft.com/library/158adecc-491a-47d9-af73-acc2cd3f8566%28Office.15%29.aspx) сообщение, содержащее значение [ResponseCode](http://msdn.microsoft.com/library/4b84d670-74c9-4d6d-84e7-f0a9f76f0d93%28Office.15%29.aspx) **NoError**, который означает успешное выполнение.</span><span class="sxs-lookup"><span data-stu-id="591e8-150">The server responds with a [CreateFolderResponse](http://msdn.microsoft.com/library/158adecc-491a-47d9-af73-acc2cd3f8566%28Office.15%29.aspx) message that includes a [ResponseCode](http://msdn.microsoft.com/library/4b84d670-74c9-4d6d-84e7-f0a9f76f0d93%28Office.15%29.aspx) value of **NoError**, which indicates success.</span></span>
  
## <a name="get-a-search-folder-by-using-the-ews-managed-api"></a><span data-ttu-id="591e8-151">Получение папки поиска с помощью управляемого интерфейса API веб-служб Exchange</span><span class="sxs-lookup"><span data-stu-id="591e8-151">Get a search folder by using the EWS Managed API</span></span>
<span data-ttu-id="591e8-152"><a name="bk_RetrieveEWSMA"> </a></span><span class="sxs-lookup"><span data-stu-id="591e8-152"></span></span>

<span data-ttu-id="591e8-153">Используйте метод [ExchangeService.FindFolders](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.exchangeservice.findfolders%28v=exchg.80%29.aspx) управляемый API EWS для поиска папок поиска.</span><span class="sxs-lookup"><span data-stu-id="591e8-153">Use the [ExchangeService.FindFolders](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.exchangeservice.findfolders%28v=exchg.80%29.aspx) EWS Managed API method to find search folders.</span></span> <span data-ttu-id="591e8-154">Обратите внимание, что нельзя ограничить результаты можно включить только папки поиска; может потребоваться, который следует учитывать при обработки результатов.</span><span class="sxs-lookup"><span data-stu-id="591e8-154">Note, however, that you can't limit your results to only include search folders; you'll want to keep that in mind when you process the results.</span></span> <span data-ttu-id="591e8-155">Используйте метод [SearchFolder.Bind](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.searchfolder.bind%28v=exchg.80%29.aspx) для получения папок поиска.</span><span class="sxs-lookup"><span data-stu-id="591e8-155">Use the [SearchFolder.Bind](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.searchfolder.bind%28v=exchg.80%29.aspx) method to get search folders.</span></span> 
  
<span data-ttu-id="591e8-156">Следующий пример находит первые 10 папок в папке папки поиска.</span><span class="sxs-lookup"><span data-stu-id="591e8-156">The following example finds the first 10 folders in the Search Folders folder.</span></span> <span data-ttu-id="591e8-157">Проверяется, чтобы определить, является ли каждый из папки поиска и, если таким образом, она получает папки поиска и отображает сколько целевые папки будет выполняться поиск.</span><span class="sxs-lookup"><span data-stu-id="591e8-157">It checks to determine whether each one is a search folder, and if so, it gets the search folder and displays how many target folders it searches.</span></span>
  
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

## <a name="get-a-search-folder-by-using-ews"></a><span data-ttu-id="591e8-158">Получение папки поиска с помощью веб-служб Exchange</span><span class="sxs-lookup"><span data-stu-id="591e8-158">Get a search folder by using EWS</span></span>
<span data-ttu-id="591e8-159"><a name="bk_RetrieveEWS"> </a></span><span class="sxs-lookup"><span data-stu-id="591e8-159"></span></span>

<span data-ttu-id="591e8-160">Если вы используете веб-служб Exchange, с помощью [операции FindFolder](http://msdn.microsoft.com/library/7a9855aa-06cc-45ba-ad2a-645c15b7d031%28Office.15%29.aspx) поиск в папках поиска и [операции GetFolder](http://msdn.microsoft.com/library/355bcf93-dc71-4493-b177-622afac5fdb9%28Office.15%29.aspx) для возвращения папок поиска.</span><span class="sxs-lookup"><span data-stu-id="591e8-160">If you're using EWS, use the [FindFolder operation](http://msdn.microsoft.com/library/7a9855aa-06cc-45ba-ad2a-645c15b7d031%28Office.15%29.aspx) to find search folders, and the [GetFolder operation](http://msdn.microsoft.com/library/355bcf93-dc71-4493-b177-622afac5fdb9%28Office.15%29.aspx) to get search folders.</span></span> <span data-ttu-id="591e8-161">Успешного ответа **GetFolder** для папки поиска будет содержать элемент [SearchFolder](http://msdn.microsoft.com/library/1a7d408b-2e98-4391-8834-085ed6d5757c%28Office.15%29.aspx) .</span><span class="sxs-lookup"><span data-stu-id="591e8-161">A successful **GetFolder** response for a search folder will contain a [SearchFolder](http://msdn.microsoft.com/library/1a7d408b-2e98-4391-8834-085ed6d5757c%28Office.15%29.aspx) element.</span></span> <span data-ttu-id="591e8-162">В следующем примере запрос находит первые 10 папок в папке папки поиска.</span><span class="sxs-lookup"><span data-stu-id="591e8-162">The following request example finds the first 10 folders in the Search Folders folder.</span></span> 
  
```XML
<?xml version="1.0" encoding="utf-8"?>
<soap:Envelope xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" 
    xmlns:m="http://schemas.microsoft.com/exchange/services/2006/messages" 
    xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types" 
    xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/">
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

<span data-ttu-id="591e8-163">Сервер возвращает следующие ответ, который отображает один папки поиска.</span><span class="sxs-lookup"><span data-stu-id="591e8-163">The server returns the following response, which shows one search folder.</span></span>
  
```XML
<?xml version="1.0" encoding="utf-8"?>
<s:Envelope xmlns:s="http://schemas.xmlsoap.org/soap/envelope/">
  <s:Header>
    <h:ServerVersionInfo MajorVersion="15" MinorVersion="0" MajorBuildNumber="712" MinorBuildNumber="22" Version="V2_3" 
        xmlns:h="http://schemas.microsoft.com/exchange/services/2006/types" 
        xmlns="http://schemas.microsoft.com/exchange/services/2006/types" 
        xmlns:xsd="http://www.w3.org/2001/XMLSchema" 
        xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" />
  </s:Header>
  <s:Body xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" xmlns:xsd="http://www.w3.org/2001/XMLSchema">
    <m:FindFolderResponse xmlns:m="http://schemas.microsoft.com/exchange/services/2006/messages" 
        xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types">
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

<span data-ttu-id="591e8-164">В следующем примере запроса используется значение элемента [FolderId](http://msdn.microsoft.com/library/00d14e3e-4365-4f21-8f88-eaeea73b9bf7%28Office.15%29.aspx) из предыдущего ответа в запрос операции **GetFolder** для получения папки поиска.</span><span class="sxs-lookup"><span data-stu-id="591e8-164">The following example of a request uses the value of the [FolderId](http://msdn.microsoft.com/library/00d14e3e-4365-4f21-8f88-eaeea73b9bf7%28Office.15%29.aspx) element from the previous response in a **GetFolder** operation request to get the search folder.</span></span> 
  
```XML
<?xml version="1.0" encoding="utf-8"?>
<soap:Envelope xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" 
    xmlns:m="http://schemas.microsoft.com/exchange/services/2006/messages" 
    xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types" 
    xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/">
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

<span data-ttu-id="591e8-165">Сервер возвращает ответ все первого свойства для папки поиска.</span><span class="sxs-lookup"><span data-stu-id="591e8-165">The server returns the following response with all the first-class properties for the search folder.</span></span>
  
```XML
<?xml version="1.0" encoding="utf-8"?>
<s:Envelope xmlns:s="http://schemas.xmlsoap.org/soap/envelope/">
  <s:Header>
    <h:ServerVersionInfo MajorVersion="15" MinorVersion="0" MajorBuildNumber="712" MinorBuildNumber="22" Version="V2_3" 
        xmlns:h="http://schemas.microsoft.com/exchange/services/2006/types" 
        xmlns="http://schemas.microsoft.com/exchange/services/2006/types" 
        xmlns:xsd="http://www.w3.org/2001/XMLSchema" 
        xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" />
  </s:Header>
  <s:Body xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" xmlns:xsd="http://www.w3.org/2001/XMLSchema">
    <m:GetFolderResponse xmlns:m="http://schemas.microsoft.com/exchange/services/2006/messages" 
        xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types">
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

## <a name="update-a-search-folder-by-using-the-ews-managed-api"></a><span data-ttu-id="591e8-166">Изменение папки поиска с помощью управляемого интерфейса API веб-служб Exchange</span><span class="sxs-lookup"><span data-stu-id="591e8-166">Update a search folder by using the EWS Managed API</span></span>
<span data-ttu-id="591e8-167"><a name="bk_UpdateEWSMA"> </a></span><span class="sxs-lookup"><span data-stu-id="591e8-167"></span></span>

<span data-ttu-id="591e8-168">Метод [Folder.Update](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.folder.update%28v=exchg.80%29.aspx) управляемый API EWS для объекта **SearchFolder** обновить папку поиска.</span><span class="sxs-lookup"><span data-stu-id="591e8-168">Use the [Folder.Update](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.folder.update%28v=exchg.80%29.aspx) EWS Managed API method on a **SearchFolder** object to update a search folder.</span></span> <span data-ttu-id="591e8-169">В следующем примере обновляются параметры поиска на папки поиска с отображаемым именем «От руководителя».</span><span class="sxs-lookup"><span data-stu-id="591e8-169">The following example updates the search criteria on a search folder with the display name "From Manager".</span></span> 
  
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

## <a name="update-a-search-folder-by-using-ews"></a><span data-ttu-id="591e8-170">Изменение папки поиска с помощью веб-служб Exchange</span><span class="sxs-lookup"><span data-stu-id="591e8-170">Update a search folder by using EWS</span></span>
<span data-ttu-id="591e8-171"><a name="bk_UpdateEWS"> </a></span><span class="sxs-lookup"><span data-stu-id="591e8-171"></span></span>

<span data-ttu-id="591e8-172">Если вы используете веб-служб Exchange, с помощью [операции UpdateFolder](http://msdn.microsoft.com/library/3494c996-b834-4813-b1ca-d99642d8b4e7%28Office.15%29.aspx) с элементом [SearchFolder](http://msdn.microsoft.com/library/1a7d408b-2e98-4391-8834-085ed6d5757c%28Office.15%29.aspx) обновить папку поиска.</span><span class="sxs-lookup"><span data-stu-id="591e8-172">If you're using EWS, use the [UpdateFolder operation](http://msdn.microsoft.com/library/3494c996-b834-4813-b1ca-d99642d8b4e7%28Office.15%29.aspx) with a [SearchFolder](http://msdn.microsoft.com/library/1a7d408b-2e98-4391-8834-085ed6d5757c%28Office.15%29.aspx) element to update a search folder.</span></span> <span data-ttu-id="591e8-173">В следующем примере запрос на обновление условия поиска для папки поиска «От руководителя».</span><span class="sxs-lookup"><span data-stu-id="591e8-173">The following request example updates the search criteria on the "From Manager" search folder.</span></span> 
  
```XML
<?xml version="1.0" encoding="utf-8"?>
<soap:Envelope xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" 
    xmlns:m="http://schemas.microsoft.com/exchange/services/2006/messages" 
    xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types" 
    xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/">
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

<span data-ttu-id="591e8-174">Сервер отвечает с [UpdateFolderResponse](http://msdn.microsoft.com/library/31f47739-dc9c-46ba-9e3f-cce25dc85e6e%28Office.15%29.aspx) сообщения, которое содержит значение [ResponseCode](http://msdn.microsoft.com/library/4b84d670-74c9-4d6d-84e7-f0a9f76f0d93%28Office.15%29.aspx) **NoError**, который означает успешное выполнение.</span><span class="sxs-lookup"><span data-stu-id="591e8-174">The server responds with an [UpdateFolderResponse](http://msdn.microsoft.com/library/31f47739-dc9c-46ba-9e3f-cce25dc85e6e%28Office.15%29.aspx) message that includes a [ResponseCode](http://msdn.microsoft.com/library/4b84d670-74c9-4d6d-84e7-f0a9f76f0d93%28Office.15%29.aspx) value of **NoError**, which indicates success.</span></span>
  
## <a name="delete-a-search-folder-by-using-the-ews-managed-api"></a><span data-ttu-id="591e8-175">Удаление папки поиска с помощью управляемого интерфейса API веб-служб Exchange</span><span class="sxs-lookup"><span data-stu-id="591e8-175">Delete a search folder by using the EWS Managed API</span></span>
<span data-ttu-id="591e8-176"><a name="bk_DeleteEWSMA"> </a></span><span class="sxs-lookup"><span data-stu-id="591e8-176"></span></span>

<span data-ttu-id="591e8-177">Метод [Folder.Delete](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.folder.delete%28v=exchg.80%29.aspx) управляемый API EWS для объекта **SearchFolder** удаление папки поиска.</span><span class="sxs-lookup"><span data-stu-id="591e8-177">Use the [Folder.Delete](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.folder.delete%28v=exchg.80%29.aspx) EWS Managed API method on a **SearchFolder** object to delete a search folder.</span></span> <span data-ttu-id="591e8-178">В следующем примере удаляется папки поиска с отображаемым именем «От руководителя».</span><span class="sxs-lookup"><span data-stu-id="591e8-178">The following example deletes a search folder with the display name "From Manager".</span></span> <span data-ttu-id="591e8-179">Папка удаленного поиска перемещаются папки "Удаленные".</span><span class="sxs-lookup"><span data-stu-id="591e8-179">The deleted search folder is moved to the Deleted Items folder.</span></span> 
  
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

## <a name="delete-a-search-folder-by-using-ews"></a><span data-ttu-id="591e8-180">Удаление папки поиска с помощью веб-служб Exchange</span><span class="sxs-lookup"><span data-stu-id="591e8-180">Delete a search folder by using EWS</span></span>
<span data-ttu-id="591e8-181"><a name="bk_DeleteEWS"> </a></span><span class="sxs-lookup"><span data-stu-id="591e8-181"></span></span>

<span data-ttu-id="591e8-182">Если вы используете веб-служб Exchange, с помощью [операции DeleteFolder](http://msdn.microsoft.com/library/b0f92682-4895-4bcf-a4a1-e4c2e8403979%28Office.15%29.aspx) удаление папки поиска.</span><span class="sxs-lookup"><span data-stu-id="591e8-182">If you're using EWS, use the [DeleteFolder operation](http://msdn.microsoft.com/library/b0f92682-4895-4bcf-a4a1-e4c2e8403979%28Office.15%29.aspx) to delete a search folder.</span></span> <span data-ttu-id="591e8-183">В следующем примере удаляется папка поиска и переводит его в папку «Удаленные».</span><span class="sxs-lookup"><span data-stu-id="591e8-183">The following example deletes a search folder and moves it to the Deleted Items folder.</span></span> 
  
```XML
<?xml version="1.0" encoding="utf-8"?>
<soap:Envelope xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" 
    xmlns:m="http://schemas.microsoft.com/exchange/services/2006/messages" 
    xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types" 
    xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/">
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

<span data-ttu-id="591e8-184">Сервер отвечает кодом [DeleteFolderResponse](http://msdn.microsoft.com/library/27578bda-ef0a-4a33-bccc-2c1bc1735424%28Office.15%29.aspx) сообщение, содержащее значение [ResponseCode](http://msdn.microsoft.com/library/4b84d670-74c9-4d6d-84e7-f0a9f76f0d93%28Office.15%29.aspx) **NoError**, который означает успешное выполнение.</span><span class="sxs-lookup"><span data-stu-id="591e8-184">The server responds with a [DeleteFolderResponse](http://msdn.microsoft.com/library/27578bda-ef0a-4a33-bccc-2c1bc1735424%28Office.15%29.aspx) message that includes a [ResponseCode](http://msdn.microsoft.com/library/4b84d670-74c9-4d6d-84e7-f0a9f76f0d93%28Office.15%29.aspx) value of **NoError**, which indicates success.</span></span>
  
## <a name="see-also"></a><span data-ttu-id="591e8-185">См. также</span><span class="sxs-lookup"><span data-stu-id="591e8-185">See also</span></span>


- [<span data-ttu-id="591e8-186">Поиск и веб-службах Exchange</span><span class="sxs-lookup"><span data-stu-id="591e8-186">Search and EWS in Exchange</span></span>](search-and-ews-in-exchange.md)
    
- [<span data-ttu-id="591e8-187">Используйте фильтры поиска с помощью веб-служб Exchange в Exchange</span><span class="sxs-lookup"><span data-stu-id="591e8-187">Use search filters with EWS in Exchange</span></span>](how-to-use-search-filters-with-ews-in-exchange.md)
    
- [<span data-ttu-id="591e8-188">Класс SearchFolder</span><span class="sxs-lookup"><span data-stu-id="591e8-188">SearchFolder class</span></span>](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.searchfolder%28v=exchg.80%29.aspx)
    
- [<span data-ttu-id="591e8-189">CreateFolder Operation</span><span class="sxs-lookup"><span data-stu-id="591e8-189">CreateFolder operation</span></span>](http://msdn.microsoft.com/library/6f6c334c-b190-4e55-8f0a-38f2a018d1b3%28Office.15%29.aspx)
    
- [<span data-ttu-id="591e8-190">FindFolder Operation</span><span class="sxs-lookup"><span data-stu-id="591e8-190">FindFolder operation</span></span>](http://msdn.microsoft.com/library/7a9855aa-06cc-45ba-ad2a-645c15b7d031%28Office.15%29.aspx)
    
- [<span data-ttu-id="591e8-191">GetFolder Operation</span><span class="sxs-lookup"><span data-stu-id="591e8-191">GetFolder operation</span></span>](http://msdn.microsoft.com/library/355bcf93-dc71-4493-b177-622afac5fdb9%28Office.15%29.aspx)
    
- [<span data-ttu-id="591e8-192">Операцию UpdateFolder</span><span class="sxs-lookup"><span data-stu-id="591e8-192">UpdateFolder operation</span></span>](http://msdn.microsoft.com/library/3494c996-b834-4813-b1ca-d99642d8b4e7%28Office.15%29.aspx)
    
- [<span data-ttu-id="591e8-193">Операция DeleteFolder</span><span class="sxs-lookup"><span data-stu-id="591e8-193">DeleteFolder operation</span></span>](http://msdn.microsoft.com/library/b0f92682-4895-4bcf-a4a1-e4c2e8403979%28Office.15%29.aspx)
    

