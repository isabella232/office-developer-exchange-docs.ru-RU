---
title: Работа с папками с помощью EWS в Exchange
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.assetid: 4b3eb746-74c4-42a0-aa2c-742c147f1871
description: Узнайте, как создавать, получать, обновлять и удалять папки с помощью управляемого API EWS или EWS в Exchange.
localization_priority: Priority
ms.openlocfilehash: a184d8da4d6949f01f47afc6a9fb7ed30729fd3b
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/03/2020
ms.locfileid: "44456383"
---
# <a name="work-with-folders-by-using-ews-in-exchange"></a>Работа с папками с помощью EWS в Exchange

Узнайте, как создавать, получать, обновлять и удалять папки с помощью управляемого API EWS или EWS в Exchange.
  
Для структурирования и упорядочивания почтовых ящиков в Exchange используются папки. Вы можете создавать новые, получать, обновлять и удалять папки с помощью управляемого API EWS или EWS. Каждый метод или операции, перечисленные в следующей таблице, выполняются для объекта [Folder](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.folder%28v=exchg.80%29.aspx) , типа [папки](https://msdn.microsoft.com/library/812948d8-c7db-45ce-bb3a-77233a53a974%28Office.15%29.aspx) или [одного из классов или типов производной папки](folders-and-items-in-ews-in-exchange.md#bk_folders).
  
**Таблица 1. Методы и операции для создания, возврата, обновления и удаления папок**

|**Задача**|**Метод управляемого API EWS**|**Операция EWS**|
|:-----|:-----|:-----|
|Создание папки  <br/> |[Folder. Save](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.folder.save%28v=exchg.80%29.aspx) <br/> |[CreateFolder](https://msdn.microsoft.com/library/6f6c334c-b190-4e55-8f0a-38f2a018d1b3%28Office.15%29.aspx) <br/> |
|Создание иерархии папок  <br/> |Недоступно  <br/> |[CreateFolderPath](https://msdn.microsoft.com/library/5a10aa5e-3f25-4ec3-a0b9-284c30918a1f%28Office.15%29.aspx) <br/> |
|Получение папки  <br/> |[Folder. Bind](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.folder.bind%28v=exchg.80%29.aspx) <br/> |[GetFolder](https://msdn.microsoft.com/library/355bcf93-dc71-4493-b177-622afac5fdb9%28Office.15%29.aspx) <br/> |
|Получение иерархии папок  <br/> |[Folder. Финдфолдерс](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.folder.findfolders%28v=exchg.80%29.aspx) <br/> |[FindFolder](https://msdn.microsoft.com/library/7a9855aa-06cc-45ba-ad2a-645c15b7d031%28Office.15%29.aspx) <br/> |
|Обновление папки  <br/> |[Folder. Update](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.folder.update%28v=exchg.80%29.aspx) <br/> |[UpdateFolder](https://msdn.microsoft.com/library/3494c996-b834-4813-b1ca-d99642d8b4e7%28Office.15%29.aspx) <br/> |
|Удаление папки  <br/> |[Folder. Delete](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.folder.delete%28v=exchg.80%29.aspx) <br/> |[DeleteFolder](https://msdn.microsoft.com/library/b0f92682-4895-4bcf-a4a1-e4c2e8403979%28Office.15%29.aspx) <br/> |

<a name="bk_createfolderewsma"> </a>

## <a name="create-a-folder-by-using-the-ews-managed-api"></a>Создание папки с помощью управляемого API EWS

В приведенном ниже примере кода показано, как использовать класс [Folder](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.folder%28v=exchg.80%29.aspx) для создания новой универсальной папки с [отображаемым именем](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.folder.displayname%28v=exchg.80%29.aspx) "Custom Folder" и значением свойства [фолдеркласс](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.folder.folderclass%28v=exchg.80%29.aspx) для платформы IPF. Ноте. Метод [Folder. Save](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.folder.save%28v=exchg.80%29.aspx) сохраняет папку в качестве дочерней папки папки "Входящие". 
  
В этих примерах предполагается, что **Служба** является допустимым объектом [ExchangeService](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.exchangeservice%28v=exchg.80%29.aspx) и что пользователь прошел проверку подлинности на сервере Exchange. 
  
```cs
// Create a custom folder.
Folder folder = new Folder(service);
folder.DisplayName = "Custom Folder";
folder.FolderClass = "IPF.Note";
// Save the folder as a child folder of the Inbox.
folder.Save(WellKnownFolderName.Inbox);
```

Чтобы создать папку другого типа, например, [календарфолдер](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.calendarfolder%28v=exchg.80%29.aspx), [контактсфолдер](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.contactsfolder%28v=exchg.80%29.aspx), [SearchFolder](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.searchfolder%28v=exchg.80%29.aspx)или [тасксфолдер](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.tasksfolder%28v=exchg.80%29.aspx), создайте новый экземпляр определенного класса (вместо универсального класса **папки** ) и не задавайте свойство **фолдеркласс** . Например, в приведенном ниже примере кода показано, как создать новый объект [тасксфолдер](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.tasksfolder%28v=exchg.80%29.aspx).
  
```cs
// Create a custom Tasks folder.
TasksFolder folder = new TasksFolder(service);
folder.DisplayName = "Custom Tasks";
// Save the folder as a child folder in the Inbox folder.
// This method call results in a CreateFolder call to EWS.
folder.Save(WellKnownFolderName.Inbox);
```

Если вы попытаетесь создать экземпляр определенного класса, а также задать свойство **фолдеркласс** , будет выдано сообщение об ошибке [еррорнофолдерклассоверриде](https://msdn.microsoft.com/library/exchangewebservices.responsecodetype%28v=exchg.80%29.aspx) . 
  
Обратите внимание, что вы не можете пакетно создавать несколько папок в рамках одного вызова метода с помощью управляемого API EWS.
  
## <a name="create-a-folder-by-using-ews"></a>Создание папки с помощью EWS
<a name="bk_createfolderews"> </a>

С помощью EWS можно создать одну папку или несколько папок.
  
Чтобы создать одну папку, отправьте сообщение запроса операции [CreateFolder](https://msdn.microsoft.com/library/6f6c334c-b190-4e55-8f0a-38f2a018d1b3%28Office.15%29.aspx) . Запрос операции **CreateFolder** указывает на то, что родительской папкой является папка "Входящие", [DisplayName](https://msdn.microsoft.com/library/e7efbbe1-6629-4d11-bed1-ed899e3f9d77%28Office.15%29.aspx) — "Custom Folder", а значение элемента [фолдеркласс](https://msdn.microsoft.com/library/0041d135-2869-4612-89a5-d1aa86aa1093%28Office.15%29.aspx) — IPF. Ноте. 
  
Это также запрос XML, который управляемый API EWS отправляет, когда вы создаете новую папку и вызываете метод [Folder. Save](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.folder.save%28v=exchg.80%29.aspx) . 
  
```XML
<?xml version="1.0" encoding="utf-8"?>
<soap:Envelope xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" 
               xmlns:m="https://schemas.microsoft.com/exchange/services/2006/messages"
               xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types"
               xmlns:soap="https://schemas.xmlsoap.org/soap/envelope/">
  <soap:Header>
    <t:RequestServerVersion Version="Exchange2007_SP1" />
  </soap:Header>
  <soap:Body>
    <m:CreateFolder>
      <m:ParentFolderId>
        <t:DistinguishedFolderId Id="inbox" />
      </m:ParentFolderId>
      <m:Folders>
        <t:Folder>
          <t:FolderClass>IPF.Note</t:FolderClass>
          <t:DisplayName>Custom Folder</t:DisplayName>
        </t:Folder>
      </m:Folders>
    </m:CreateFolder>
  </soap:Body>
</soap:Envelope>
```

Сервер отвечает на запрос **CreateFolder** с сообщением [креатефолдерреспонсе](https://msdn.microsoft.com/library/158adecc-491a-47d9-af73-acc2cd3f8566%28Office.15%29.aspx) , которое содержит значение [респонсекоде](https://msdn.microsoft.com/library/aa580757%28v=exchg.150%29.aspx) **, указывающее, что**папка была успешно создана, и [FolderId](https://msdn.microsoft.com/library/00d14e3e-4365-4f21-8f88-eaeea73b9bf7%28Office.15%29.aspx) созданного сообщения. 
  
Чтобы создать несколько папок, включите несколько элементов [Folder](https://msdn.microsoft.com/library/812948d8-c7db-45ce-bb3a-77233a53a974%28Office.15%29.aspx) в сообщение запроса операции **CreateFolder** . Все новые папки должны находиться в одной родительской папке. 
  
## <a name="create-a-folder-hierarchy-by-using-ews"></a>Создание иерархии папок с помощью EWS
<a name="bk_createfolderhierarchy"> </a>

Вы можете создать иерархию папок в едином вызове с помощью операции [CREATEFOLDERPATH](https://msdn.microsoft.com/library/5a10aa5e-3f25-4ec3-a0b9-284c30918a1f%28Office.15%29.aspx) EWS. Эта функция недоступна в управляемом API EWS. Вместо этого, если вы используете управляемый API EWS, вы можете создавать папки по одному, как показано в разделе [Создание папки с помощью EWS](#bk_createfolderews).
  
> [!NOTE]
> Управляемый API EWS не реализует эту функцию. 
  
## <a name="get-a-folder-by-using-the-ews-managed-api"></a>Получение папки с помощью управляемого API EWS
<a name="bk_getfolderewsma"> </a>

В приведенном ниже примере кода показано, как использовать метод [Folder. Bind](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.folder.bind%28v=exchg.80%29.aspx) для получения папки "Входящие". Рекомендуется ограничить возвращаемые свойства только теми, которые необходимы для вашего приложения. В этом примере показано, как ограничить возвращаемые свойства только свойством [ID](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.folder.id%28v=exchg.80%29.aspx) , создав объект набор [свойств](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.propertyset%28v=exchg.80%29.aspx) и применяя значение [идонли](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.basepropertyset%28v=exchg.80%29.aspx) к свойству [басепропертисет](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.propertyset.basepropertyset%28v=exchg.80%29.aspx) . 
  
В этом примере предполагается, что **служба** является действительным объектом [ExchangeService](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.exchangeservice%28v=exchg.80%29.aspx), и что пользователь прошел проверку подлинности на сервере Exchange server. 
  
```cs
// As a best practice, limit the properties returned to only those that are required.
// In this scenario, you only need the FolderId.
PropertySet propSet = new PropertySet(BasePropertySet.IdOnly);
// Bind to an existing folder and get only the properties specified in the PropertySet.
// This method call results in a GetFolder call to EWS.
Folder rootfolder = Folder.Bind(service, WellKnownFolderName.Inbox, propSet);
```

Если необходимо вернуть дополнительные свойства, добавьте свойства из класса [фолдерсчема](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.folderschema%28v=exchg.80%29.aspx) в набор **свойств**или используйте один из перегруженных методов [BIND](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.folder.bind%28v=exchg.80%29.aspx) , которые возвращают все свойства первого класса. 
  
Обратите внимание, что вы не можете получить несколько папок одновременно с помощью управляемого API EWS. Метод **BIND** необходимо вызывать отдельно для каждой папки. 
  
## <a name="get-a-folder-by-using-ews"></a>Получение папки с помощью EWS
<a name="bk_getfolderews"> </a>

С помощью EWS можно получить одну или несколько папок.
  
Чтобы получить одну папку, отправьте серверу сообщение с запросом на выполнение операции с [папкой](https://msdn.microsoft.com/library/355bcf93-dc71-4493-b177-622afac5fdb9%28Office.15%29.aspx) . В следующем примере для параметра [басешапе](https://msdn.microsoft.com/library/42c04f3b-abaa-4197-a3d6-d21677ffb1c0%28Office.15%29.aspx) задано значение **идонли**, поэтому возвращается только [FolderId](https://msdn.microsoft.com/library/00d14e3e-4365-4f21-8f88-eaeea73b9bf7%28Office.15%29.aspx) указанной папки. Элемент [фолдеридс](https://msdn.microsoft.com/library/3ff9d15a-7220-4785-ae6b-583a7eb82005%28Office.15%29.aspx) указывает, что извлекаемой папкой является папка "Входящие". 
  
Это также запрос XML, который управляемый API EWS отправляет при выполнении связывания с папкой с помощью метода [Folder. Bind](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.folder.bind%28v=exchg.80%29.aspx) . 
  
Чтобы получить несколько папок, включите несколько элементов [фолдеридс](https://msdn.microsoft.com/library/812948d8-c7db-45ce-bb3a-77233a53a974%28Office.15%29.aspx) в сообщение с запросом операции "операция с **папкой** ". 
  
```XML
<?xml version="1.0" encoding="utf-8"?>
<soap:Envelope xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" xmlns:m="https://schemas.microsoft.com/exchange/services/2006/messages" xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types" xmlns:soap="https://schemas.xmlsoap.org/soap/envelope/">
  <soap:Header>
    <t:RequestServerVersion Version="Exchange2007_SP1" />
  </soap:Header>
  <soap:Body>
    <m:GetFolder>
      <m:FolderShape>
        <t:BaseShape>IdOnly</t:BaseShape>
      </m:FolderShape>
      <m:FolderIds>
        <t:DistinguishedFolderId Id="inbox" />
      </m:FolderIds>
    </m:GetFolder>
  </soap:Body>
</soap:Envelope>
```

В следующем примере XML-кода показано сообщение [жетфолдерреспонсе](https://msdn.microsoft.com/library/47abeec8-78dd-4297-8525-099174ec880d%28Office.15%29.aspx) , которое отправляется от сервера клиенту в ответ на запрос операции- **папки** . Он содержит только значение [FolderId](https://msdn.microsoft.com/library/00d14e3e-4365-4f21-8f88-eaeea73b9bf7%28Office.15%29.aspx) папки "Входящие". Для удобства значения некоторых атрибутов и элементов были сокращены. 
  
```XML
<?xml version="1.0" encoding="utf-8"?>
<s:Envelope xmlns:s="https://schemas.xmlsoap.org/soap/envelope/">
  <s:Header>
    <h:ServerVersionInfo MajorVersion="15"
                         MinorVersion="0"
                         MajorBuildNumber="800"
                         MinorBuildNumber="16"
                         Version="V2_6"
                         xmlns:h="https://schemas.microsoft.com/exchange/services/2006/types"
                         xmlns="https://schemas.microsoft.com/exchange/services/2006/types"
                         xmlns:xsd="http://www.w3.org/2001/XMLSchema"
                         xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance"/>
  </s:Header>
  <s:Body xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance"
          xmlns:xsd="http://www.w3.org/2001/XMLSchema">
    <m:GetFolderResponse xmlns:m="https://schemas.microsoft.com/exchange/services/2006/messages"
                         xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types">
      <m:ResponseMessages>
        <m:GetFolderResponseMessage ResponseClass="Success">
          <m:ResponseCode>NoError</m:ResponseCode>
          <m:Folders>
            <t:Folder>
              <t:FolderId Id="AAAENAAA=" ChangeKey="AQAAABYAAAAPxolXAHv3TaHUnjW8wWqXAAAEkbCr"/>
            </t:Folder>
          </m:Folders>
        </m:GetFolderResponseMessage>
      </m:ResponseMessages>
    </m:GetFolderResponse>
  </s:Body>
</s:Envelope>
```

## <a name="get-a-folder-hierarchy-by-using-the-ews-managed-api"></a>Получение иерархии папок с помощью управляемого API EWS
<a name="bk_getfolderhierarchyewsma"> </a>

В приведенном ниже примере кода показано, как получить вложенные папки для указанной корневой папки. В этом примере извлекаются подпапки папки **мсгфолдеррут** , которая является корнем поддерева IPM (где хранятся папки и элементы почтовых ящиков). 
  
В этом примере создается объект класса [FolderView](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.folderview%28v=exchg.80%29.aspx) для ограничения результатов для ответа метода [Folder. финдфолдерс](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.folder.findfolders%28v=exchg.80%29.aspx) . В этом сценарии свойства возвращаются следующим образом: [ID](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.folder.id%28v=exchg.80%29.aspx), [DisplayName](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.folder.displayname%28v=exchg.80%29.aspx)и расширенное свойство, которое указывает, является ли эта папка скрытой. Задайте для свойства [FolderView. обход](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.folderview.traversal%28v=EXCHG.80%29.aspx) значение Deep, чтобы выполнить рекурсивный поиск, чтобы сервер возвращал подпапки, и присвойте корневому каталогу значение **мсгфолдеррут**, чтобы сервер возвращал все папки пользователя (а сервер не возвращал системные папки в поддереве без IPM).
  
В этом примере предполагается, что **служба** является действительным объектом [ExchangeService](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.exchangeservice%28v=exchg.80%29.aspx), и что пользователь прошел проверку подлинности на сервере Exchange server. 
  
```XML
// Create a new folder view, and pass in the maximum number of folders to return.
FolderView view = new FolderView(folderViewSize);
// Create an extended property definition for the PR_ATTR_HIDDEN property,
// so that your results will indicate whether the folder is a hidden folder.
ExtendedPropertyDefinition isHiddenProp = new ExtendedPropertyDefinition(0x10f4, MapiPropertyType.Boolean);
// As a best practice, limit the properties returned to only those required.
// In this case, return the folder ID, DisplayName, and the value of the isHiddenProp
// extended property.
view.PropertySet = new PropertySet(BasePropertySet.IdOnly, FolderSchema.DisplayName, isHiddenProp);
// Indicate a Traversal value of Deep, so that all subfolders are retrieved.
view.Traversal = FolderTraversal.Deep;
// Call FindFolders to retrieve the folder hierarchy, starting with the MsgFolderRoot folder.
// This method call results in a FindFolder call to EWS.
FindFoldersResults findFolderResults = service.FindFolders(WellKnownFolderName.MsgFolderRoot, view);
```

## <a name="get-a-folder-hierarchy-by-using-ews"></a>Получение иерархии папок с помощью EWS
<a name="bk_getfolderhierarchyews"> </a>

В следующих примерах XML показано, как использовать операцию [FindFolder](https://msdn.microsoft.com/library/7a9855aa-06cc-45ba-ad2a-645c15b7d031%28Office.15%29.aspx) для получения иерархии папок с помощью EWS. В этом примере показано получение папки **мсгфолдеррут** , которая является корнем поддерева IPM, и всех вложенных в нее папок. Атрибуту **прохождения** присвоено значение **Deep** , чтобы сервер выполнял рекурсивный поиск в иерархии папок и возвращал только папки и вложенные папки в указанном корне в ответе. В этом примере элемент [басешапе](https://msdn.microsoft.com/library/42c04f3b-abaa-4197-a3d6-d21677ffb1c0%28Office.15%29.aspx) имеет значение **идонли** , чтобы сервер возвращал только элемент [FolderId](https://msdn.microsoft.com/library/00d14e3e-4365-4f21-8f88-eaeea73b9bf7%28Office.15%29.aspx) . Чтобы легче было понять выходные данные, включите элемент **DisplayName** в результаты, включив его в элемент [аддитионалпропертиес](https://msdn.microsoft.com/library/7a269aed-dcfd-4c3e-9e14-094e53828101%28Office.15%29.aspx) в запросе вместе со значением **екстендедфиелдури** для свойства **PR_ATTR_HIDDEN** , чтобы узнать, являются ли папки скрытыми папками. 
  
Это также запрос XML, который управляемый API EWS отправляет при вызове метода [финдфолдерс](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.exchangeservice.findfolders%28v=exchg.80%29.aspx) . 
  
```XML
<?xml version="1.0" encoding="utf-8"?>
<soap:Envelope xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance"
               xmlns:m="https://schemas.microsoft.com/exchange/services/2006/messages"
               xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types"
               xmlns:soap="https://schemas.xmlsoap.org/soap/envelope/">
  <soap:Header>
    <t:RequestServerVersion Version="Exchange2007_SP1" />
  </soap:Header>
  <soap:Body>
    <m:FindFolder Traversal="Deep">
      <m:FolderShape>
        <t:BaseShape>IdOnly</t:BaseShape>
        <t:AdditionalProperties>
          <t:FieldURI FieldURI="folder:DisplayName" />
          <t:ExtendedFieldURI PropertyTag="4340"
                              PropertyType="Boolean" />
        </t:AdditionalProperties>
      </m:FolderShape>
      <m:IndexedPageFolderView MaxEntriesReturned="100"
                               Offset="0"
                               BasePoint="Beginning" />
      <m:ParentFolderIds>
        <t:DistinguishedFolderId Id="msgfolderroot" />
      </m:ParentFolderIds>
    </m:FindFolder>
  </soap:Body>
</soap:Envelope>
```

В следующем примере XML-кода показано сообщение [финдфолдерреспонсе](https://msdn.microsoft.com/library/f5dd813c-9698-4a39-8fca-3a825df365ed%28Office.15%29.aspx) , которое отправляется от сервера клиенту в ответ на запрос операции **FindFolder** . Он содержит только [FolderId](https://msdn.microsoft.com/library/00d14e3e-4365-4f21-8f88-eaeea73b9bf7%28Office.15%29.aspx), [DisplayName](https://msdn.microsoft.com/library/e7efbbe1-6629-4d11-bed1-ed899e3f9d77%28Office.15%29.aspx)и значение расширенного свойства **PR_ATTR_HIDDEN** для всех вложенных папок в папке **мсгрутфолдер** . Если для элемента [value](https://msdn.microsoft.com/library/9a30cadd-909e-41b1-b4e9-291643dd89c6%28Office.15%29.aspx) задано значение true, папка должна быть скрыта в клиентском представлении. 
  
Кроме того, это XML-ответ, который управляемый API EWS отправляет при получении нескольких папок с помощью метода [FindFolder](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.folder.findfolders%28v=exchg.80%29.aspx) . Значения некоторых атрибутов и элементов были сокращены для удобочитаемости, а некоторые папки не были включены для краткости. 
  
```XML
<?xml version="1.0" encoding="utf-8"?><s:Envelope xmlns:s="https://schemas.xmlsoap.org/soap/envelope/">
  <s:Header>
    <h:ServerVersionInfo MajorVersion="15"
                         MinorVersion="0"
                         MajorBuildNumber="815"
                         MinorBuildNumber="6"
                         Version="V2_7"
                         xmlns:h="https://schemas.microsoft.com/exchange/services/2006/types"
                         xmlns="https://schemas.microsoft.com/exchange/services/2006/types"
                         xmlns:xsd="http://www.w3.org/2001/XMLSchema"
                         xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance"/>
  </s:Header>
  <s:Body xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance"
          xmlns:xsd="http://www.w3.org/2001/XMLSchema">
    <m:FindFolderResponse xmlns:m="https://schemas.microsoft.com/exchange/services/2006/messages"
                          xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types">
      <m:ResponseMessages>
        <m:FindFolderResponseMessage ResponseClass="Success">
          <m:ResponseCode>NoError</m:ResponseCode>
          <m:RootFolder IndexedPagingOffset="16"
                        TotalItemsInView="16"
                        IncludesLastItemInRange="true">
            <t:Folders>
              <t:CalendarFolder>
                <t:FolderId Id="AAAEOAAA="
                            ChangeKey="AgAAABYAAAAPxolXAHv3TaHUnjW8wWqXAAAAAAA3"/>
                <t:DisplayName>Calendar</t:DisplayName>
                <t:ExtendedProperty>
                  <t:ExtendedFieldURI PropertyTag="0x10f4"
                                      PropertyType="Boolean"/>
                  <t:Value>false</t:Value>
                </t:ExtendedProperty>
              </t:CalendarFolder>
              <t:ContactsFolder>
                <t:FolderId Id="AAAEPAAA="
                            ChangeKey="AwAAABYAAAAPxolXAHv3TaHUnjW8wWqXAAAAAAA4"/>
                <t:DisplayName>Contacts</t:DisplayName>
                <t:ExtendedProperty>
                  <t:ExtendedFieldURI PropertyTag="0x10f4"
                                      PropertyType="Boolean"/>
                  <t:Value>false</t:Value>
                </t:ExtendedProperty>
              </t:ContactsFolder>
              <t:ContactsFolder>
                <t:FolderId Id="AAAUKAAA="
                            ChangeKey="AwAAABYAAAAPxolXAHv3TaHUnjW8wWqXAAAAAAS5"/>
                <t:DisplayName>Recipient Cache</t:DisplayName>
                <t:ExtendedProperty>
                  <t:ExtendedFieldURI PropertyTag="0x10f4"
                                      PropertyType="Boolean"/>
                  <t:Value>true</t:Value>
                </t:ExtendedProperty>
              </t:ContactsFolder>
              <t:Folder>
                <t:FolderId Id="AAAUJAAA="
                            ChangeKey="AQAAABYAAAAPxolXAHv3TaHUnjW8wWqXAAAAAASx"/>
                <t:DisplayName>Conversation Action Settings</t:DisplayName>
                <t:ExtendedProperty>
                  <t:ExtendedFieldURI PropertyTag="0x10f4"
                                      PropertyType="Boolean"/>
                  <t:Value>true</t:Value>
                </t:ExtendedProperty>
              </t:Folder>
…
            </t:Folders>
          </m:RootFolder>
        </m:FindFolderResponseMessage>
      </m:ResponseMessages>
    </m:FindFolderResponse>
  </s:Body>
</s:Envelope>
```

## <a name="update-a-folder-by-using-the-ews-managed-api"></a>Обновление папки с помощью управляемого API EWS
<a name="bk_updatefolderewsma"> </a>

В приведенном ниже примере кода показано, как обновить отображаемое имя папки с помощью управляемого API EWS.
  
Сначала создайте набор [свойств](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.propertyset%28v=exchg.80%29.aspx) , чтобы ограничить число свойств, возвращаемых сервером в ответе [Folder. Bind](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.folder.bind%28v=exchg.80%29.aspx) . Рекомендуется использовать **Басепропертисет** **идонли** для уменьшения числа вызовов к базе данных Exchange. Затем используйте метод **BIND** для связывания с папкой, которую требуется обновить. Затем обновите свойство [DisplayName](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.folder.displayname%28v=exchg.80%29.aspx) и используйте метод [Folder. Update](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.folder.update%28v=exchg.80%29.aspx) , чтобы сохранить изменения. 
  
В этом примере предполагается, что **Служба** является допустимым объектом [ExchangeService](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.exchangeservice%28v=exchg.80%29.aspx) и что пользователь прошел проверку подлинности на сервере Exchange. Локальная переменная *FolderId* — это [идентификатор](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.folder.id%28v=exchg.80%29.aspx) обновляемой папки. 
  
```cs
// As a best practice, only include the ID value in the PropertySet.
PropertySet propertySet = new PropertySet(BasePropertySet.IdOnly);
// Bind to an existing folder and get the FolderId.
// This method call results in a GetFolder call to EWS.
Folder folder = Folder.Bind(service, folderId, propertySet);
// Update the display name of the folder.
folder.DisplayName = "Updated folder name";
// Save the updates.
// This method call results in an UpdateFolder call to EWS.
folder.Update();

```

## <a name="update-a-folder-by-using-ews"></a>Обновление папки с помощью EWS
<a name="bk_updatefolderews"> </a>

В приведенных ниже примерах XML-кода показано, как обновить отображаемое имя папки с помощью EWS.
  
Сначала отправьте сообщение с запросом на выполнение операции с [папкой](https://msdn.microsoft.com/library/355bcf93-dc71-4493-b177-622afac5fdb9%28Office.15%29.aspx) , чтобы получить обновляемую папку, как показано в разделе [получение иерархии папок с помощью EWS](#bk_getfolderhierarchyews).
  
Затем отправьте серверу сообщение с запросом на выполнение операции [операцию UpdateFolder](https://msdn.microsoft.com/library/3494c996-b834-4813-b1ca-d99642d8b4e7%28Office.15%29.aspx) , чтобы обновить папку. Запрос операции **операцию UpdateFolder** обновляет [DisplayName](https://msdn.microsoft.com/library/42c04f3b-abaa-4197-a3d6-d21677ffb1c0%28Office.15%29.aspx) на "обновленную настраиваемую папку". 
  
Это также запрос XML, который отправляет управляемый API EWS при обновлении папки с помощью метода [Folder. Update](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.folder.update%28v=exchg.80%29.aspx) . Для удобства значения некоторых атрибутов и элементов были сокращены. 
  
```XML
<?xml version="1.0" encoding="utf-8"?>
<soap:Envelope xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" xmlns:m="https://schemas.microsoft.com/exchange/services/2006/messages" xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types" xmlns:soap="https://schemas.xmlsoap.org/soap/envelope/">
  <soap:Header>
    <t:RequestServerVersion Version="Exchange2007_SP1" />
  </soap:Header>
  <soap:Body>
    <m:UpdateFolder>
      <m:FolderChanges>
        <t:FolderChange>
          <t:FolderId Id="OrV9ZAAA=" ChangeKey="AQAAABYAAABVzRdyy/cHS4XTC9itCRdUAAAOrXWb" />
          <t:Updates>
            <t:SetFolderField>
              <t:FieldURI FieldURI="folder:DisplayName" />
              <t:Folder>
                <t:DisplayName>Updated Custom Folder</t:DisplayName>
              </t:Folder>
            </t:SetFolderField>
          </t:Updates>
        </t:FolderChange>
      </m:FolderChanges>
    </m:UpdateFolder>
  </soap:Body>
</soap:Envelope>
```

Сервер отвечает на запрос **операцию UpdateFolder** с сообщением [упдатефолдерреспонсе](https://msdn.microsoft.com/library/31f47739-dc9c-46ba-9e3f-cce25dc85e6e%28Office.15%29.aspx) , которое содержит значение [респонсекоде](https://msdn.microsoft.com/library/aa580757%28v=exchg.150%29.aspx) , равное **ошибке**, и [FolderId](https://msdn.microsoft.com/library/00d14e3e-4365-4f21-8f88-eaeea73b9bf7%28Office.15%29.aspx) папки, которая была обновлена с помощью обновленного значения атрибута **чанжекэй** . 
  
## <a name="delete-a-folder-by-using-the-ews-managed-api"></a>Удаление папки с помощью управляемого API EWS
<a name="bk_deletefolderewsma"> </a>

В этой статье представлен простой пример, в котором показано, как удалить папку с помощью управляемого API EWS. Более подробную информацию об удалении папок [можно узнать в статье Удаление элементов с помощью EWS в Exchange](deleting-items-by-using-ews-in-exchange.md).
  
Чтобы удалить папку с помощью управляемого API EWS, сначала используйте метод [Folder. Bind](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.folder.bind%28v=exchg.80%29.aspx) для связывания с объектом службы с удаляемой папкой. Затем используйте метод [Folder. Delete](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.folder.delete%28v=exchg.80%29.aspx) для удаления папки с помощью режима удаления [HardDelete](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.deletemode%28v=exchg.80%29.aspx) . 
  
В этом примере предполагается, что **служба** является действительным объектом [ExchangeService](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.exchangeservice%28v=exchg.80%29.aspx), и что пользователь прошел проверку подлинности на сервере Exchange server. Локальная переменная *FolderId* — [идентификатор](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.folder.id%28v=exchg.80%29.aspx) удаляемой папки. 
  
```cs
// Bind to an existing folder and get all its properties.
// This method call results in a GetFolder call to EWS.
Folder folder = Folder.Bind(service, folderId);
// HardDelete the folder.
// This method call results in a DeleteFolder call to EWS.
folder.Delete(DeleteMode.HardDelete);
```

## <a name="delete-a-folder-by-using-ews"></a>Удаление папки с помощью EWS
<a name="bk_deletefolderews"> </a>

В этой статье представлен базовый пример кода XML, в котором показано, как удалить папку с помощью EWS. Более подробную информацию об удалении папок [можно узнать в статье Удаление элементов с помощью EWS в Exchange](deleting-items-by-using-ews-in-exchange.md).
  
Чтобы удалить папку с помощью EWS, сначала отправьте сообщение с запросом операции "операция с [папкой](https://msdn.microsoft.com/library/355bcf93-dc71-4493-b177-622afac5fdb9%28Office.15%29.aspx) ", чтобы получить обновляемую папку, как показано в разделе [Получение папки с помощью EWS](#bk_getfolderews). 
  
Затем отправьте серверу запрос на получение сообщения об операции [DeleteFolder](https://msdn.microsoft.com/library/b0f92682-4895-4bcf-a4a1-e4c2e8403979%28Office.15%29.aspx) , чтобы удалить папку. Запрос операции **DeleteFolder** указывает на то, что **делететипе** является **HardDelete** и включает [FolderId](https://msdn.microsoft.com/library/00d14e3e-4365-4f21-8f88-eaeea73b9bf7%28Office.15%29.aspx) папки для удаления. 
  
Это также запрос XML, который отправляет управляемый API EWS при удалении папки с помощью метода [Folder. Delete](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.folder.delete%28v=exchg.80%29.aspx) . Для удобства значения некоторых атрибутов и элементов были сокращены. 
  
```XML
<?xml version="1.0" encoding="utf-8"?>
<soap:Envelope xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" 
               xmlns:m="https://schemas.microsoft.com/exchange/services/2006/messages" 
               xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types" 
               xmlns:soap="https://schemas.xmlsoap.org/soap/envelope/">
  <soap:Header>
    <t:RequestServerVersion Version="Exchange2007_SP1" />
  </soap:Header>
  <soap:Body>
    <m:DeleteFolder DeleteType="HardDelete">
      <m:FolderIds>
        <t:FolderId Id="OrV9ZAAA=" ChangeKey="AQAAABYAAABVzRdyy/cHS4XTC9itCRdUAAAOrXWf" />
      </m:FolderIds>
    </m:DeleteFolder>
  </soap:Body>
</soap:Envelope>
```

Сервер отвечает на запрос **DeleteFolder** с сообщением [делетефолдерреспонсе](https://msdn.microsoft.com/library/27578bda-ef0a-4a33-bccc-2c1bc1735424%28Office.15%29.aspx) , которое содержит значение [респонсекоде](https://msdn.microsoft.com/library/aa580757%28v=exchg.150%29.aspx) , равное **ошибке**, что указывает на то, что удаление папки прошло успешно.
  
## <a name="next-steps"></a>Дальнейшие действия
<a name="bk_nextsteps"> </a>

После получения папок на сервере или внесения изменений в папки может потребоваться [Синхронизация иерархии папок](how-to-synchronize-folders-by-using-ews-in-exchange.md) или [Подписка на уведомления об изменениях папки](notification-subscriptions-mailbox-events-and-ews-in-exchange.md) на сервере. 
  
## <a name="see-also"></a>См. также

- [Папки и элементы в веб-службах Exchange](folders-and-items-in-ews-in-exchange.md)   
- [Работа с элементами почтовых ящиков Exchange с помощью веб-служб Exchange](how-to-work-with-exchange-mailbox-items-by-using-ews-in-exchange.md)    
- [Удаление элементов с помощью EWS в Exchange](deleting-items-by-using-ews-in-exchange.md)   
- [Разработка клиентов веб-служб для Exchange](develop-web-service-clients-for-exchange.md)
    

