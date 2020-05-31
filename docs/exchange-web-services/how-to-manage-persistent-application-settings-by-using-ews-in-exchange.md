---
title: Управление параметрами сохраняемого приложения с помощью EWS в Exchange
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
localization_priority: Normal
ms.assetid: 90f561f2-e40e-4f5b-b321-f86dbf4a1b71
description: Узнайте, как создавать, искать, получать, обновлять и удалять параметры сохраняемого приложения с помощью управляемого API EWS или EWS в Exchange.
ms.openlocfilehash: ab5a9cc927bd0a6c4efacce622cc71db1a9b02a3
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/25/2018
ms.locfileid: "19761044"
---
# <a name="manage-persistent-application-settings-by-using-ews-in-exchange"></a><span data-ttu-id="bdd0a-103">Управление параметрами сохраняемого приложения с помощью EWS в Exchange</span><span class="sxs-lookup"><span data-stu-id="bdd0a-103">Manage persistent application settings by using EWS in Exchange</span></span>

<span data-ttu-id="bdd0a-104">Узнайте, как создавать, искать, получать, обновлять и удалять параметры сохраняемого приложения с помощью управляемого API EWS или EWS в Exchange.</span><span class="sxs-lookup"><span data-stu-id="bdd0a-104">Learn how to create, find, get, update, and delete persistent application settings by using the EWS Managed API or EWS in Exchange.</span></span> 
  
<span data-ttu-id="bdd0a-105">Объекты конфигурации пользователя — это оптимальный способ хранения параметров конфигурации для клиентского приложения Exchange, в основном потому, что они скрыты от результатов поиска в большинстве клиентских приложений.</span><span class="sxs-lookup"><span data-stu-id="bdd0a-105">User configuration objects are the best option for storing configuration settings for your Exchange client application, primarily because they are hidden from search results in most client applications.</span></span> <span data-ttu-id="bdd0a-106">Как правило, клиентские приложения скрывают эти параметры, так как конечный пользователь не видит их, а пользователь случайно не получает доступ к этой информации.</span><span class="sxs-lookup"><span data-stu-id="bdd0a-106">Client applications typically hide these settings because the end user doesn't need to see them, and so that the user doesn't accidentally access this information.</span></span> <span data-ttu-id="bdd0a-107">В примерах кода, приведенных в этой статье, показано, как можно использовать объекты конфигурации пользователей для управления сохраняемыми параметрами, включая создание, поиск, получение, обновление и удаление параметров постоянного приложения, хранящихся в пользовательских объектах конфигурации.</span><span class="sxs-lookup"><span data-stu-id="bdd0a-107">The code examples in this article show you how you can use user configuration objects to manage persistent settings, including how to create, find, get, update, and delete persistent application settings that are stored in user configuration objects.</span></span>

<span data-ttu-id="bdd0a-108"><a name="createconfiguration"> </a></span><span class="sxs-lookup"><span data-stu-id="bdd0a-108"><a name="createconfiguration"> </a></span></span>

## <a name="create-an-application-setting-by-using-the-ews-managed-api"></a><span data-ttu-id="bdd0a-109">Создание параметра приложения с помощью управляемого API EWS</span><span class="sxs-lookup"><span data-stu-id="bdd0a-109">Create an application setting by using the EWS Managed API</span></span>

<span data-ttu-id="bdd0a-110">Для создания настраиваемого параметра конфигурации можно использовать метод [усерконфигуратион. Save](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.userconfiguration.save%28v=exchg.80%29.aspx) для управляемого API EWS.</span><span class="sxs-lookup"><span data-stu-id="bdd0a-110">You can use the [UserConfiguration.Save](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.userconfiguration.save%28v=exchg.80%29.aspx) EWS Managed API method to create a custom configuration setting.</span></span> <span data-ttu-id="bdd0a-111">Объект конфигурации пользователя может содержать XML-файл, двоичный код, словарь данных или сочетание этих трех типов данных.</span><span class="sxs-lookup"><span data-stu-id="bdd0a-111">A user configuration object can contain XML, binary, a data dictionary, or a combination of those three data types.</span></span> <span data-ttu-id="bdd0a-112">В приведенном ниже примере показано, как сохранить объект конфигурации пользователя с именем Контосодрафтсеттингс, который содержит двоичные данные в папке "Черновики", с помощью управляемого API EWS.</span><span class="sxs-lookup"><span data-stu-id="bdd0a-112">The following example shows how to save a user configuration object named ContosoDraftSettings that contains binary data to your Drafts folder by using the EWS Managed API.</span></span> <span data-ttu-id="bdd0a-113">Это может быть полезно, если вы хотите хранить сведения о конфигурации для отображения элементов черновиков в клиентском приложении.</span><span class="sxs-lookup"><span data-stu-id="bdd0a-113">This might be useful if you want to store configuration information about how draft items are displayed in your client application.</span></span> 
  
