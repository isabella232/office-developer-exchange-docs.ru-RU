---
title: Работа с скрытые папки с помощью веб-служб Exchange в Exchange
manager: sethgros
ms.date: 03/9/2015
ms.audience: Developer
localization_priority: Normal
ms.assetid: 7ae7c045-cd90-4c9f-baf5-0464d5058f45
description: Узнайте, как сделать папку скрытые и поиск скрытых папок с помощью управляемого интерфейса API веб-служб Exchange или веб-служб Exchange в Exchange.
ms.openlocfilehash: 72efc16ecc247d307b7300526e7d345fe6bdd3ac
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/11/2018
ms.locfileid: "19761136"
---
# <a name="work-with-hidden-folders-by-using-ews-in-exchange"></a>Работа с скрытые папки с помощью веб-служб Exchange в Exchange

Узнайте, как сделать папку скрытые и поиск скрытых папок с помощью управляемого интерфейса API веб-служб Exchange или веб-служб Exchange в Exchange.
  
Одно исключение папок в корневой папки почтового ящика Exchange (не являющиеся IPM поддерево) скрыты от пользователя. С другой стороны всех папок в **MsgFolderRoot** (поддерева IPM) отображаются для пользователя. Так как скрыть папку в разделе **MsgFolderRoot**? Это не то непросто — все сводится к только что одно свойство, [PidTagAttributeHidden](http://msdn.microsoft.com/en-us/library/cc433490%28v=exchg.80%29.aspx) (0x10F4000B) расширенные свойства. Если этому свойству присвоено **значение true**, Outlook или другой клиент, который использует свойство для определения видимости папки будет скрыть папку из представления пользователя. Так как расширенные свойства, более сложных по сравнению с свойство среднее папки, поэтому в этой статье, следуя инструкциям основные сценарии.
  
**В таблице 1. Управляемый API EWS методы и операции веб-служб Exchange для работы с скрытые папки**

|**Задача**|**Метод управляемого API EWS**|**Операция служб EWS**|
|:-----|:-----|:-----|
|Скрыть папку  <br/> |[Folder.Bind](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.folder.bind%28v=exchg.80%29.aspx) , а затем [Folder.Update](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.folder.update%28v=exchg.80%29.aspx) <br/> |[GetFolder](http://msdn.microsoft.com/library/355bcf93-dc71-4493-b177-622afac5fdb9%28Office.15%29.aspx) следуют [UpdateFolder](http://msdn.microsoft.com/library/3494c996-b834-4813-b1ca-d99642d8b4e7%28Office.15%29.aspx) <br/> |
|Найти скрытые папки  <br/> |[FindFolders](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.exchangeservice.findfolders%28v=exchg.80%29.aspx) <br/> |[FindFolder](http://msdn.microsoft.com/library/7a9855aa-06cc-45ba-ad2a-645c15b7d031%28Office.15%29.aspx) <br/> |
   
Вы не знаете, что такое одно исключение — то есть, какие папки в корне ОТОБРАЖАЕТСЯ для пользователей? Это папка Finder (также известной как значение перечисления **SearchFolders**[WellKnownFolder](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.wellknownfoldername%28v=exchg.80%29.aspx) , или значение элемента[DistinguishedFolderId](http://msdn.microsoft.com/library/50018162-2941-4227-8a5b-d6b4686bb32f%28Office.15%29.aspx) **searchfolders**), содержащая папки поиска пользователей. Папки поиска, созданные в папке поиска отображаются для пользователей Outlook. Если вам нужно создать папку поиска, которая не отображается для пользователей, переместите его в корневой папке, чтобы скрыть его. В отличие от других папок свойства **PidTagAttributeHidden** значение **true** будет скрывает папки поиска в папке поиска. 
  
## <a name="hide-a-folder-by-using-the-ews-managed-api"></a>Скрыть папку с помощью управляемого интерфейса API веб-служб Exchange
<a name="bk_hideewsma"> </a>

Можно [сделать существующую папку](how-to-work-with-folders-by-using-ews-in-exchange.md#bk_createfolderewsma) скрытые папки с помощью изменения [PidTagAttributeHidden](http://msdn.microsoft.com/en-us/library/cc433490%28v=exchg.80%29.aspx) расширенные свойства, значение **true**. Во-первых создание [определения расширенных свойств для свойства](properties-and-extended-properties-in-ews-in-exchange.md). Далее метод [привязки](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.folder.bind%28v=exchg.80%29.aspx) используется для получения в папку, а затем обновите значение свойства **PidTagAttributeHidden** имеет значение true, и использовать метод [Update](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.folder.update%28v=exchg.80%29.aspx) для сохранения изменений. 
  
В этом примере предполагается, что этой **службы** является допустимым [ExchangeService](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.exchangeservice%28v=exchg.80%29.aspx) , что пользователь прошел проверку подлинности на сервере Exchange и что **folderId** является допустимым [Folder.Id](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.folder.id%28v=exchg.80%29.aspx) , который указывает папку, чтобы скрыть объектов для владельца почтового ящика. 
  
```cs
private static void MakeHidden(FolderId folderId, ExchangeService service)
{
    // Create an extended property definition for the PidTagAttributeHidden property.
    ExtendedPropertyDefinition isHiddenProp = new ExtendedPropertyDefinition(0x10f4, MapiPropertyType.Boolean);
    PropertySet propSet = new PropertySet(isHiddenProp);
    // Bind to a folder and retrieve the PidTagAttributeHidden property.
    Folder folder = Folder.Bind(service, folderId, propSet);
    // Set the PidTagAttributeHidden property to true.
    folder.SetExtendedProperty(isHiddenProp, true);
    // Save the changes.
    folder.Update();
}
```

## <a name="hide-a-folder-by-using-ews"></a>Скрыть папку с помощью веб-служб Exchange
<a name="bk_hideews"> </a>

Можно использовать веб-служб Exchange [Убедитесь в существующей папке](how-to-work-with-folders-by-using-ews-in-exchange.md#bk_createfolderewsma) скрытые папки с помощью изменения [PidTagAttributeHidden](http://msdn.microsoft.com/en-us/library/cc433490%28v=exchg.80%29.aspx) расширенные свойства, значение **true**. Во-первых используйте операцию [GetFolder](http://msdn.microsoft.com/library/355bcf93-dc71-4493-b177-622afac5fdb9%28Office.15%29.aspx) для получения в папку, а затем извлечь свойство **PidTagAttributeHidden** , включая элемент [ExtendedFieldURI](http://msdn.microsoft.com/library/b3c6ea3a-9ead-44b9-9d99-64ecf12bde23%28Office.15%29.aspx) , а если задать значение **PropertyTag** , 4340 и **PropertyType **значение типа Boolean. 
  
Это также запроса XML, управляемый API EWS отправляет при использовании метода **привязки** для получения папки перед [внесением его скрытые папки](#bk_hideewsma).
  
Значение [FolderId](http://msdn.microsoft.com/library/00d14e3e-4365-4f21-8f88-eaeea73b9bf7%28Office.15%29.aspx) сокращение для удобства чтения. 
  
```XML
<?xml version="1.0" encoding="utf-8"?>
<soap:Envelope xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance"
               xmlns:m="http://schemas.microsoft.com/exchange/services/2006/messages"
               xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types"
               xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/">
  <soap:Header>
    <t:RequestServerVersion Version="Exchange2007_SP1" />
  </soap:Header>
  <soap:Body>
    <m:GetFolder>
      <m:FolderShape>
        <t:BaseShape>IdOnly</t:BaseShape>
        <t:AdditionalProperties>
          <t:ExtendedFieldURI PropertyTag="4340"
                              PropertyType="Boolean" />
        </t:AdditionalProperties>
      </m:FolderShape>
      <m:FolderIds>
        <t:FolderId Id="IQywAAAA==" />
      </m:FolderIds>
    </m:GetFolder>
  </soap:Body>
</soap:Envelope>
```

Сервер отвечает на запрос **GetFolder** [GetFolderResponse](http://msdn.microsoft.com/library/47abeec8-78dd-4297-8525-099174ec880d%28Office.15%29.aspx) сообщение, которое содержит значение элемента [ResponseCode](http://msdn.microsoft.com/library/4b84d670-74c9-4d6d-84e7-f0a9f76f0d93%28Office.15%29.aspx) **NoError**, это означает, что папка был успешно извлечен. Ответ также включает в себя [значение](http://msdn.microsoft.com/library/196278d4-5e77-4e0a-8af6-8ac065610510%28Office.15%29.aspx) для [ExtendedProperty](http://msdn.microsoft.com/library/f9701409-b620-4afe-b9ee-4c1e95507af7%28Office.15%29.aspx). В этом примере **значение** задано **значение false**, что означает, что папка в настоящее время не скрыто.
  
```XML
<?xml version="1.0" encoding="utf-8"?>
<s:Envelope xmlns:s="http://schemas.xmlsoap.org/soap/envelope/">
  <s:Header>
    <h:ServerVersionInfo MajorVersion="15"
                         MinorVersion="0"
                         MajorBuildNumber="898"
                         MinorBuildNumber="23"
                         Version="V2_10"
                         xmlns:h="http://schemas.microsoft.com/exchange/services/2006/types"
                         xmlns="http://schemas.microsoft.com/exchange/services/2006/types"
                         xmlns:xsd="http://www.w3.org/2001/XMLSchema"
                         xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" />
  </s:Header>
  <s:Body xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance"
          xmlns:xsd="http://www.w3.org/2001/XMLSchema">
    <m:GetFolderResponse xmlns:m="http://schemas.microsoft.com/exchange/services/2006/messages"
                         xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types">
      <m:ResponseMessages>
        <m:GetFolderResponseMessage ResponseClass="Success">
          <m:ResponseCode>NoError</m:ResponseCode>
          <m:Folders>
            <t:Folder>
              <t:FolderId Id="IQywAAAA=="
                          ChangeKey="AQAAABYAAAD32nSTjepyT63rYH17n9THAAAAABED" />
              <t:ExtendedProperty>
                <t:ExtendedFieldURI PropertyTag="0x10f4"
                                    PropertyType="Boolean" />
                <t:Value>false</t:Value>
              </t:ExtendedProperty>
            </t:Folder>
          </m:Folders>
        </m:GetFolderResponseMessage>
      </m:ResponseMessages>
    </m:GetFolderResponse>
  </s:Body>
</s:Envelope>
```

Чтобы изменить значение **ExtendedProperty** имеет значение true, с помощью операции [UpdateFolder](http://msdn.microsoft.com/library/3494c996-b834-4813-b1ca-d99642d8b4e7%28Office.15%29.aspx) . Включить элементы **ExtendedProperty**, **ExtendedFieldURI**и **значения** для **PidTagAttributeHidden** расширенные свойства, а значение элемент **Value** **значение true** скрыть папку. 
  
Это также запроса XML, управляемый API EWS отправляет при использовании метода **обновления** обновить папку можно [было скрытые папки](#bk_hideewsma).
  
```XML
<?xml version="1.0" encoding="utf-8"?>
<soap:Envelope xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance"
               xmlns:m="http://schemas.microsoft.com/exchange/services/2006/messages"
               xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types"
               xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/">
  <soap:Header>
    <t:RequestServerVersion Version="Exchange2007_SP1" />
  </soap:Header>
  <soap:Body>
    <m:UpdateFolder>
      <m:FolderChanges>
        <t:FolderChange>
          <t:FolderId Id="IQywAAAA=="
                      ChangeKey="AQAAABYAAAD32nSTjepyT63rYH17n9THAAAAABED" />
          <t:Updates>
            <t:SetFolderField>
              <t:ExtendedFieldURI PropertyTag="4340"
                                  PropertyType="Boolean" />
              <t:Folder>
                <t:ExtendedProperty>
                  <t:ExtendedFieldURI PropertyTag="4340"
                                      PropertyType="Boolean" />
                  <t:Value>true</t:Value>
                </t:ExtendedProperty>
              </t:Folder>
            </t:SetFolderField>
          </t:Updates>
        </t:FolderChange>
      </m:FolderChanges>
    </m:UpdateFolder>
  </soap:Body>
</soap:Envelope>
```

Сервер отвечает на запрос **UpdateFolder** с [UpdateFolderResponse](http://msdn.microsoft.com/library/31f47739-dc9c-46ba-9e3f-cce25dc85e6e%28Office.15%29.aspx) сообщения, которое содержит значение элемента [ResponseCode](http://msdn.microsoft.com/library/4b84d670-74c9-4d6d-84e7-f0a9f76f0d93%28Office.15%29.aspx) **NoError**, это означает, что папка обновлен успешно и теперь скрыта.
  
## <a name="find-all-hidden-folders-by-using-the-ews-managed-api"></a>Поиск всех скрытых папок с помощью управляемого интерфейса API веб-служб Exchange
<a name="bk_findhiddenewsma"> </a>

Можно найти все скрытые папки в родительской папке, создание [определения расширенных свойств](properties-and-extended-properties-in-ews-in-exchange.md) для **PidTagAttributeHidden** расширенные свойства и затем с помощью метода [FindFolders](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.exchangeservice.findfolders%28v=exchg.80%29.aspx) для поиска папок с ** PidTagAttributeHidden** значение, которое имеет значение **true**. В этом примере используется MsgFolderRoot, также известные как хранилища или поддерева IPM, что и родительская папка для поиска в разделе.
  
В этом примере предполагается, что эта **Служба** является допустимым объектом [ExchangeService](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.exchangeservice%28v=exchg.80%29.aspx) владельца почтового ящика, а пользователь прошел проверку подлинности на сервере Exchange. 
  
```cs
private static void FindHiddenFolders(ExchangeService service)
{
    // Create an extended property definition for the PidTagAttributeHidden property.
    ExtendedPropertyDefinition isHiddenProp = new ExtendedPropertyDefinition(0x10f4, MapiPropertyType.Boolean);
    // Create a folder view to retrieve up to 100 folders and 
    // retrieve only the PidTagAttributeHidden and the display name.
    FolderView folderView = new FolderView(100);
    folderView.PropertySet = new PropertySet(isHiddenProp, FolderSchema.DisplayName);
    // Indicate a Traversal value of Deep, so that all subfolders are retrieved.
    folderView.Traversal = FolderTraversal.Deep;
    // Find all hidden folders under the MsgFolderRoot.
    // This call results in a FindFolder call to EWS.
    FindFoldersResults findFolder = service.FindFolders(WellKnownFolderName.MsgFolderRoot,
            new SearchFilter.IsEqualTo(isHiddenProp, true), folderView);
    // Display the folder ID and display name of each hidden folder.
    foreach (Folder folder in findFolder)
    {
        Console.WriteLine("FolderId: {0}", folder.Id);
        Console.WriteLine("DisplayName: {0}", folder.DisplayName);
        Console.WriteLine("\r\n");
    }
}
```

## <a name="find-all-hidden-folders-by-using-ews"></a>Поиск всех скрытых папок с помощью веб-служб Exchange
<a name="bk_findhiddenews"> </a>

Можно использовать веб-служб Exchange для поиска всех скрытых папок в существующей папке путем вызова операции [FindFolder](http://msdn.microsoft.com/library/7a9855aa-06cc-45ba-ad2a-645c15b7d031%28Office.15%29.aspx) и поиск папок, [PidTagAttributeHidden](http://msdn.microsoft.com/en-us/library/cc433490%28v=exchg.80%29.aspx) расширенного свойства имеет значение **true**. Чтобы сделать это, включают [выражение IsEqualTo](http://msdn.microsoft.com/library/48e7e067-049c-4184-8026-071e6f558e8a%28Office.15%29.aspx)[ограничение](http://msdn.microsoft.com/library/77f19014-d112-4999-8e83-ecc32a117a73%28Office.15%29.aspx) , которое ищет элемент [ExtendedFieldURI](http://msdn.microsoft.com/library/b3c6ea3a-9ead-44b9-9d99-64ecf12bde23%28Office.15%29.aspx) для свойства **PidTagAttributeHidden** (значение **PropertyTag** , 4243 и значение Boolean, **PropertyType** ) как показано в следующем запросе. В этом примере используется MsgFolderRoot, также известные как хранилища или поддерева IPM, что и родительская папка для поиска в разделе. 
  
Это также XML-запрос, который отправляет управляемый API EWS при использовании метода **FindFolders** для [поиска всех скрытых папок](#bk_findhiddenewsma).
  
```XML
<?xml version="1.0" encoding="utf-8"?>
<soap:Envelope xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance"
               xmlns:m="http://schemas.microsoft.com/exchange/services/2006/messages"
               xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types"
               xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/">
  <soap:Header>
    <t:RequestServerVersion Version="Exchange2007_SP1" />
    <t:TimeZoneContext>
      <t:TimeZoneDefinition Id="Central Standard Time" />
    </t:TimeZoneContext>
  </soap:Header>
  <soap:Body>
    <m:FindFolder Traversal="Deep">
      <m:FolderShape>
        <t:BaseShape>IdOnly</t:BaseShape>
        <t:AdditionalProperties>
          <t:ExtendedFieldURI PropertyTag="4340"
                              PropertyType="Boolean" />
          <t:FieldURI FieldURI="folder:DisplayName" />
        </t:AdditionalProperties>
      </m:FolderShape>
      <m:IndexedPageFolderView MaxEntriesReturned="100"
                               Offset="0"
                               BasePoint="Beginning" />
      <m:Restriction>
        <t:IsEqualTo>
          <t:ExtendedFieldURI PropertyTag="4340"
                              PropertyType="Boolean" />
          <t:FieldURIOrConstant>
            <t:Constant Value="true" />
          </t:FieldURIOrConstant>
        </t:IsEqualTo>
      </m:Restriction>
      <m:ParentFolderIds>
        <t:DistinguishedFolderId Id="msgfolderroot" />
      </m:ParentFolderIds>
    </m:FindFolder>
  </soap:Body>
</soap:Envelope>
```

Сервер отвечает на запрос **FindFolder** [FindFolderResponse](http://msdn.microsoft.com/library/f5dd813c-9698-4a39-8fca-3a825df365ed%28Office.15%29.aspx) сообщение, которое содержит значение элемента [ResponseCode](http://msdn.microsoft.com/library/4b84d670-74c9-4d6d-84e7-f0a9f76f0d93%28Office.15%29.aspx) **NoError**, это означает, что папка поиска прошла успешно, а также все скрытые папки в корневой папке сообщения.
  
Значения [FolderId](http://msdn.microsoft.com/library/00d14e3e-4365-4f21-8f88-eaeea73b9bf7%28Office.15%29.aspx) сокращаются для удобства чтения. 
  
```XML
<?xml version="1.0" encoding="utf-8"?>
<s:Envelope xmlns:s="http://schemas.xmlsoap.org/soap/envelope/">
  <s:Header>
    <h:ServerVersionInfo MajorVersion="15"
                         MinorVersion="0"
                         MajorBuildNumber="898"
                         MinorBuildNumber="23"
                         Version="V2_10"
                         xmlns:h="http://schemas.microsoft.com/exchange/services/2006/types"
                         xmlns="http://schemas.microsoft.com/exchange/services/2006/types"
                         xmlns:xsd="http://www.w3.org/2001/XMLSchema"
                         xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" />
  </s:Header>
  <s:Body xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance"
          xmlns:xsd="http://www.w3.org/2001/XMLSchema">
    <m:FindFolderResponse xmlns:m="http://schemas.microsoft.com/exchange/services/2006/messages"
                          xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types">
      <m:ResponseMessages>
        <m:FindFolderResponseMessage ResponseClass="Success">
          <m:ResponseCode>NoError</m:ResponseCode>
          <m:RootFolder IndexedPagingOffset="6"
                        TotalItemsInView="6"
                        IncludesLastItemInRange="true">
            <t:Folders>
              <t:ContactsFolder>
                <t:FolderId Id="IBHgAAAA=="
                            ChangeKey="AwAAABYAAAD32nSTjepyT63rYH17n9THAAAAAACz" />
                <t:DisplayName>{06967759-274D-40B2-A3EB-D7F9E73727D7}</t:DisplayName>
                <t:ExtendedProperty>
                  <t:ExtendedFieldURI PropertyTag="0x10f4"
                                      PropertyType="Boolean" />
                  <t:Value>true</t:Value>
                </t:ExtendedProperty>
              </t:ContactsFolder>
              <t:ContactsFolder>
                <t:FolderId Id="IBHwAAAA=="
                            ChangeKey="AwAAABYAAAD32nSTjepyT63rYH17n9THAAAAAAC7" />
                <t:DisplayName>{A9E2BC46-B3A0-4243-B315-60D991004455}</t:DisplayName>
                <t:ExtendedProperty>
                  <t:ExtendedFieldURI PropertyTag="0x10f4"
                                      PropertyType="Boolean" />
                  <t:Value>true</t:Value>
                </t:ExtendedProperty>
              </t:ContactsFolder>
              <t:ContactsFolder>
                <t:FolderId Id="IBIQAAAA=="
                            ChangeKey="AwAAABYAAAD32nSTjepyT63rYH17n9THAAAAAADO" />
                <t:DisplayName>GAL Contacts</t:DisplayName>
                <t:ExtendedProperty>
                  <t:ExtendedFieldURI PropertyTag="0x10f4"
                                      PropertyType="Boolean" />
                  <t:Value>true</t:Value>
                </t:ExtendedProperty>
              </t:ContactsFolder>
              <t:ContactsFolder>
                <t:FolderId Id="IBHQAAAA=="
                            ChangeKey="AwAAABYAAAD32nSTjepyT63rYH17n9THAAAAAACa" />
                <t:DisplayName>Recipient Cache</t:DisplayName>
                <t:ExtendedProperty>
                  <t:ExtendedFieldURI PropertyTag="0x10f4"
                                      PropertyType="Boolean" />
                  <t:Value>true</t:Value>
                </t:ExtendedProperty>
              </t:ContactsFolder>
              <t:Folder>
                <t:FolderId Id="HAAAAA=="
                            ChangeKey="AQAAABYAAAD32nSTjepyT63rYH17n9THAAAAAACS" />
                <t:DisplayName>Conversation Action Settings</t:DisplayName>
                <t:ExtendedProperty>
                  <t:ExtendedFieldURI PropertyTag="0x10f4"
                                      PropertyType="Boolean" />
                  <t:Value>true</t:Value>
                </t:ExtendedProperty>
              </t:Folder>
              <t:Folder>
                <t:FolderId Id="IQywAAAA=="
                            ChangeKey="AQAAABYAAAD32nSTjepyT63rYH17n9THAAAeZIBf" />
                <t:DisplayName>TestFolder</t:DisplayName>
                <t:ExtendedProperty>
                  <t:ExtendedFieldURI PropertyTag="0x10f4"
                                      PropertyType="Boolean" />
                  <t:Value>true</t:Value>
                </t:ExtendedProperty>
              </t:Folder>
            </t:Folders>
          </m:RootFolder>
        </m:FindFolderResponseMessage>
      </m:ResponseMessages>
    </m:FindFolderResponse>
  </s:Body>
</s:Envelope>
```

## 
<a name="bk_findhiddenews"> </a>

После того, как скрытые или не скрытым папок может потребоваться получение иерархии папок или [синхронизации иерархии папок](how-to-synchronize-folders-by-using-ews-in-exchange.md). Примеры, которые показывают, что вы как для [получения иерархии папок с помощью управляемого интерфейса API веб-служб Exchange](how-to-work-with-folders-by-using-ews-in-exchange.md#bk_getfolderhierarchyewsma) или [Получение иерархии папок с помощью веб-служб Exchange](how-to-work-with-folders-by-using-ews-in-exchange.md#bk_getfolderhierarchyews) также указать, какие папки в иерархии являются скрытыми. 
  
## <a name="see-also"></a>См. также


- [Папки и элементы в веб-службах Exchange](folders-and-items-in-ews-in-exchange.md)
    
- [Работа с папками с помощью веб-служб Exchange в Exchange](how-to-work-with-folders-by-using-ews-in-exchange.md)
    
- [Работа с папками поиска с помощью веб-служб Exchange в Exchange](how-to-work-with-search-folders-by-using-ews-in-exchange.md)
    

