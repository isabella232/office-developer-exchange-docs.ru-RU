---
title: Управление параметрами сохраняемого приложения с помощью веб-служб Exchange в Exchange
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
localization_priority: Normal
ms.assetid: 90f561f2-e40e-4f5b-b321-f86dbf4a1b71
description: Узнайте, как создать, найти, получение, обновления и удаления параметров сохраняемый приложения с помощью управляемого интерфейса API веб-служб Exchange или веб-служб Exchange в Exchange.
ms.openlocfilehash: ab5a9cc927bd0a6c4efacce622cc71db1a9b02a3
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/25/2018
ms.locfileid: "19761044"
---
# <a name="manage-persistent-application-settings-by-using-ews-in-exchange"></a><span data-ttu-id="364ab-103">Управление параметрами сохраняемого приложения с помощью веб-служб Exchange в Exchange</span><span class="sxs-lookup"><span data-stu-id="364ab-103">Manage persistent application settings by using EWS in Exchange</span></span>

<span data-ttu-id="364ab-104">Узнайте, как создать, найти, получение, обновления и удаления параметров сохраняемый приложения с помощью управляемого интерфейса API веб-служб Exchange или веб-служб Exchange в Exchange.</span><span class="sxs-lookup"><span data-stu-id="364ab-104">Learn how to create, find, get, update, and delete persistent application settings by using the EWS Managed API or EWS in Exchange.</span></span> 
  
<span data-ttu-id="364ab-105">Объектов конфигурации пользователя — лучший вариант для хранения параметров конфигурации для клиентского приложения Exchange, прежде всего, поскольку они являются скрытыми из результатов поиска в большинстве клиентских приложений.</span><span class="sxs-lookup"><span data-stu-id="364ab-105">User configuration objects are the best option for storing configuration settings for your Exchange client application, primarily because they are hidden from search results in most client applications.</span></span> <span data-ttu-id="364ab-106">Клиентские приложения обычно скрывать эти параметры, поскольку конечный пользователь не нужно просмотреть их и, чтобы не иметь доступ этот пользователь случайно эти сведения.</span><span class="sxs-lookup"><span data-stu-id="364ab-106">Client applications typically hide these settings because the end user doesn't need to see them, and so that the user doesn't accidentally access this information.</span></span> <span data-ttu-id="364ab-107">Примеры кода в этой статье показано, вы об использовании объектов конфигурации пользователя для управления постоянных параметров, включая создание, поиск, получение, обновление и удаление параметров сохраняемый приложения, которые хранятся в объектах конфигурации пользователя.</span><span class="sxs-lookup"><span data-stu-id="364ab-107">The code examples in this article show you how you can use user configuration objects to manage persistent settings, including how to create, find, get, update, and delete persistent application settings that are stored in user configuration objects.</span></span>

<span data-ttu-id="364ab-108"><a name="createconfiguration"> </a></span><span class="sxs-lookup"><span data-stu-id="364ab-108"></span></span>

## <a name="create-an-application-setting-by-using-the-ews-managed-api"></a><span data-ttu-id="364ab-109">Создание параметра приложения с помощью управляемого интерфейса API веб-служб Exchange</span><span class="sxs-lookup"><span data-stu-id="364ab-109">Create an application setting by using the EWS Managed API</span></span>

