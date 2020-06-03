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
ms.lasthandoff: 06/03/2020
ms.locfileid: "44456369"
---
# <a name="work-with-search-folders-by-using-ews-in-exchange"></a>Работайте с папками поиска с помощью EWS в Exchange

Узнайте, как создавать, получать, обновлять и удалять папки поиска с помощью управляемого API EWS или EWS в Exchange.
  
Папка поиска представляет собой постоянный "постоянный" Поиск в почтовом ящике пользователя. Папка поиска выглядит и действует как обычная папка почтового ящика. Однако вместо элементов, содержащих элементы, оно содержит "виртуальную" копию элементов из всех папок в ее области поиска, соответствующих критериям поиска, заданным для папки. Как приложения, так и конечные пользователи могут использовать папки поиска. Нужно ли приложению выполнять одинаковый Поиск и снова? Папки поиска — это отличный инструмент для этой задачи. Или, возможно, вам нужно предоставить пользователям возможность получать доступ к папкам поиска в клиенте и управлять ими. Независимо от вашего сценария, управляемый API EWS и EWS позволяют приложению полностью взаимодействовать с папками поиска.

> [!NOTE] 
> Эта статья относится только к использованию Outlook в интерактивном режиме. Папки поиска не синхронизируются; Поэтому папки поиска, созданные в интерактивном режиме, не будут отображаться в режиме кэширования.
  
**Таблица 1. Методы управляемого API EWS и операции EWS для работы с папками поиска**

