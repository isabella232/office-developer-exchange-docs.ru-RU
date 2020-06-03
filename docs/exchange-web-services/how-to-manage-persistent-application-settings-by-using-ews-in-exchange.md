---
title: Управление параметрами сохраняемого приложения с помощью EWS в Exchange
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
localization_priority: Normal
ms.assetid: 90f561f2-e40e-4f5b-b321-f86dbf4a1b71
description: Узнайте, как создавать, искать, получать, обновлять и удалять параметры сохраняемого приложения с помощью управляемого API EWS или EWS в Exchange.
ms.openlocfilehash: ab7b3ef5f87d8a26a412ca7187dc93c58d73112f
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/03/2020
ms.locfileid: "44455732"
---
# <a name="manage-persistent-application-settings-by-using-ews-in-exchange"></a>Управление параметрами сохраняемого приложения с помощью EWS в Exchange

Узнайте, как создавать, искать, получать, обновлять и удалять параметры сохраняемого приложения с помощью управляемого API EWS или EWS в Exchange. 
  
Объекты конфигурации пользователя — это оптимальный способ хранения параметров конфигурации для клиентского приложения Exchange, в основном потому, что они скрыты от результатов поиска в большинстве клиентских приложений. Как правило, клиентские приложения скрывают эти параметры, так как конечный пользователь не видит их, а пользователь случайно не получает доступ к этой информации. В примерах кода, приведенных в этой статье, показано, как можно использовать объекты конфигурации пользователей для управления сохраняемыми параметрами, включая создание, поиск, получение, обновление и удаление параметров постоянного приложения, хранящихся в пользовательских объектах конфигурации.

<a name="createconfiguration"> </a>

## <a name="create-an-application-setting-by-using-the-ews-managed-api"></a>Создание параметра приложения с помощью управляемого API EWS

Для создания настраиваемого параметра конфигурации можно использовать метод [усерконфигуратион. Save](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.userconfiguration.save%28v=exchg.80%29.aspx) для управляемого API EWS. Объект конфигурации пользователя может содержать XML-файл, двоичный код, словарь данных или сочетание этих трех типов данных. В приведенном ниже примере показано, как сохранить объект конфигурации пользователя с именем Контосодрафтсеттингс, который содержит двоичные данные в папке "Черновики", с помощью управляемого API EWS. Это может быть полезно, если вы хотите хранить сведения о конфигурации для отображения элементов черновиков в клиентском приложении. 
  
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

## <a name="create-an-application-setting-by-using-ews"></a>Создание параметра приложения с помощью EWS
<a name="bk_createEWS"> </a>