```cs
private static void CreateUserConfiguration(ExchangeService service, byte[] binaryData)
{
    // Create the user configuration object.
    UserConfiguration configDrafts = new UserConfiguration(service);
    // Add user configuration data to the BinaryData property.
    configDrafts.BinaryData = binaryData;
    // Name and save the user configuration object on the Drafts folder.
    // This results in a call to EWS.
    configDrafts.Save("ContosoDraftSettings", WellKnownFolderName.Drafts);
}
```

## <a name="create-an-application-setting-by-using-ews"></a><span data-ttu-id="bdd0a-114">Создание параметра приложения с помощью EWS</span><span class="sxs-lookup"><span data-stu-id="bdd0a-114">Create an application setting by using EWS</span></span>
<span data-ttu-id="bdd0a-115"><a name="bk_createEWS"> </a></span><span class="sxs-lookup"><span data-stu-id="bdd0a-115"><a name="bk_createEWS"> </a></span></span>

<span data-ttu-id="bdd0a-116">Для создания настраиваемых параметров конфигурации можно использовать операцию [CreateUserConfiguration](http://msdn.microsoft.com/library/eb5b8ab6-9743-481c-aac9-f9aa889bd353%28Office.15%29.aspx) EWS.</span><span class="sxs-lookup"><span data-stu-id="bdd0a-116">You can use the [CreateUserConfiguration](http://msdn.microsoft.com/library/eb5b8ab6-9743-481c-aac9-f9aa889bd353%28Office.15%29.aspx) EWS operation to create a custom configuration setting.</span></span> <span data-ttu-id="bdd0a-117">В следующем примере показан XML-код запроса для создания объекта конфигурации пользователя с именем Контосодрафтсеттингс.</span><span class="sxs-lookup"><span data-stu-id="bdd0a-117">The following example shows the request XML for creating a user configuration object named ContosoDraftSettings.</span></span> <span data-ttu-id="bdd0a-118">Запрос пытается сохранить двоичный поток в объект конфигурации пользователя в папке "Черновики".</span><span class="sxs-lookup"><span data-stu-id="bdd0a-118">The request attempts to save a binary stream to a user configuration object on the Drafts folder.</span></span> <span data-ttu-id="bdd0a-119">Это тот же XML-код, который создается в примере управляемого API EWS.</span><span class="sxs-lookup"><span data-stu-id="bdd0a-119">This is the same XML that is generated by the EWS Managed API example.</span></span> 
  
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
    <m:CreateUserConfiguration>
      <m:UserConfiguration>
        <t:UserConfigurationName Name="ContosoDraftSettings">
          <t:DistinguishedFolderId Id="drafts" />
        </t:UserConfigurationName>
        <t:BinaryData>iVBORw0KGH5UhKquRSzaeAAAAAElFTkSuQmCC</t:BinaryData>
      </m:UserConfiguration>
    </m:CreateUserConfiguration>
  </soap:Body>
</soap:Envelope>
```

<span data-ttu-id="bdd0a-120">[ОТКЛИК XML](http://msdn.microsoft.com/library/eb5b8ab6-9743-481c-aac9-f9aa889bd353%28Office.15%29.aspx) является простым и указывает, был ли запрос на создание успешным или возникла ошибка.</span><span class="sxs-lookup"><span data-stu-id="bdd0a-120">The [response XML](http://msdn.microsoft.com/library/eb5b8ab6-9743-481c-aac9-f9aa889bd353%28Office.15%29.aspx) is simple and indicates whether the create request was successful or whether an error occurred.</span></span> 
  
## <a name="find-an-application-setting-by-using-the-ews-managed-api"></a><span data-ttu-id="bdd0a-121">Поиск параметра приложения с помощью управляемого API EWS</span><span class="sxs-lookup"><span data-stu-id="bdd0a-121">Find an application setting by using the EWS Managed API</span></span>
<span data-ttu-id="bdd0a-122"><a name="findconfiguration"> </a></span><span class="sxs-lookup"><span data-stu-id="bdd0a-122"><a name="findconfiguration"> </a></span></span>

<span data-ttu-id="bdd0a-123">Для поиска объектов конфигурации пользователя можно использовать метод Managed API [Folder. FindItems](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.folder.finditems%28v=exchg.80%29.aspx) EWS с соответствующим параметром обхода.</span><span class="sxs-lookup"><span data-stu-id="bdd0a-123">You can use the [Folder.FindItems](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.folder.finditems%28v=exchg.80%29.aspx) EWS Managed API method with the associated traversal option to find user configuration objects.</span></span> <span data-ttu-id="bdd0a-124">В приведенном ниже примере кода показано, как найти объекты конфигурации пользователя, хранящиеся в папке "Черновики", с помощью управляемого API EWS.</span><span class="sxs-lookup"><span data-stu-id="bdd0a-124">The following code example shows you how to find user configuration objects stored on the Drafts folder by using the EWS Managed API.</span></span> 
  
```cs
private static void FindAssociated(ExchangeService service)
{
    // This is the ItemClass prefix of user configuration objects that are created by using EWS.
    const string userConfigPrefix = "IPM.Configuration.";
            
    // This is the name of a configuration setting created by using EWS.
    string userConfigName = "TestConfig";
    // Return the first five items. 
    ItemView view = new ItemView(5);
    // Request only the properties that you need. Because all the results will be user configuration 
    // objects, you won't need to request the ItemSchema.IsAssociated property, which identifies 
    // user configuration objects.
    PropertySet props = new PropertySet(BasePropertySet.IdOnly, 
                                        ItemSchema.ItemClass);
    view.PropertySet = props;
            
    // Set the traversal to find user configuration objects. 
    view.Traversal = ItemTraversal.Associated;
    // Send the request to search the Drafts folder for all the user configuration objects 
    // in the folder. You do not have to use a search restriction because you will not return
    // a large number of search results. For this scenario, it is better to sort the results
    // on the client. This method results in a call to EWS.
    FindItemsResults<Item> findResults = service.FindItems(WellKnownFolderName.Drafts, view);
    // Output a list of the item classes for the associated items. 
    foreach (Item item in findResults)
    {
        if (item.ItemClass == userConfigPrefix + userConfigName)
        {
            Console.WriteLine("You found the configuration: " + userConfigPrefix + userConfigName);
        }
    }
}
```

## <a name="find-an-application-setting-by-using-ews"></a><span data-ttu-id="bdd0a-125">Поиск параметров приложения с помощью EWS</span><span class="sxs-lookup"><span data-stu-id="bdd0a-125">Find an application setting by using EWS</span></span>
<span data-ttu-id="bdd0a-126"><a name="bk_findEWS"> </a></span><span class="sxs-lookup"><span data-stu-id="bdd0a-126"><a name="bk_findEWS"> </a></span></span>

<span data-ttu-id="bdd0a-127">Для поиска объектов конфигурации пользователя можно использовать операцию [FindItem](http://msdn.microsoft.com/library/ebad6aae-16e7-44de-ae63-a95b24539729%28Office.15%29.aspx) EWS.</span><span class="sxs-lookup"><span data-stu-id="bdd0a-127">You can use the [FindItem](http://msdn.microsoft.com/library/ebad6aae-16e7-44de-ae63-a95b24539729%28Office.15%29.aspx) EWS operation to find user configuration objects.</span></span> 
  
<span data-ttu-id="bdd0a-128">В следующем примере показан XML-код запроса для поиска объектов конфигурации пользователя.</span><span class="sxs-lookup"><span data-stu-id="bdd0a-128">The following example shows the request XML for finding user configuration objects.</span></span> <span data-ttu-id="bdd0a-129">Это тот же XML-код, который создается в примере управляемого API EWS.</span><span class="sxs-lookup"><span data-stu-id="bdd0a-129">This is the same XML that is generated by the EWS Managed API example.</span></span>
  
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
    <m:FindItem Traversal="Associated">
      <m:ItemShape>
        <t:BaseShape>IdOnly</t:BaseShape>
        <t:AdditionalProperties>
          <t:FieldURI FieldURI="item:ItemClass" />
        </t:AdditionalProperties>
      </m:ItemShape>
      <m:IndexedPageItemView MaxEntriesReturned="5" Offset="0" BasePoint="Beginning" />
      <m:ParentFolderIds>
        <t:DistinguishedFolderId Id="drafts" />
      </m:ParentFolderIds>
    </m:FindItem>
  </soap:Body>
</soap:Envelope>
```

<span data-ttu-id="bdd0a-130">В следующем примере показан успешный XML-код ответа для поиска объектов конфигурации пользователя.</span><span class="sxs-lookup"><span data-stu-id="bdd0a-130">The following example shows the successful response XML for finding user configuration objects.</span></span> <span data-ttu-id="bdd0a-131">Это тот же XML-код, который обрабатывается в примере управляемого API EWS.</span><span class="sxs-lookup"><span data-stu-id="bdd0a-131">This is the same XML that is processed by the EWS Managed API example.</span></span> <span data-ttu-id="bdd0a-132">Обратите внимание на следующее в этом ответе XML:</span><span class="sxs-lookup"><span data-stu-id="bdd0a-132">Note the following in this response XML:</span></span> 
  
- <span data-ttu-id="bdd0a-133">Мы сократили идентификатор и изменили ключи для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="bdd0a-133">We shortened the identifier and change keys for readability.</span></span>
    
- <span data-ttu-id="bdd0a-134">Два объекта конфигурации пользователя возвращаются в виде сообщений.</span><span class="sxs-lookup"><span data-stu-id="bdd0a-134">The two user configuration objects are returned as messages.</span></span> <span data-ttu-id="bdd0a-135">Это связано с тем, что операция **FindItem** возвращает все элементы, не определенные в схеме EWS в виде элементов сообщения.</span><span class="sxs-lookup"><span data-stu-id="bdd0a-135">This is because the **FindItem** operation returns all items that are not defined in the EWS schema as message items.</span></span> 
    
- <span data-ttu-id="bdd0a-136">Свойства [ItemClass](http://msdn.microsoft.com/library/56020078-50b4-4880-894a-a9f234033cfb%28Office.15%29.aspx) для двух объектов конфигурации пользователей отличаются.</span><span class="sxs-lookup"><span data-stu-id="bdd0a-136">The [ItemClass](http://msdn.microsoft.com/library/56020078-50b4-4880-894a-a9f234033cfb%28Office.15%29.aspx) properties for the two user configuration objects are different.</span></span> <span data-ttu-id="bdd0a-137">Первый объект конфигурации пользователя был создан с помощью EWS.</span><span class="sxs-lookup"><span data-stu-id="bdd0a-137">The first user configuration object was created by using EWS.</span></span> <span data-ttu-id="bdd0a-138">Второй объект был создан другим API.</span><span class="sxs-lookup"><span data-stu-id="bdd0a-138">The second object was created by another API.</span></span> 
    
```XML
<?xml version="1.0" encoding="utf-8"?>
<s:Envelope xmlns:s="http://schemas.xmlsoap.org/soap/envelope/">
  <s:Header>
    <h:ServerVersionInfo MajorVersion="15" 
                         MinorVersion="0" 
                         MajorBuildNumber="800" 
                         MinorBuildNumber="5" 
                         Version="V2_6" 
                         xmlns:h="http://schemas.microsoft.com/exchange/services/2006/types" 
                         xmlns="http://schemas.microsoft.com/exchange/services/2006/types" 
                         xmlns:xsd="http://www.w3.org/2001/XMLSchema" 
                         xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" />
  </s:Header>
  <s:Body xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" 
          xmlns:xsd="http://www.w3.org/2001/XMLSchema">
    <m:FindItemResponse xmlns:m="http://schemas.microsoft.com/exchange/services/2006/messages" 
                        xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types">
      <m:ResponseMessages>
        <m:FindItemResponseMessage ResponseClass="Success">
          <m:ResponseCode>NoError</m:ResponseCode>
          <m:RootFolder IndexedPagingOffset="2" 
                        TotalItemsInView="2" 
                        IncludesLastItemInRange="true">
            <t:Items>
              <t:Message>
                <t:ItemId Id="AAMkDEY9M6AAA=" ChangeKey="CQAAACYnYF5aFMwP0T" />
                <t:ItemClass>IPM.Configuration.TestConfig</t:ItemClass>
              </t:Message>
              <t:Message>
                <t:ItemId Id="AAkADEzOzFAAA=" ChangeKey="CQAAABQAAABAByOw==" />
                <t:ItemClass>IPM.Microsoft.FolderDesign.NamedView</t:ItemClass>
              </t:Message>
            </t:Items>
          </m:RootFolder>
        </m:FindItemResponseMessage>
      </m:ResponseMessages>
    </m:FindItemResponse>
  </s:Body>
</s:Envelope>
```

## <a name="get-and-update-application-settings-by-using-the-ews-managed-api"></a><span data-ttu-id="bdd0a-139">Получение и обновление параметров приложения с помощью управляемого API EWS</span><span class="sxs-lookup"><span data-stu-id="bdd0a-139">Get and update application settings by using the EWS Managed API</span></span>
<span data-ttu-id="bdd0a-140"><a name="getconfiguration"> </a></span><span class="sxs-lookup"><span data-stu-id="bdd0a-140"><a name="getconfiguration"> </a></span></span>

<span data-ttu-id="bdd0a-141">Найдя объект конфигурации пользователя, вы можете использовать метод управляемого API [усерконфигуратион. Bind](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.userconfiguration.bind%28v=exchg.80%29.aspx) EWS, чтобы получить объект Configuration из почтового ящика.</span><span class="sxs-lookup"><span data-stu-id="bdd0a-141">After you find a user configuration object, you can use the [UserConfiguration.Bind](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.userconfiguration.bind%28v=exchg.80%29.aspx) EWS Managed API method to get the configuration object from the mailbox.</span></span> <span data-ttu-id="bdd0a-142">После получения объекта Configuration можно использовать метод [усерконфигуратион. Update](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.userconfiguration.bind%28v=exchg.80%29.aspx) , чтобы обновить его.</span><span class="sxs-lookup"><span data-stu-id="bdd0a-142">After you get the configuration object, you can use the [UserConfiguration.Update](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.userconfiguration.bind%28v=exchg.80%29.aspx) method to update it.</span></span> <span data-ttu-id="bdd0a-143">В приведенном ниже примере показано, как получить и обновить объект конфигурации пользователя с помощью управляемого API EWS.</span><span class="sxs-lookup"><span data-stu-id="bdd0a-143">The following example shows how to get and update a user configuration object by using the EWS Managed API.</span></span> 
  
```cs
private static void GetAndUpdateUserConfiguration(ExchangeService service)
{
    // Binds to a user configuration object named "TestConfig" in the user's mailbox. 
    // Results in a call to EWS. You can also use the Load method to get the latest
    // server version of the user configuration object.
    UserConfiguration usrConfig = UserConfiguration.Bind(service,
                                                         "TestConfig",
                                                         WellKnownFolderName.Drafts,
                                                         UserConfigurationProperties.All);
            
    // Display the returned configuration object property values.
    if (usrConfig.XmlData != null)
    {
        Console.WriteLine("XmlData: " + Encoding.UTF8.GetString(usrConfig.XmlData));
    }
    if (usrConfig.BinaryData != null)
    {
        Console.WriteLine("BinaryData: " + Encoding.UTF8.GetString(usrConfig.BinaryData));
    }
    if (usrConfig.Dictionary.Count > 0)
    {
        Console.WriteLine("Contains {0} dictionary entries", usrConfig.Dictionary.Count);
    }
    // Add dictionary property values to the local copy of the object.
    usrConfig.Dictionary.Add("Key5", 1);
    // Updates the server version of the user configuration object 
    // if it has changed on the client. Results in a call to EWS.
    if (usrConfig.IsDirty)
    {
        usrConfig.Update();
    }
}
```

## <a name="get-and-update-application-settings-by-using-ews"></a><span data-ttu-id="bdd0a-144">Получение и обновление параметров приложения с помощью EWS</span><span class="sxs-lookup"><span data-stu-id="bdd0a-144">Get and update application settings by using EWS</span></span>
<span data-ttu-id="bdd0a-145"><a name="bk_getEWS"> </a></span><span class="sxs-lookup"><span data-stu-id="bdd0a-145"><a name="bk_getEWS"> </a></span></span>

<span data-ttu-id="bdd0a-146">С помощью операции [GetUserConfiguration](http://msdn.microsoft.com/library/71d50e3c-92bd-435f-8118-b28bb85f8138%28Office.15%29.aspx) EWS можно получить объект конфигурации из почтового ящика и [UpdateUserConfiguration](http://msdn.microsoft.com/library/eda73b62-6a3a-43ae-8fd9-f30892811f27%28Office.15%29.aspx) для обновления объекта.</span><span class="sxs-lookup"><span data-stu-id="bdd0a-146">You can use the [GetUserConfiguration](http://msdn.microsoft.com/library/71d50e3c-92bd-435f-8118-b28bb85f8138%28Office.15%29.aspx) EWS operation to retrieve the configuration object from the mailbox, and the [UpdateUserConfiguration](http://msdn.microsoft.com/library/eda73b62-6a3a-43ae-8fd9-f30892811f27%28Office.15%29.aspx) to update the object.</span></span> <span data-ttu-id="bdd0a-147">В следующем примере показан XML-код запроса для получения объекта конфигурации пользователя с именем Тестконфиг.</span><span class="sxs-lookup"><span data-stu-id="bdd0a-147">The following example shows the request XML for getting a user configuration object named TestConfig.</span></span> <span data-ttu-id="bdd0a-148">Запрос утверждает, что все конфигурации должны быть возвращены в ответе.</span><span class="sxs-lookup"><span data-stu-id="bdd0a-148">The request states that all configurations should be returned in the response.</span></span> <span data-ttu-id="bdd0a-149">Это тот же XML-код, который создается в примере управляемого API EWS.</span><span class="sxs-lookup"><span data-stu-id="bdd0a-149">This is the same XML that is generated by the EWS Managed API example.</span></span> 
  
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
    <m:GetUserConfiguration>
      <m:UserConfigurationName Name="TestConfig">
        <t:DistinguishedFolderId Id="drafts" />
      </m:UserConfigurationName>
      <m:UserConfigurationProperties>All</m:UserConfigurationProperties>
    </m:GetUserConfiguration>
  </soap:Body>
</soap:Envelope>
```

<span data-ttu-id="bdd0a-150">В следующем примере показан успешный XML-код отклика для возврата объектов конфигурации пользователя.</span><span class="sxs-lookup"><span data-stu-id="bdd0a-150">The following example shows the successful response XML for getting a user configuration objects.</span></span> <span data-ttu-id="bdd0a-151">Ответ содержит словарь данных.</span><span class="sxs-lookup"><span data-stu-id="bdd0a-151">The response contains a data dictionary.</span></span> <span data-ttu-id="bdd0a-152">Это тот же XML-код, который обрабатывается в примере управляемого API EWS.</span><span class="sxs-lookup"><span data-stu-id="bdd0a-152">This is the same XML that is processed by the EWS Managed API example.</span></span> 
  
```XML
<?xml version="1.0" encoding="utf-8"?>
<s:Envelope xmlns:s="http://schemas.xmlsoap.org/soap/envelope/">
  <s:Header>
    <h:ServerVersionInfo MajorVersion="15" 
                         MinorVersion="0" 
                         MajorBuildNumber="800" 
                         MinorBuildNumber="5" 
                         Version="V2_6" 
                         xmlns:h="http://schemas.microsoft.com/exchange/services/2006/types" 
                         xmlns="http://schemas.microsoft.com/exchange/services/2006/types" 
                         xmlns:xsd="http://www.w3.org/2001/XMLSchema" 
                         xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" />
  </s:Header>
  <s:Body xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" 
          xmlns:xsd="http://www.w3.org/2001/XMLSchema">
    <m:GetUserConfigurationResponse xmlns:m="http://schemas.microsoft.com/exchange/services/2006/messages" 
                                    xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types">
      <m:ResponseMessages>
        <m:GetUserConfigurationResponseMessage ResponseClass="Success">
          <m:ResponseCode>NoError</m:ResponseCode>
          <m:UserConfiguration>
            <t:UserConfigurationName Name="TestConfig">
              <t:DistinguishedFolderId Id="drafts" />
            </t:UserConfigurationName>
            <t:ItemId Id="AAMkDEY9M6AAA=" ChangeKey="CQAAACYnYF5aFMwP0T" />
            <t:Dictionary>
              <t:DictionaryEntry>
                <t:DictionaryKey>
                  <t:Type>String</t:Type>
                  <t:Value>Key1</t:Value>
                </t:DictionaryKey>
                <t:DictionaryValue>
                  <t:Type>Integer32</t:Type>
                  <t:Value>1</t:Value>
                </t:DictionaryValue>
              </t:DictionaryEntry>
              <t:DictionaryEntry>
                <t:DictionaryKey>
                  <t:Type>String</t:Type>
                  <t:Value>PhoneNumber</t:Value>
                </t:DictionaryKey>
                <t:DictionaryValue>
                  <t:Type>String</t:Type>
                  <t:Value>555-555-1111</t:Value>
                </t:DictionaryValue>
              </t:DictionaryEntry>
            </t:Dictionary>
          </m:UserConfiguration>
        </m:GetUserConfigurationResponseMessage>
      </m:ResponseMessages>
    </m:GetUserConfigurationResponse>
  </s:Body>
</s:Envelope>
```

<span data-ttu-id="bdd0a-153">В следующем примере показан XML-код запроса для обновления объекта конфигурации пользователя.</span><span class="sxs-lookup"><span data-stu-id="bdd0a-153">The following example shows the request XML for updating a user configuration object.</span></span> <span data-ttu-id="bdd0a-154">Запрос утверждает, что все конфигурации должны быть возвращены в ответе.</span><span class="sxs-lookup"><span data-stu-id="bdd0a-154">The request states that all configurations should be returned in the response.</span></span> <span data-ttu-id="bdd0a-155">Это тот же XML-код, который создается с помощью управляемого API EWS в примере, в котором вызывается метод **усерконфигуратион. Update** .</span><span class="sxs-lookup"><span data-stu-id="bdd0a-155">This is the same XML that is generated by the EWS Managed API example that calls the **UserConfiguration.Update** method.</span></span> <span data-ttu-id="bdd0a-156">Вы видите, что XML-файл обновления содержит существующие записи словаря и дополнительный, добавленный перед обновлением.</span><span class="sxs-lookup"><span data-stu-id="bdd0a-156">You can see that the update XML contains the existing dictionary entries and the additional one that was added before the update.</span></span> 
  
```xml
<?xml version="1.0" encoding="utf-8"?>
<soap:Envelope xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" 
               xmlns:m="http://schemas.microsoft.com/exchange/services/2006/messages" 
               xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types" 
               xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/">
  <soap:Header>
    <t:RequestServerVersion Version="Exchange2013" />
  </soap:Header>
  <soap:Body>
    <m:UpdateUserConfiguration>
      <m:UserConfiguration>
        <t:UserConfigurationName Name="TestConfig">
          <t:DistinguishedFolderId Id="drafts" />
        </t:UserConfigurationName>
        <t:Dictionary>
          <t:DictionaryEntry>
            <t:DictionaryKey>
              <t:Type>String</t:Type>
              <t:Value>Key1</t:Value>
            </t:DictionaryKey>
            <t:DictionaryValue>
              <t:Type>Integer32</t:Type>
              <t:Value>1</t:Value>
            </t:DictionaryValue>
          </t:DictionaryEntry>
          <t:DictionaryEntry>
            <t:DictionaryKey>
              <t:Type>String</t:Type>
              <t:Value>PhoneNumber</t:Value>
            </t:DictionaryKey>
            <t:DictionaryValue>
              <t:Type>String</t:Type>
              <t:Value>555-555-1111</t:Value>
            </t:DictionaryValue>
          </t:DictionaryEntry>
          <t:DictionaryEntry>
            <t:DictionaryKey>
              <t:Type>String</t:Type>
              <t:Value>Key5</t:Value>
            </t:DictionaryKey>
            <t:DictionaryValue>
              <t:Type>Integer32</t:Type>
              <t:Value>1</t:Value>
            </t:DictionaryValue>
          </t:DictionaryEntry>
        </t:Dictionary>
      </m:UserConfiguration>
    </m:UpdateUserConfiguration>
  </soap:Body>
</soap:Envelope>
```

<span data-ttu-id="bdd0a-157">[ОТКЛИК XML](http://msdn.microsoft.com/library/eda73b62-6a3a-43ae-8fd9-f30892811f27%28Office.15%29.aspx) является простым и указывает, было ли обновление успешным или произошла ошибка.</span><span class="sxs-lookup"><span data-stu-id="bdd0a-157">The [response XML](http://msdn.microsoft.com/library/eda73b62-6a3a-43ae-8fd9-f30892811f27%28Office.15%29.aspx) is simple and indicates whether the update was successful or whether an error occurred.</span></span> 
  
## <a name="delete-an-application-setting-by-using-the-ews-managed-api"></a><span data-ttu-id="bdd0a-158">Удаление параметра приложения с помощью управляемого API EWS</span><span class="sxs-lookup"><span data-stu-id="bdd0a-158">Delete an application setting by using the EWS Managed API</span></span>
<span data-ttu-id="bdd0a-159"><a name="deleteconfiguration"> </a></span><span class="sxs-lookup"><span data-stu-id="bdd0a-159"><a name="deleteconfiguration"> </a></span></span>

<span data-ttu-id="bdd0a-160">Для удаления объектов конфигурации пользователя можно использовать метод [усерконфигуратион. Delete](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.userconfiguration.delete%28v=exchg.80%29.aspx) для управляемого API EWS.</span><span class="sxs-lookup"><span data-stu-id="bdd0a-160">You can use the [UserConfiguration.Delete](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.userconfiguration.delete%28v=exchg.80%29.aspx) EWS Managed API method to delete user configuration objects.</span></span> <span data-ttu-id="bdd0a-161">В приведенном ниже примере кода показано, как удалить объект конфигурации пользователя Контосодрафтсеттингс с помощью управляемого API EWS.</span><span class="sxs-lookup"><span data-stu-id="bdd0a-161">The following code example shows you how to delete the ContosoDraftSettings user configuration object by using the EWS Managed API.</span></span> 
  
```cs
private static void DeleteUserConfiguration(ExchangeService service)
{
    // Binds to a user configuration object. Results in a call to EWS.
    UserConfiguration usrConfig = UserConfiguration.Bind(service,
                                                        "ContosoDraftSettings",
                                                        WellKnownFolderName.Drafts,
                                                        UserConfigurationProperties.Id);
    // Deletes the user configuration object.
    // Results in a call to EWS.
    usrConfig.Delete();
}
```

## <a name="delete-an-application-setting-by-using-ews"></a><span data-ttu-id="bdd0a-162">Удаление параметра приложения с помощью EWS</span><span class="sxs-lookup"><span data-stu-id="bdd0a-162">Delete an application setting by using EWS</span></span>
<span data-ttu-id="bdd0a-163"><a name="bk_deleteEWS"> </a></span><span class="sxs-lookup"><span data-stu-id="bdd0a-163"><a name="bk_deleteEWS"> </a></span></span>

<span data-ttu-id="bdd0a-164">Для удаления объектов конфигурации пользователя можно использовать операцию [DeleteUserConfiguration](http://msdn.microsoft.com/library/93e44690-be2d-4fdb-96a8-4ded3c193aed%28Office.15%29.aspx) EWS.</span><span class="sxs-lookup"><span data-stu-id="bdd0a-164">You can use the [DeleteUserConfiguration](http://msdn.microsoft.com/library/93e44690-be2d-4fdb-96a8-4ded3c193aed%28Office.15%29.aspx) EWS operation to delete user configuration objects.</span></span> 
  
<span data-ttu-id="bdd0a-165">В следующем примере показан XML-код запроса для удаления объекта конфигурации пользователя с именем Контосодрафтсеттингс, который был применен к папке "Черновики".</span><span class="sxs-lookup"><span data-stu-id="bdd0a-165">The following example shows the request XML for deleting a user configuration object named ContosoDraftSettings that was applied to the Drafts folder.</span></span> <span data-ttu-id="bdd0a-166">Это тот же XML-код, который создается в примере управляемого API EWS.</span><span class="sxs-lookup"><span data-stu-id="bdd0a-166">This is the same XML that is generated by the EWS Managed API example.</span></span>
  
```xml
<?xml version="1.0" encoding="utf-8"?>
<soap:Envelope xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" 
               xmlns:m="http://schemas.microsoft.com/exchange/services/2006/messages" 
               xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types" 
               xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/">
  <soap:Header>
    <t:RequestServerVersion Version="Exchange2013" />
  </soap:Header>
  <soap:Body>
    <m:DeleteUserConfiguration>
      <m:UserConfigurationName Name="ContosoDraftSettings">
        <t:DistinguishedFolderId Id="drafts" />
      </m:UserConfigurationName>
    </m:DeleteUserConfiguration>
  </soap:Body>
</soap:Envelope>
```

<span data-ttu-id="bdd0a-167">[XML-код отклика](http://msdn.microsoft.com/library/93e44690-be2d-4fdb-96a8-4ded3c193aed%28Office.15%29.aspx) прост и указывает, был ли запрос на удаление успешным, или возникла ли ошибка.</span><span class="sxs-lookup"><span data-stu-id="bdd0a-167">The [response XML](http://msdn.microsoft.com/library/93e44690-be2d-4fdb-96a8-4ded3c193aed%28Office.15%29.aspx) is simple and indicates whether the delete request was a success or whether an error occurred.</span></span> 
  
## <a name="see-also"></a><span data-ttu-id="bdd0a-168">См. также</span><span class="sxs-lookup"><span data-stu-id="bdd0a-168">See also</span></span>

- [<span data-ttu-id="bdd0a-169">Параметры сохраняемого приложения в веб-службах Exchange</span><span class="sxs-lookup"><span data-stu-id="bdd0a-169">Persistent application settings in EWS in Exchange</span></span>](persistent-application-settings-in-ews-in-exchange.md)
- [<span data-ttu-id="bdd0a-170">Общие сведения о разработке клиента EWS для Exchange</span><span class="sxs-lookup"><span data-stu-id="bdd0a-170">EWS client design overview for Exchange</span></span>](ews-client-design-overview-for-exchange.md)   
- [<span data-ttu-id="bdd0a-171">Разработка клиентов веб-служб для Exchange</span><span class="sxs-lookup"><span data-stu-id="bdd0a-171">Develop web service clients for Exchange</span></span>](develop-web-service-clients-for-exchange.md)
    