<span data-ttu-id="364ab-110">Можно использовать метод [UserConfiguration.Save](http://msdn.microsoft.com/ru-ru/library/microsoft.exchange.webservices.data.userconfiguration.save%28v=exchg.80%29.aspx) управляемый API веб-служб Exchange для создания настраиваемого параметра.</span><span class="sxs-lookup"><span data-stu-id="364ab-110">You can use the [UserConfiguration.Save](http://msdn.microsoft.com/ru-ru/library/microsoft.exchange.webservices.data.userconfiguration.save%28v=exchg.80%29.aspx) EWS Managed API method to create a custom configuration setting.</span></span> <span data-ttu-id="364ab-111">Объект конфигурации пользователя может содержать XML, двоичный, словарь данных или сочетание этих трех типов данных.</span><span class="sxs-lookup"><span data-stu-id="364ab-111">A user configuration object can contain XML, binary, a data dictionary, or a combination of those three data types.</span></span> <span data-ttu-id="364ab-112">Следующем примере показано, как сохранить объект конфигурации пользователя с именем ContosoDraftSettings, который содержит двоичные данные в папке «Черновики» с помощью управляемого интерфейса API веб-служб Exchange.</span><span class="sxs-lookup"><span data-stu-id="364ab-112">The following example shows how to save a user configuration object named ContosoDraftSettings that contains binary data to your Drafts folder by using the EWS Managed API.</span></span> <span data-ttu-id="364ab-113">Это может быть полезно использовать для хранения сведений о конфигурации о как черновики отображаются в клиентском приложении.</span><span class="sxs-lookup"><span data-stu-id="364ab-113">This might be useful if you want to store configuration information about how draft items are displayed in your client application.</span></span> 
  
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

## <a name="create-an-application-setting-by-using-ews"></a><span data-ttu-id="364ab-114">Создание параметра приложения с помощью веб-служб Exchange</span><span class="sxs-lookup"><span data-stu-id="364ab-114">Create an application setting by using EWS</span></span>
<span data-ttu-id="364ab-115"><a name="bk_createEWS"> </a></span><span class="sxs-lookup"><span data-stu-id="364ab-115"></span></span>

<span data-ttu-id="364ab-116">Можно использовать операцию [CreateUserConfiguration](http://msdn.microsoft.com/library/eb5b8ab6-9743-481c-aac9-f9aa889bd353%28Office.15%29.aspx) веб-служб Exchange для создания настраиваемого параметра.</span><span class="sxs-lookup"><span data-stu-id="364ab-116">You can use the [CreateUserConfiguration](http://msdn.microsoft.com/library/eb5b8ab6-9743-481c-aac9-f9aa889bd353%28Office.15%29.aspx) EWS operation to create a custom configuration setting.</span></span> <span data-ttu-id="364ab-117">В следующем примере показано запроса XML для создания объекта конфигурации пользователя с именем ContosoDraftSettings.</span><span class="sxs-lookup"><span data-stu-id="364ab-117">The following example shows the request XML for creating a user configuration object named ContosoDraftSettings.</span></span> <span data-ttu-id="364ab-118">Запрос пытается сохранить двоичный поток для объекта конфигурации пользователя в папке "Черновики".</span><span class="sxs-lookup"><span data-stu-id="364ab-118">The request attempts to save a binary stream to a user configuration object on the Drafts folder.</span></span> <span data-ttu-id="364ab-119">Это же XML-ФАЙЛ, созданный в примере управляемый API веб-служб Exchange.</span><span class="sxs-lookup"><span data-stu-id="364ab-119">This is the same XML that is generated by the EWS Managed API example.</span></span> 
  
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

<span data-ttu-id="364ab-120">[Ответ XML](http://msdn.microsoft.com/library/eb5b8ab6-9743-481c-aac9-f9aa889bd353%28Office.15%29.aspx) простой и указывает, является ли запрос создания прошла успешно или ли произошла ошибка.</span><span class="sxs-lookup"><span data-stu-id="364ab-120">The [response XML](http://msdn.microsoft.com/library/eb5b8ab6-9743-481c-aac9-f9aa889bd353%28Office.15%29.aspx) is simple and indicates whether the create request was successful or whether an error occurred.</span></span> 
  
## <a name="find-an-application-setting-by-using-the-ews-managed-api"></a><span data-ttu-id="364ab-121">Найдите параметр приложения с помощью управляемого интерфейса API веб-служб Exchange</span><span class="sxs-lookup"><span data-stu-id="364ab-121">Find an application setting by using the EWS Managed API</span></span>
<span data-ttu-id="364ab-122"><a name="findconfiguration"> </a></span><span class="sxs-lookup"><span data-stu-id="364ab-122"></span></span>

<span data-ttu-id="364ab-123">Можно использовать метод управляемый API EWS [Folder.FindItems](http://msdn.microsoft.com/ru-ru/library/microsoft.exchange.webservices.data.folder.finditems%28v=exchg.80%29.aspx) с параметром связанного обхода для поиска объектов конфигурации пользователей.</span><span class="sxs-lookup"><span data-stu-id="364ab-123">You can use the [Folder.FindItems](http://msdn.microsoft.com/ru-ru/library/microsoft.exchange.webservices.data.folder.finditems%28v=exchg.80%29.aspx) EWS Managed API method with the associated traversal option to find user configuration objects.</span></span> <span data-ttu-id="364ab-124">В следующем примере кода показано, как найти пользователя конфигурации, хранящихся в папке "Черновики" с помощью управляемого интерфейса API веб-служб Exchange.</span><span class="sxs-lookup"><span data-stu-id="364ab-124">The following code example shows you how to find user configuration objects stored on the Drafts folder by using the EWS Managed API.</span></span> 
  
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

## <a name="find-an-application-setting-by-using-ews"></a><span data-ttu-id="364ab-125">Найдите параметр приложения с помощью веб-служб Exchange</span><span class="sxs-lookup"><span data-stu-id="364ab-125">Find an application setting by using EWS</span></span>
<span data-ttu-id="364ab-126"><a name="bk_findEWS"> </a></span><span class="sxs-lookup"><span data-stu-id="364ab-126"></span></span>

<span data-ttu-id="364ab-127">Можно использовать операцию [FindItem](http://msdn.microsoft.com/library/ebad6aae-16e7-44de-ae63-a95b24539729%28Office.15%29.aspx) веб-служб Exchange для поиска объектов конфигурации пользователей.</span><span class="sxs-lookup"><span data-stu-id="364ab-127">You can use the [FindItem](http://msdn.microsoft.com/library/ebad6aae-16e7-44de-ae63-a95b24539729%28Office.15%29.aspx) EWS operation to find user configuration objects.</span></span> 
  
<span data-ttu-id="364ab-128">В следующем примере показано запроса XML для поиска пользователя объектов конфигурации.</span><span class="sxs-lookup"><span data-stu-id="364ab-128">The following example shows the request XML for finding user configuration objects.</span></span> <span data-ttu-id="364ab-129">Это же XML-ФАЙЛ, созданный в примере управляемый API веб-служб Exchange.</span><span class="sxs-lookup"><span data-stu-id="364ab-129">This is the same XML that is generated by the EWS Managed API example.</span></span>
  
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

<span data-ttu-id="364ab-130">В следующем примере показано успешного ответа XML для поиска пользователя объектов конфигурации.</span><span class="sxs-lookup"><span data-stu-id="364ab-130">The following example shows the successful response XML for finding user configuration objects.</span></span> <span data-ttu-id="364ab-131">Это же XML-кода, обрабатываемых в примере управляемый API веб-служб Exchange.</span><span class="sxs-lookup"><span data-stu-id="364ab-131">This is the same XML that is processed by the EWS Managed API example.</span></span> <span data-ttu-id="364ab-132">Обратите внимание на следующее в данном ответе XML.</span><span class="sxs-lookup"><span data-stu-id="364ab-132">Note the following in this response XML:</span></span> 
  
- <span data-ttu-id="364ab-133">Мы сокращение идентификатор и измените ключи для удобства чтения.</span><span class="sxs-lookup"><span data-stu-id="364ab-133">We shortened the identifier and change keys for readability.</span></span>
    
- <span data-ttu-id="364ab-134">Объекты конфигурации два пользователя возвращается в виде сообщения.</span><span class="sxs-lookup"><span data-stu-id="364ab-134">The two user configuration objects are returned as messages.</span></span> <span data-ttu-id="364ab-135">Это, так как операция **FindItem** возвращает все элементы, которые не определены в схеме веб-служб Exchange как элементы сообщения.</span><span class="sxs-lookup"><span data-stu-id="364ab-135">This is because the **FindItem** operation returns all items that are not defined in the EWS schema as message items.</span></span> 
    
- <span data-ttu-id="364ab-136">Свойства [ItemClass](http://msdn.microsoft.com/library/56020078-50b4-4880-894a-a9f234033cfb%28Office.15%29.aspx) для объектов конфигурации два пользователя не совпадают.</span><span class="sxs-lookup"><span data-stu-id="364ab-136">The [ItemClass](http://msdn.microsoft.com/library/56020078-50b4-4880-894a-a9f234033cfb%28Office.15%29.aspx) properties for the two user configuration objects are different.</span></span> <span data-ttu-id="364ab-137">Первый объект конфигурации пользователя был создан с помощью веб-служб Exchange.</span><span class="sxs-lookup"><span data-stu-id="364ab-137">The first user configuration object was created by using EWS.</span></span> <span data-ttu-id="364ab-138">Второй объект был создан с другой API.</span><span class="sxs-lookup"><span data-stu-id="364ab-138">The second object was created by another API.</span></span> 
    
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

## <a name="get-and-update-application-settings-by-using-the-ews-managed-api"></a><span data-ttu-id="364ab-139">Получение и обновление параметров приложения с помощью управляемого интерфейса API веб-служб Exchange</span><span class="sxs-lookup"><span data-stu-id="364ab-139">Get and update application settings by using the EWS Managed API</span></span>
<span data-ttu-id="364ab-140"><a name="getconfiguration"> </a></span><span class="sxs-lookup"><span data-stu-id="364ab-140"></span></span>

<span data-ttu-id="364ab-141">Найденный объект конфигурации пользователя, можно использовать метод [UserConfiguration.Bind](http://msdn.microsoft.com/ru-ru/library/microsoft.exchange.webservices.data.userconfiguration.bind%28v=exchg.80%29.aspx) управляемый API EWS для получения объекта конфигурации из почтового ящика.</span><span class="sxs-lookup"><span data-stu-id="364ab-141">After you find a user configuration object, you can use the [UserConfiguration.Bind](http://msdn.microsoft.com/ru-ru/library/microsoft.exchange.webservices.data.userconfiguration.bind%28v=exchg.80%29.aspx) EWS Managed API method to get the configuration object from the mailbox.</span></span> <span data-ttu-id="364ab-142">После получения объекта конфигурации, можно использовать метод [UserConfiguration.Update](http://msdn.microsoft.com/ru-ru/library/microsoft.exchange.webservices.data.userconfiguration.bind%28v=exchg.80%29.aspx) для его обновления.</span><span class="sxs-lookup"><span data-stu-id="364ab-142">After you get the configuration object, you can use the [UserConfiguration.Update](http://msdn.microsoft.com/ru-ru/library/microsoft.exchange.webservices.data.userconfiguration.bind%28v=exchg.80%29.aspx) method to update it.</span></span> <span data-ttu-id="364ab-143">Следующем примере показано, как получить и обновление объекта конфигурации пользователя с помощью управляемого интерфейса API веб-служб Exchange.</span><span class="sxs-lookup"><span data-stu-id="364ab-143">The following example shows how to get and update a user configuration object by using the EWS Managed API.</span></span> 
  
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

## <a name="get-and-update-application-settings-by-using-ews"></a><span data-ttu-id="364ab-144">Получение и обновление параметров приложения с помощью веб-служб Exchange</span><span class="sxs-lookup"><span data-stu-id="364ab-144">Get and update application settings by using EWS</span></span>
<span data-ttu-id="364ab-145"><a name="bk_getEWS"> </a></span><span class="sxs-lookup"><span data-stu-id="364ab-145"></span></span>

<span data-ttu-id="364ab-146">Можно использовать операцию [GetUserConfiguration](http://msdn.microsoft.com/library/71d50e3c-92bd-435f-8118-b28bb85f8138%28Office.15%29.aspx) веб-служб Exchange для получения объекта конфигурации из почтового ящика и [UpdateUserConfiguration](http://msdn.microsoft.com/library/eda73b62-6a3a-43ae-8fd9-f30892811f27%28Office.15%29.aspx) для обновления объекта.</span><span class="sxs-lookup"><span data-stu-id="364ab-146">You can use the [GetUserConfiguration](http://msdn.microsoft.com/library/71d50e3c-92bd-435f-8118-b28bb85f8138%28Office.15%29.aspx) EWS operation to retrieve the configuration object from the mailbox, and the [UpdateUserConfiguration](http://msdn.microsoft.com/library/eda73b62-6a3a-43ae-8fd9-f30892811f27%28Office.15%29.aspx) to update the object.</span></span> <span data-ttu-id="364ab-147">В следующем примере показано запроса XML для получения объекта конфигурации пользователя с именем TestConfig.</span><span class="sxs-lookup"><span data-stu-id="364ab-147">The following example shows the request XML for getting a user configuration object named TestConfig.</span></span> <span data-ttu-id="364ab-148">В запросе указывается, что все конфигурации должны быть возвращены в ответе.</span><span class="sxs-lookup"><span data-stu-id="364ab-148">The request states that all configurations should be returned in the response.</span></span> <span data-ttu-id="364ab-149">Это же XML-ФАЙЛ, созданный в примере управляемый API веб-служб Exchange.</span><span class="sxs-lookup"><span data-stu-id="364ab-149">This is the same XML that is generated by the EWS Managed API example.</span></span> 
  
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

<span data-ttu-id="364ab-150">В следующем примере показано успешного ответа XML для получения объектов конфигурации пользователя.</span><span class="sxs-lookup"><span data-stu-id="364ab-150">The following example shows the successful response XML for getting a user configuration objects.</span></span> <span data-ttu-id="364ab-151">Ответ содержит словарь данных.</span><span class="sxs-lookup"><span data-stu-id="364ab-151">The response contains a data dictionary.</span></span> <span data-ttu-id="364ab-152">Это же XML-кода, обрабатываемых в примере управляемый API веб-служб Exchange.</span><span class="sxs-lookup"><span data-stu-id="364ab-152">This is the same XML that is processed by the EWS Managed API example.</span></span> 
  
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

<span data-ttu-id="364ab-153">В следующем примере показано запроса XML для обновления объекта конфигурации пользователя.</span><span class="sxs-lookup"><span data-stu-id="364ab-153">The following example shows the request XML for updating a user configuration object.</span></span> <span data-ttu-id="364ab-154">В запросе указывается, что все конфигурации должны быть возвращены в ответе.</span><span class="sxs-lookup"><span data-stu-id="364ab-154">The request states that all configurations should be returned in the response.</span></span> <span data-ttu-id="364ab-155">Это же XML-ФАЙЛ, созданный в примере управляемый API EWS, вызывающий метод **UserConfiguration.Update** .</span><span class="sxs-lookup"><span data-stu-id="364ab-155">This is the same XML that is generated by the EWS Managed API example that calls the **UserConfiguration.Update** method.</span></span> <span data-ttu-id="364ab-156">Вы можете увидеть, что обновление XML содержит существующие записи словаря и дополнительные тот, который был добавлен перед обновлением.</span><span class="sxs-lookup"><span data-stu-id="364ab-156">You can see that the update XML contains the existing dictionary entries and the additional one that was added before the update.</span></span> 
  
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

<span data-ttu-id="364ab-157">[Ответ XML](http://msdn.microsoft.com/library/eda73b62-6a3a-43ae-8fd9-f30892811f27%28Office.15%29.aspx) простой и указывает, является ли обновление выполнено успешно или ли произошла ошибка.</span><span class="sxs-lookup"><span data-stu-id="364ab-157">The [response XML](http://msdn.microsoft.com/library/eda73b62-6a3a-43ae-8fd9-f30892811f27%28Office.15%29.aspx) is simple and indicates whether the update was successful or whether an error occurred.</span></span> 
  
## <a name="delete-an-application-setting-by-using-the-ews-managed-api"></a><span data-ttu-id="364ab-158">Удаление параметра приложения с помощью управляемого интерфейса API веб-служб Exchange</span><span class="sxs-lookup"><span data-stu-id="364ab-158">Delete an application setting by using the EWS Managed API</span></span>
<span data-ttu-id="364ab-159"><a name="deleteconfiguration"> </a></span><span class="sxs-lookup"><span data-stu-id="364ab-159"></span></span>

<span data-ttu-id="364ab-160">Можно использовать метод [UserConfiguration.Delete](http://msdn.microsoft.com/ru-ru/library/microsoft.exchange.webservices.data.userconfiguration.delete%28v=exchg.80%29.aspx) управляемый API веб-служб Exchange для удаления объектов конфигурации пользователей.</span><span class="sxs-lookup"><span data-stu-id="364ab-160">You can use the [UserConfiguration.Delete](http://msdn.microsoft.com/ru-ru/library/microsoft.exchange.webservices.data.userconfiguration.delete%28v=exchg.80%29.aspx) EWS Managed API method to delete user configuration objects.</span></span> <span data-ttu-id="364ab-161">В следующем примере кода показано, как удалить объект конфигурации ContosoDraftSettings пользователя с помощью управляемого интерфейса API веб-служб Exchange.</span><span class="sxs-lookup"><span data-stu-id="364ab-161">The following code example shows you how to delete the ContosoDraftSettings user configuration object by using the EWS Managed API.</span></span> 
  
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

## <a name="delete-an-application-setting-by-using-ews"></a><span data-ttu-id="364ab-162">Удаление параметра приложения с помощью веб-служб Exchange</span><span class="sxs-lookup"><span data-stu-id="364ab-162">Delete an application setting by using EWS</span></span>
<span data-ttu-id="364ab-163"><a name="bk_deleteEWS"> </a></span><span class="sxs-lookup"><span data-stu-id="364ab-163"></span></span>

<span data-ttu-id="364ab-164">Можно использовать операцию [DeleteUserConfiguration](http://msdn.microsoft.com/library/93e44690-be2d-4fdb-96a8-4ded3c193aed%28Office.15%29.aspx) веб-служб Exchange для удаления объектов конфигурации пользователей.</span><span class="sxs-lookup"><span data-stu-id="364ab-164">You can use the [DeleteUserConfiguration](http://msdn.microsoft.com/library/93e44690-be2d-4fdb-96a8-4ded3c193aed%28Office.15%29.aspx) EWS operation to delete user configuration objects.</span></span> 
  
<span data-ttu-id="364ab-165">В следующем примере показано запроса XML для удаления объекта конфигурации пользователя с именем ContosoDraftSettings, которая была применена к папке "Черновики".</span><span class="sxs-lookup"><span data-stu-id="364ab-165">The following example shows the request XML for deleting a user configuration object named ContosoDraftSettings that was applied to the Drafts folder.</span></span> <span data-ttu-id="364ab-166">Это же XML-ФАЙЛ, созданный в примере управляемый API веб-служб Exchange.</span><span class="sxs-lookup"><span data-stu-id="364ab-166">This is the same XML that is generated by the EWS Managed API example.</span></span>
  
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

<span data-ttu-id="364ab-167">[Ответ XML](http://msdn.microsoft.com/library/93e44690-be2d-4fdb-96a8-4ded3c193aed%28Office.15%29.aspx) простой и указывает, была ли запрос delete успешно или ли произошла ошибка.</span><span class="sxs-lookup"><span data-stu-id="364ab-167">The [response XML](http://msdn.microsoft.com/library/93e44690-be2d-4fdb-96a8-4ded3c193aed%28Office.15%29.aspx) is simple and indicates whether the delete request was a success or whether an error occurred.</span></span> 
  
## <a name="see-also"></a><span data-ttu-id="364ab-168">См. также</span><span class="sxs-lookup"><span data-stu-id="364ab-168">See also</span></span>

- [<span data-ttu-id="364ab-169">Параметры сохраняемого приложения в веб-службах Exchange</span><span class="sxs-lookup"><span data-stu-id="364ab-169">Persistent application settings in EWS in Exchange</span></span>](persistent-application-settings-in-ews-in-exchange.md)
- [<span data-ttu-id="364ab-170">Общие сведения о разработке клиента EWS для Exchange</span><span class="sxs-lookup"><span data-stu-id="364ab-170">EWS client design overview for Exchange</span></span>](ews-client-design-overview-for-exchange.md)   
- [<span data-ttu-id="364ab-171">Разработка клиентов веб-служб для Exchange</span><span class="sxs-lookup"><span data-stu-id="364ab-171">Develop web service clients for Exchange</span></span>](develop-web-service-clients-for-exchange.md)
    