Для создания настраиваемых параметров конфигурации можно использовать операцию [CreateUserConfiguration](https://msdn.microsoft.com/library/eb5b8ab6-9743-481c-aac9-f9aa889bd353%28Office.15%29.aspx) EWS. В следующем примере показан XML-код запроса для создания объекта конфигурации пользователя с именем Контосодрафтсеттингс. Запрос пытается сохранить двоичный поток в объект конфигурации пользователя в папке "Черновики". Это тот же XML-код, который создается в примере управляемого API EWS. 
  
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

[ОТКЛИК XML](https://msdn.microsoft.com/library/eb5b8ab6-9743-481c-aac9-f9aa889bd353%28Office.15%29.aspx) является простым и указывает, был ли запрос на создание успешным или возникла ошибка. 
  
## <a name="find-an-application-setting-by-using-the-ews-managed-api"></a>Поиск параметра приложения с помощью управляемого API EWS
<a name="findconfiguration"> </a>

Для поиска объектов конфигурации пользователя можно использовать метод Managed API [Folder. FindItems](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.folder.finditems%28v=exchg.80%29.aspx) EWS с соответствующим параметром обхода. В приведенном ниже примере кода показано, как найти объекты конфигурации пользователя, хранящиеся в папке "Черновики", с помощью управляемого API EWS. 
  
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

## <a name="find-an-application-setting-by-using-ews"></a>Поиск параметров приложения с помощью EWS
<a name="bk_findEWS"> </a>

Для поиска объектов конфигурации пользователя можно использовать операцию [FindItem](https://msdn.microsoft.com/library/ebad6aae-16e7-44de-ae63-a95b24539729%28Office.15%29.aspx) EWS. 
  
В следующем примере показан XML-код запроса для поиска объектов конфигурации пользователя. Это тот же XML-код, который создается в примере управляемого API EWS.
  
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

В следующем примере показан успешный XML-код ответа для поиска объектов конфигурации пользователя. Это тот же XML-код, который обрабатывается в примере управляемого API EWS. Обратите внимание на следующее в этом ответе XML: 
  
- Мы сократили идентификатор и изменили ключи для удобочитаемости.
    
- Два объекта конфигурации пользователя возвращаются в виде сообщений. Это связано с тем, что операция **FindItem** возвращает все элементы, не определенные в схеме EWS в виде элементов сообщения. 
    
- Свойства [ItemClass](https://msdn.microsoft.com/library/56020078-50b4-4880-894a-a9f234033cfb%28Office.15%29.aspx) для двух объектов конфигурации пользователей отличаются. Первый объект конфигурации пользователя был создан с помощью EWS. Второй объект был создан другим API. 
    
```XML
<?xml version="1.0" encoding="utf-8"?>
<s:Envelope xmlns:s="https://schemas.xmlsoap.org/soap/envelope/">
  <s:Header>
    <h:ServerVersionInfo MajorVersion="15" 
                         MinorVersion="0" 
                         MajorBuildNumber="800" 
                         MinorBuildNumber="5" 
                         Version="V2_6" 
                         xmlns:h="https://schemas.microsoft.com/exchange/services/2006/types" 
                         xmlns="https://schemas.microsoft.com/exchange/services/2006/types" 
                         xmlns:xsd="http://www.w3.org/2001/XMLSchema" 
                         xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" />
  </s:Header>
  <s:Body xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" 
          xmlns:xsd="http://www.w3.org/2001/XMLSchema">
    <m:FindItemResponse xmlns:m="https://schemas.microsoft.com/exchange/services/2006/messages" 
                        xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types">
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

## <a name="get-and-update-application-settings-by-using-the-ews-managed-api"></a>Получение и обновление параметров приложения с помощью управляемого API EWS
<a name="getconfiguration"> </a>

Найдя объект конфигурации пользователя, вы можете использовать метод управляемого API [усерконфигуратион. Bind](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.userconfiguration.bind%28v=exchg.80%29.aspx) EWS, чтобы получить объект Configuration из почтового ящика. После получения объекта Configuration можно использовать метод [усерконфигуратион. Update](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.userconfiguration.bind%28v=exchg.80%29.aspx) , чтобы обновить его. В приведенном ниже примере показано, как получить и обновить объект конфигурации пользователя с помощью управляемого API EWS. 
  
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

## <a name="get-and-update-application-settings-by-using-ews"></a>Получение и обновление параметров приложения с помощью EWS
<a name="bk_getEWS"> </a>

С помощью операции [GetUserConfiguration](https://msdn.microsoft.com/library/71d50e3c-92bd-435f-8118-b28bb85f8138%28Office.15%29.aspx) EWS можно получить объект конфигурации из почтового ящика и [UpdateUserConfiguration](https://msdn.microsoft.com/library/eda73b62-6a3a-43ae-8fd9-f30892811f27%28Office.15%29.aspx) для обновления объекта. В следующем примере показан XML-код запроса для получения объекта конфигурации пользователя с именем Тестконфиг. Запрос утверждает, что все конфигурации должны быть возвращены в ответе. Это тот же XML-код, который создается в примере управляемого API EWS. 
  
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
    <m:GetUserConfiguration>
      <m:UserConfigurationName Name="TestConfig">
        <t:DistinguishedFolderId Id="drafts" />
      </m:UserConfigurationName>
      <m:UserConfigurationProperties>All</m:UserConfigurationProperties>
    </m:GetUserConfiguration>
  </soap:Body>
</soap:Envelope>
```

В следующем примере показан успешный XML-код отклика для возврата объектов конфигурации пользователя. Ответ содержит словарь данных. Это тот же XML-код, который обрабатывается в примере управляемого API EWS. 
  
```XML
<?xml version="1.0" encoding="utf-8"?>
<s:Envelope xmlns:s="https://schemas.xmlsoap.org/soap/envelope/">
  <s:Header>
    <h:ServerVersionInfo MajorVersion="15" 
                         MinorVersion="0" 
                         MajorBuildNumber="800" 
                         MinorBuildNumber="5" 
                         Version="V2_6" 
                         xmlns:h="https://schemas.microsoft.com/exchange/services/2006/types" 
                         xmlns="https://schemas.microsoft.com/exchange/services/2006/types" 
                         xmlns:xsd="http://www.w3.org/2001/XMLSchema" 
                         xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" />
  </s:Header>
  <s:Body xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" 
          xmlns:xsd="http://www.w3.org/2001/XMLSchema">
    <m:GetUserConfigurationResponse xmlns:m="https://schemas.microsoft.com/exchange/services/2006/messages" 
                                    xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types">
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

В следующем примере показан XML-код запроса для обновления объекта конфигурации пользователя. Запрос утверждает, что все конфигурации должны быть возвращены в ответе. Это тот же XML-код, который создается с помощью управляемого API EWS в примере, в котором вызывается метод **усерконфигуратион. Update** . Вы видите, что XML-файл обновления содержит существующие записи словаря и дополнительный, добавленный перед обновлением. 
  
```xml
<?xml version="1.0" encoding="utf-8"?>
<soap:Envelope xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" 
               xmlns:m="https://schemas.microsoft.com/exchange/services/2006/messages" 
               xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types" 
               xmlns:soap="https://schemas.xmlsoap.org/soap/envelope/">
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

[ОТКЛИК XML](https://msdn.microsoft.com/library/eda73b62-6a3a-43ae-8fd9-f30892811f27%28Office.15%29.aspx) является простым и указывает, было ли обновление успешным или произошла ошибка. 
  
## <a name="delete-an-application-setting-by-using-the-ews-managed-api"></a>Удаление параметра приложения с помощью управляемого API EWS
<a name="deleteconfiguration"> </a>

Для удаления объектов конфигурации пользователя можно использовать метод [усерконфигуратион. Delete](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.userconfiguration.delete%28v=exchg.80%29.aspx) для управляемого API EWS. В приведенном ниже примере кода показано, как удалить объект конфигурации пользователя Контосодрафтсеттингс с помощью управляемого API EWS. 
  
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

## <a name="delete-an-application-setting-by-using-ews"></a>Удаление параметра приложения с помощью EWS
<a name="bk_deleteEWS"> </a>

Для удаления объектов конфигурации пользователя можно использовать операцию [DeleteUserConfiguration](https://msdn.microsoft.com/library/93e44690-be2d-4fdb-96a8-4ded3c193aed%28Office.15%29.aspx) EWS. 
  
В следующем примере показан XML-код запроса для удаления объекта конфигурации пользователя с именем Контосодрафтсеттингс, который был применен к папке "Черновики". Это тот же XML-код, который создается в примере управляемого API EWS.
  
```xml
<?xml version="1.0" encoding="utf-8"?>
<soap:Envelope xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" 
               xmlns:m="https://schemas.microsoft.com/exchange/services/2006/messages" 
               xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types" 
               xmlns:soap="https://schemas.xmlsoap.org/soap/envelope/">
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

[XML-код отклика](https://msdn.microsoft.com/library/93e44690-be2d-4fdb-96a8-4ded3c193aed%28Office.15%29.aspx) прост и указывает, был ли запрос на удаление успешным, или возникла ли ошибка. 
  
## <a name="see-also"></a>См. также

- [Параметры сохраняемого приложения в веб-службах Exchange](persistent-application-settings-in-ews-in-exchange.md)
- [Общие сведения о разработке клиента EWS для Exchange](ews-client-design-overview-for-exchange.md)   
- [Разработка клиентов веб-служб для Exchange](develop-web-service-clients-for-exchange.md)
    