|Что требуется сделать|В управляемом API EWS используйте...|В EWS используйте...|
|:-----|:-----|:-----|
|Создание папки поиска  <br/> |[SearchFolder. Save](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.searchfolder.save%28v=exchg.80%29.aspx) <br/> |[Операция CreateFolder](https://msdn.microsoft.com/library/6f6c334c-b190-4e55-8f0a-38f2a018d1b3%28Office.15%29.aspx) <br/> |
|Получение папки поиска  <br/> |[SearchFolder. Bind](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.searchfolder.bind%28v=exchg.80%29.aspx) <br/> |[Операция GetFolder](https://msdn.microsoft.com/library/355bcf93-dc71-4493-b177-622afac5fdb9%28Office.15%29.aspx) <br/> |
|Обновление папки поиска  <br/> |[SearchFolder. Update](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.folder.update%28v=exchg.80%29.aspx) <br/> |[Операция UpdateFolder](https://msdn.microsoft.com/library/3494c996-b834-4813-b1ca-d99642d8b4e7%28Office.15%29.aspx) <br/> |
|Удаление папки поиска  <br/> |[SearchFolder. Delete](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.folder.delete%28v=exchg.80%29.aspx) <br/> |[Операция DeleteFolder](https://msdn.microsoft.com/library/b0f92682-4895-4bcf-a4a1-e4c2e8403979%28Office.15%29.aspx) <br/> |
   
## <a name="core-concepts-to-know-for-working-with-search-folders"></a>Основные понятия, которые необходимо знать при работе с папками поиска
<a name="bk_CoreConcepts"> </a>

Перед началом работы с папками поиска необходимо ознакомиться с принципами работы фильтров поиска. Для выражения критериев в папках поиска используются фильтры поиска. Фильтры поиска для папок поиска создаются аналогично тем, как создаются [фильтры поиска для операций поиска](how-to-use-search-filters-with-ews-in-exchange.md) . 
  
## <a name="create-a-search-folder-by-using-the-ews-managed-api"></a>Создание папки поиска с помощью управляемого API EWS
<a name="bk_CreateEWSMA"> </a>

По сути, папка поиска создается с помощью управляемого API EWS так же, как и обычная папка. Однако вместо [класса Folder](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.folder%28v=exchg.80%29.aspx)используйте [класс SearchFolder](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.searchfolder%28v=exchg.80%29.aspx)и задайте [свойство сеарчпараметерс](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.searchfolder.searchparameters%28v=exchg.80%29.aspx) для настройки условий поиска. 
  
В следующем примере создается папка поиска для поиска всех сообщений в папке "Входящие" и вложенных папках, отправленных руководителем пользователя sadie@contoso.com. Папка создается как дочерний элемент папки "папки поиска" в почтовом ящике пользователя.
  
> [!NOTE]
> Вы можете создать папку поиска в качестве дочерней для любой папки в почтовом ящике пользователя. Тем не менее, если вы хотите, чтобы новая папка отображалась в разделе папки поиска в Outlook, создайте ее в папке Поиск папок, используя значение **SearchFolders** [перечисления веллкновнфолдернаме](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.wellknownfoldername%28v=exchg.80%29.aspx). 
  
В этом примере предполагается, что для объекта **ExchangeService** выполнена инициализация с допустимыми значениями в свойствах [Credentials](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.exchangeservicebase.credentials%28v=exchg.80%29.aspx) и [Url](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.exchangeservice.url%28v=exchg.80%29.aspx). 
  
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

## <a name="create-a-search-folder-by-using-ews"></a>Создание папки поиска с помощью EWS
<a name="bk_CreateEWS"> </a>

Если вы используете EWS, используйте [операцию CreateFolder](https://msdn.microsoft.com/library/6f6c334c-b190-4e55-8f0a-38f2a018d1b3%28Office.15%29.aspx) с элементом [SearchFolder](https://msdn.microsoft.com/library/1a7d408b-2e98-4391-8834-085ed6d5757c%28Office.15%29.aspx) для создания папки поиска. В следующем примере создается папка поиска для поиска всех сообщений в папке "Входящие" и вложенных папках, отправленных руководителем пользователя sadie@contoso.com. Папка будет создана в папке "папки поиска" в почтовом ящике пользователя. 
  
> [!NOTE]
> Вы можете создать папку поиска в качестве дочерней для любой папки в почтовом ящике пользователя. Тем не менее, если вы хотите, чтобы новая папка отображалась в разделе папки поиска в Outlook, создайте ее в папке "папки поиска", используя значение **searchfolders** в атрибуте **ID** элемента [дистингуишедфолдерид](https://msdn.microsoft.com/library/50018162-2941-4227-8a5b-d6b4686bb32f%28Office.15%29.aspx) . 
  
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

Сервер отвечает сообщением [креатефолдерреспонсе](https://msdn.microsoft.com/library/158adecc-491a-47d9-af73-acc2cd3f8566%28Office.15%29.aspx) , которое содержит значение [респонсекоде](https://msdn.microsoft.com/library/4b84d670-74c9-4d6d-84e7-f0a9f76f0d93%28Office.15%29.aspx) **, указывающее**на успешное выполнение.
  
## <a name="get-a-search-folder-by-using-the-ews-managed-api"></a>Получение папки поиска с помощью управляемого API EWS
<a name="bk_RetrieveEWSMA"> </a>

Используйте метод управляемого API [ExchangeService. финдфолдерс](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.exchangeservice.findfolders%28v=exchg.80%29.aspx) EWS для поиска папок поиска. Однако обратите внимание, что вы не можете ограничить результаты только папками поиска; при обработке результатов необходимо помнить об этом. Используйте метод [SearchFolder. Bind](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.searchfolder.bind%28v=exchg.80%29.aspx) для получения папок поиска. 
  
В следующем примере показано, как найти первые 10 папок в папке "папки поиска". Он проверяет, является ли каждый из них папкой поиска, и если да, то получает папку поиска и отображает количество целевых папок, в которых она выполняется.
  
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

## <a name="get-a-search-folder-by-using-ews"></a>Получение папки поиска с помощью EWS
<a name="bk_RetrieveEWS"> </a>

Если вы используете EWS, используйте [операцию FindFolder](https://msdn.microsoft.com/library/7a9855aa-06cc-45ba-ad2a-645c15b7d031%28Office.15%29.aspx) для поиска папок поиска и [операцию с папкой](https://msdn.microsoft.com/library/355bcf93-dc71-4493-b177-622afac5fdb9%28Office.15%29.aspx) для получения папок поиска. Успешный ответ на **папку** поиска для папки поиска будет содержать элемент [SearchFolder](https://msdn.microsoft.com/library/1a7d408b-2e98-4391-8834-085ed6d5757c%28Office.15%29.aspx) . Приведенный ниже пример запроса находит первые 10 папок в папке "папки поиска". 
  
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

Сервер возвращает следующий ответ, в котором показана одна папка поиска.
  
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

В следующем примере запроса для получения папки поиска используется значение элемента [FolderId](https://msdn.microsoft.com/library/00d14e3e-4365-4f21-8f88-eaeea73b9bf7%28Office.15%29.aspx) из предыдущего ответа из предыдущего ответа в запросе операции с **папкой** . 
  
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

Сервер возвращает следующий ответ со всеми свойствами первого класса для папки поиска.
  
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

## <a name="update-a-search-folder-by-using-the-ews-managed-api"></a>Обновление папки поиска с помощью управляемого API EWS
<a name="bk_UpdateEWSMA"> </a>

Используйте метод [Folder. Update](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.folder.update%28v=exchg.80%29.aspx) Managed API EWS для объекта **SearchFolder** , чтобы обновить папку поиска. В следующем примере обновляются условия поиска для папки поиска с отображаемым именем "из диспетчера". 
  
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

## <a name="update-a-search-folder-by-using-ews"></a>Обновление папки поиска с помощью EWS
<a name="bk_UpdateEWS"> </a>

Если вы используете EWS, используйте [операцию операцию UpdateFolder](https://msdn.microsoft.com/library/3494c996-b834-4813-b1ca-d99642d8b4e7%28Office.15%29.aspx) с элементом [SearchFolder](https://msdn.microsoft.com/library/1a7d408b-2e98-4391-8834-085ed6d5757c%28Office.15%29.aspx) для обновления папки поиска. В следующем примере запроса обновляются условия поиска в папке поиска "из диспетчера". 
  
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

Сервер отвечает сообщением [упдатефолдерреспонсе](https://msdn.microsoft.com/library/31f47739-dc9c-46ba-9e3f-cce25dc85e6e%28Office.15%29.aspx) , которое содержит значение [Респонсекоде](https://msdn.microsoft.com/library/4b84d670-74c9-4d6d-84e7-f0a9f76f0d93%28Office.15%29.aspx) , указывающее **об**успешном выполнении.
  
## <a name="delete-a-search-folder-by-using-the-ews-managed-api"></a>Удаление папки поиска с помощью управляемого API EWS
<a name="bk_DeleteEWSMA"> </a>

Используйте [папку. Delete](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.folder.delete%28v=exchg.80%29.aspx) метод управляемого API EWS для объекта **SearchFolder** , чтобы удалить папку поиска. В следующем примере удаляется папка поиска с отображаемым именем "из диспетчера". Удаленная папка поиска перемещается в папку "Удаленные". 
  
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

## <a name="delete-a-search-folder-by-using-ews"></a>Удаление папки поиска с помощью EWS
<a name="bk_DeleteEWS"> </a>

Если вы используете EWS, используйте [операцию DeleteFolder](https://msdn.microsoft.com/library/b0f92682-4895-4bcf-a4a1-e4c2e8403979%28Office.15%29.aspx) для удаления папки поиска. В следующем примере папка поиска удаляется и перемещается в папку "Удаленные". 
  
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

Сервер отвечает сообщением [делетефолдерреспонсе](https://msdn.microsoft.com/library/27578bda-ef0a-4a33-bccc-2c1bc1735424%28Office.15%29.aspx) , которое содержит значение [респонсекоде](https://msdn.microsoft.com/library/4b84d670-74c9-4d6d-84e7-f0a9f76f0d93%28Office.15%29.aspx) **, указывающее**на успешное выполнение.
  
## <a name="see-also"></a>См. также

- [Поиск и веб-службах Exchange](search-and-ews-in-exchange.md)   
- [Использование фильтров поиска с EWS в Exchange](how-to-use-search-filters-with-ews-in-exchange.md)    
- [Класс SearchFolder](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.searchfolder%28v=exchg.80%29.aspx)    
- [Операция CreateFolder](https://msdn.microsoft.com/library/6f6c334c-b190-4e55-8f0a-38f2a018d1b3%28Office.15%29.aspx)    
- [Операция FindFolder](https://msdn.microsoft.com/library/7a9855aa-06cc-45ba-ad2a-645c15b7d031%28Office.15%29.aspx)   
- [Операция GetFolder](https://msdn.microsoft.com/library/355bcf93-dc71-4493-b177-622afac5fdb9%28Office.15%29.aspx)    
- [Операция UpdateFolder](https://msdn.microsoft.com/library/3494c996-b834-4813-b1ca-d99642d8b4e7%28Office.15%29.aspx)    
- [Операция DeleteFolder](https://msdn.microsoft.com/library/b0f92682-4895-4bcf-a4a1-e4c2e8403979%28Office.15%29.aspx)
    

