---
title: Работа с папками с помощью веб-служб Exchange в Exchange
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
localization_priority: Normal
ms.assetid: 4b3eb746-74c4-42a0-aa2c-742c147f1871
description: Узнайте, как создание, получение, обновление и удаление папок с помощью управляемого интерфейса API веб-служб Exchange или веб-служб Exchange в Exchange.
ms.openlocfilehash: a9a9e5974b2751268f37a1c9faacce43a333bcdb
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/11/2018
ms.locfileid: "19761149"
---
# <a name="work-with-folders-by-using-ews-in-exchange"></a>Работа с папками с помощью веб-служб Exchange в Exchange

Узнайте, как создание, получение, обновление и удаление папок с помощью управляемого интерфейса API веб-служб Exchange или веб-служб Exchange в Exchange.
  
ВЕБ-службах Exchange использует папки для структурирования и организации почтовых ящиков. Можно создать новый, получение, обновление и удаление папок с помощью управляемого интерфейса API веб-служб Exchange или веб-служб Exchange. Каждый из методов или операции, перечисленные в следующей таблице выполняется на объект [Folder](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.folder%28v=exchg.80%29.aspx) , типа [папки](http://msdn.microsoft.com/library/812948d8-c7db-45ce-bb3a-77233a53a974%28Office.15%29.aspx) или [один из папки производные классы или типы](folders-and-items-in-ews-in-exchange.md#bk_folders).
  
**В таблице 1. Методы и операции создание, получение, обновление и удаление папок**

|**Чтобы...**|**Метод управляемого API EWS**|**Операция служб EWS**|
|:-----|:-----|:-----|
|Создайте папку  <br/> |[Folder.Save](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.folder.save%28v=exchg.80%29.aspx) <br/> |[CreateFolder](http://msdn.microsoft.com/library/6f6c334c-b190-4e55-8f0a-38f2a018d1b3%28Office.15%29.aspx) <br/> |
|Создание иерархии папок  <br/> |Недоступна  <br/> |[CreateFolderPath](http://msdn.microsoft.com/library/5a10aa5e-3f25-4ec3-a0b9-284c30918a1f%28Office.15%29.aspx) <br/> |
|Получение папки  <br/> |[Folder.Bind](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.folder.bind%28v=exchg.80%29.aspx) <br/> |[GetFolder](http://msdn.microsoft.com/library/355bcf93-dc71-4493-b177-622afac5fdb9%28Office.15%29.aspx) <br/> |
|Получение иерархии папок  <br/> |[Folder.FindFolders](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.folder.findfolders%28v=exchg.80%29.aspx) <br/> |[FindFolder](http://msdn.microsoft.com/library/7a9855aa-06cc-45ba-ad2a-645c15b7d031%28Office.15%29.aspx) <br/> |
|Изменение папки  <br/> |[Folder.Update](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.folder.update%28v=exchg.80%29.aspx) <br/> |[UpdateFolder](http://msdn.microsoft.com/library/3494c996-b834-4813-b1ca-d99642d8b4e7%28Office.15%29.aspx) <br/> |
|Удаление папки  <br/> |[Folder.Delete](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.folder.delete%28v=exchg.80%29.aspx) <br/> |[DeleteFolder](http://msdn.microsoft.com/library/b0f92682-4895-4bcf-a4a1-e4c2e8403979%28Office.15%29.aspx) <br/> |

<a name="bk_createfolderewsma"> </a>

## <a name="create-a-folder-by-using-the-ews-managed-api"></a>Создайте папку с помощью управляемого интерфейса API веб-служб Exchange

В следующем примере кода показано, как использовать класс [папку](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.folder%28v=exchg.80%29.aspx) для создания новой общей папки с [DisplayName](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.folder.displayname%28v=exchg.80%29.aspx) «Настраиваемые папки» и значение свойства [FolderClass](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.folder.folderclass%28v=exchg.80%29.aspx) IPF. Примечание. Метод [Folder.Save](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.folder.save%28v=exchg.80%29.aspx) сохраняет папку в качестве дочерней папки «Входящие». 
  
В этих примерах предполагается этой **службы** является допустимым объектом [ExchangeService](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.exchangeservice%28v=exchg.80%29.aspx) и пользователь прошел проверку подлинности на сервере Exchange. 
  
```cs
// Create a custom folder.
Folder folder = new Folder(service);
folder.DisplayName = "Custom Folder";
folder.FolderClass = "IPF.Note";
// Save the folder as a child folder of the Inbox.
folder.Save(WellKnownFolderName.Inbox);
```

Для создания другого типа папки, например [CalendarFolder](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.calendarfolder%28v=exchg.80%29.aspx), [ContactsFolder](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.contactsfolder%28v=exchg.80%29.aspx), [SearchFolder](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.searchfolder%28v=exchg.80%29.aspx)или [TasksFolder](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.tasksfolder%28v=exchg.80%29.aspx), создайте новый экземпляр объекта определенного класса (а не универсальный класс **папки** ) и не задана Свойство **FolderClass** . Например в следующем примере кода показано, как создать новый [TasksFolder](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.tasksfolder%28v=exchg.80%29.aspx).
  
```cs
// Create a custom Tasks folder.
TasksFolder folder = new TasksFolder(service);
folder.DisplayName = "Custom Tasks";
// Save the folder as a child folder in the Inbox folder.
// This method call results in a CreateFolder call to EWS.
folder.Save(WellKnownFolderName.Inbox);
```

При попытке создать экземпляр определенного класса, а также необходимо задать свойство **FolderClass** , возникает ошибка [ErrorNoFolderClassOverride](http://msdn.microsoft.com/en-us/library/exchangewebservices.responsecodetype%28v=exchg.80%29.aspx) . 
  
Обратите внимание, что нельзя Пакетное создание несколько папок в одном методе с помощью управляемого интерфейса API веб-служб Exchange.
  
## <a name="create-a-folder-by-using-ews"></a>Создайте папку с помощью веб-служб Exchange
<a name="bk_createfolderews"> </a>

Можно создать несколько папок или одной папке с помощью веб-служб Exchange.
  
Для создания единого папки, отправьте сообщение [CreateFolder](http://msdn.microsoft.com/library/6f6c334c-b190-4e55-8f0a-38f2a018d1b3%28Office.15%29.aspx) операции запроса. Запрос операции **CreateFolder** указывает, что родительской папки — это папки «Входящие», [DisplayName](http://msdn.microsoft.com/library/e7efbbe1-6629-4d11-bed1-ed899e3f9d77%28Office.15%29.aspx) — это «Настраиваемая папка» и значения элемента [FolderClass](http://msdn.microsoft.com/library/0041d135-2869-4612-89a5-d1aa86aa1093%28Office.15%29.aspx) является IPF. Примечание. 
  
Это также XML-запрос, который отправляет управляемый API EWS при создании новой папки и вызовите метод [Folder.Save](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.folder.save%28v=exchg.80%29.aspx) . 
  
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

Сервер отвечает на запрос **CreateFolder** [CreateFolderResponse](http://msdn.microsoft.com/library/158adecc-491a-47d9-af73-acc2cd3f8566%28Office.15%29.aspx) сообщение, содержащее значение [ResponseCode](http://msdn.microsoft.com/en-us/library/aa580757%28v=exchg.150%29.aspx) **NoError**, это означает, что папка была создана успешно, и [FolderId](http://msdn.microsoft.com/library/00d14e3e-4365-4f21-8f88-eaeea73b9bf7%28Office.15%29.aspx) из только что созданный сообщение. 
  
Чтобы создать несколько папок, включают несколько элементов [папки](http://msdn.microsoft.com/library/812948d8-c7db-45ce-bb3a-77233a53a974%28Office.15%29.aspx) в сообщении **CreateFolder** операции запроса. Все новые папки должен быть в одной родительской папке. 
  
## <a name="create-a-folder-hierarchy-by-using-ews"></a>Создание иерархии папок с помощью веб-служб Exchange
<a name="bk_createfolderhierarchy"> </a>

Можно создать иерархии папок в одном вызове с помощью операции EWS [CreateFolderPath](http://msdn.microsoft.com/library/5a10aa5e-3f25-4ec3-a0b9-284c30918a1f%28Office.15%29.aspx) . Те же функциональные возможности недоступен в управляемый API веб-служб Exchange. Вместо этого при использовании управляемого интерфейса API веб-служб Exchange, можно создавать папки по одному, как показано в разделе [Создание папки с помощью веб-служб Exchange](#bk_createfolderews).
  
> [!NOTE]
> Управляемый API EWS не реализует эту функцию. 
  
## <a name="get-a-folder-by-using-the-ews-managed-api"></a>Получение папки с помощью управляемого интерфейса API веб-служб Exchange
<a name="bk_getfolderewsma"> </a>

В следующем примере кода показано, как использовать метод [Folder.Bind](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.folder.bind%28v=exchg.80%29.aspx) для получения папке "Входящие". Рекомендуется ограничивайте возвращаемые только теми, необходимый для приложения свойства. В этом примере ограничивается возвращаемого свойства можно включить только свойство [Id](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.folder.id%28v=exchg.80%29.aspx) , создав объект [PropertySet](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.propertyset%28v=exchg.80%29.aspx) и применения [IdOnly](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.basepropertyset%28v=exchg.80%29.aspx) значения для свойства [BasePropertySet](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.propertyset.basepropertyset%28v=exchg.80%29.aspx) . 
  
В этом примере предполагается, что эта **Служба** является допустимым объектом [ExchangeService](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.exchangeservice%28v=exchg.80%29.aspx) и пользователь прошел проверку подлинности на сервере Exchange. 
  
```cs
// As a best practice, limit the properties returned to only those that are required.
// In this scenario, you only need the FolderId.
PropertySet propSet = new PropertySet(BasePropertySet.IdOnly);
// Bind to an existing folder and get only the properties specified in the PropertySet.
// This method call results in a GetFolder call to EWS.
Folder rootfolder = Folder.Bind(service, WellKnownFolderName.Inbox, propSet);
```

Если вам потребуется получить дополнительные свойства, добавьте свойства из класса [FolderSchema](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.folderschema%28v=exchg.80%29.aspx) **PropertySet**или использовать один из перегруженных методов [привязки](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.folder.bind%28v=exchg.80%29.aspx) , которые возвращаются все свойства первого класса. 
  
Следует отметить, что нельзя одновременно несколько папок с помощью управляемого интерфейса API веб-служб Exchange. Необходимо вызвать метод **привязки** для каждой папки отдельно. 
  
## <a name="get-a-folder-by-using-ews"></a>Получение папки с помощью веб-служб Exchange
<a name="bk_getfolderews"> </a>

Можно получить одной папке или несколько папок с помощью веб-служб Exchange.
  
Для получения одной папке отправьте сообщение [GetFolder](http://msdn.microsoft.com/library/355bcf93-dc71-4493-b177-622afac5fdb9%28Office.15%29.aspx) операция запроса к серверу. В следующем примере устанавливается [BaseShape](http://msdn.microsoft.com/library/42c04f3b-abaa-4197-a3d6-d21677ffb1c0%28Office.15%29.aspx) для **IdOnly**, возвращается только [FolderId](http://msdn.microsoft.com/library/00d14e3e-4365-4f21-8f88-eaeea73b9bf7%28Office.15%29.aspx) указанной папки. Элемент [FolderIds](http://msdn.microsoft.com/library/3ff9d15a-7220-4785-ae6b-583a7eb82005%28Office.15%29.aspx) указывает, что папка для извлечения папки "Входящие". 
  
Это также XML-запрос, который отправляет управляемый API EWS при связывании в папку с помощью метода [Folder.Bind](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.folder.bind%28v=exchg.80%29.aspx) . 
  
Чтобы получить несколько папок, включают несколько элементов [FolderIds](http://msdn.microsoft.com/library/812948d8-c7db-45ce-bb3a-77233a53a974%28Office.15%29.aspx) в сообщении **GetFolder** операции запроса. 
  
```XML
<?xml version="1.0" encoding="utf-8"?>
<soap:Envelope xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" xmlns:m="http://schemas.microsoft.com/exchange/services/2006/messages" xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types" xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/">
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

В следующем примере XML показано [GetFolderResponse](http://msdn.microsoft.com/library/47abeec8-78dd-4297-8525-099174ec880d%28Office.15%29.aspx) сообщение, которое отправляется с сервера на клиент в ответ на запрос операции **GetFolder** . Содержит только значение [FolderId](http://msdn.microsoft.com/library/00d14e3e-4365-4f21-8f88-eaeea73b9bf7%28Office.15%29.aspx) папки "Входящие". Для удобства чтения URL были сокращены значения некоторые атрибуты и элементы. 
  
```XML
<?xml version="1.0" encoding="utf-8"?>
<s:Envelope xmlns:s="http://schemas.xmlsoap.org/soap/envelope/">
  <s:Header>
    <h:ServerVersionInfo MajorVersion="15"
                         MinorVersion="0"
                         MajorBuildNumber="800"
                         MinorBuildNumber="16"
                         Version="V2_6"
                         xmlns:h="http://schemas.microsoft.com/exchange/services/2006/types"
                         xmlns="http://schemas.microsoft.com/exchange/services/2006/types"
                         xmlns:xsd="http://www.w3.org/2001/XMLSchema"
                         xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance"/>
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
              <t:FolderId Id="AAAENAAA=" ChangeKey="AQAAABYAAAAPxolXAHv3TaHUnjW8wWqXAAAEkbCr"/>
            </t:Folder>
          </m:Folders>
        </m:GetFolderResponseMessage>
      </m:ResponseMessages>
    </m:GetFolderResponse>
  </s:Body>
</s:Envelope>
```

## <a name="get-a-folder-hierarchy-by-using-the-ews-managed-api"></a>Получение иерархии папок с помощью управляемого интерфейса API веб-служб Exchange
<a name="bk_getfolderhierarchyewsma"> </a>

В следующем примере кода показано, как получить вложенные папки для указанной корневой папке. В этом примере показано получение вложенные папки в папку **MsgFolderRoot** , которая является корневым каталогом поддерева IPM (папки почтовых ящиков и элементы хранения). 
  
В этом примере объект класса [FolderView](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.folderview%28v=exchg.80%29.aspx) создается для ограничения результатов ответа метода [Folder.FindFolders](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.folder.findfolders%28v=exchg.80%29.aspx) . Этот сценарий ограничивает возвращаемых для следующих свойств: [идентификатор](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.folder.id%28v=exchg.80%29.aspx), [DisplayName](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.folder.displayname%28v=exchg.80%29.aspx)и расширенные свойства, которое указывает, является ли папка является скрытым. Задайте значение [FolderView.Traversal](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.folderview.traversal%28v=EXCHG.80%29.aspx) глубокое для выполнения рекурсивный поиск, чтобы сервер получает вложенных папок, а значение в корневой папке **MsgFolderRoot**, чтобы сервер возвращает все папках пользователя (и сервер не возвращает системные папки поддерева IPM не).
  
В этом примере предполагается, что эта **Служба** является допустимым объектом [ExchangeService](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.exchangeservice%28v=exchg.80%29.aspx) и пользователь прошел проверку подлинности на сервере Exchange. 
  
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

## <a name="get-a-folder-hierarchy-by-using-ews"></a>Получение иерархии папок с помощью веб-служб Exchange
<a name="bk_getfolderhierarchyews"> </a>

В следующих примерах XML для получения иерархии папок с помощью веб-служб Exchange с помощью операции [FindFolder](http://msdn.microsoft.com/library/7a9855aa-06cc-45ba-ad2a-645c15b7d031%28Office.15%29.aspx) . В этом примере извлекается в папку **msgfolderroot** , которая является корневым каталогом поддерева IPM и все вложенные папки. Атрибут **обхода** присваивается **глубокое** , чтобы сервер выполняет рекурсивный поиск в иерархии папок и возвращает только папки и вложенные папки в корневом каталоге указанного в ответе. В следующем примере элемент [BaseShape](http://msdn.microsoft.com/library/42c04f3b-abaa-4197-a3d6-d21677ffb1c0%28Office.15%29.aspx) присваивается **IdOnly** , чтобы сервер только возвращает элемент [FolderId](http://msdn.microsoft.com/library/00d14e3e-4365-4f21-8f88-eaeea73b9bf7%28Office.15%29.aspx) . Чтобы облегчить понимание выходные данные, включите элемент **DisplayName** в результатах, включив в элемент [AdditionalProperties](http://msdn.microsoft.com/library/7a269aed-dcfd-4c3e-9e14-094e53828101%28Office.15%29.aspx) в запросе, а также значение **ExtendedFieldURI** для **PR_ATTR_HIDDEN** свойства, чтобы знать, являются ли папки скрытые папки. 
  
Это также запроса XML, то при вызове метода [FindFolders](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.exchangeservice.findfolders%28v=exchg.80%29.aspx) отправляет управляемый API веб-служб Exchange. 
  
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

В следующем примере XML показано [FindFolderResponse](http://msdn.microsoft.com/library/f5dd813c-9698-4a39-8fca-3a825df365ed%28Office.15%29.aspx) сообщение, которое отправляется с сервера на клиент в ответ на запрос операции **FindFolder** . Он содержит только [FolderId](http://msdn.microsoft.com/library/00d14e3e-4365-4f21-8f88-eaeea73b9bf7%28Office.15%29.aspx), [DisplayName](http://msdn.microsoft.com/library/e7efbbe1-6629-4d11-bed1-ed899e3f9d77%28Office.15%29.aspx), и значение **PR_ATTR_HIDDEN** расширенные свойства для всех вложенных папок в папке **msgrootfolder** . Если [значение](http://msdn.microsoft.com/library/9a30cadd-909e-41b1-b4e9-291643dd89c6%28Office.15%29.aspx) элемента задано значение true, папка должны быть скрыты в представлении клиента. 
  
Это также XML-ответ, который отправляет управляемый API веб-служб Exchange, когда вы получаете несколько папок с помощью метода [FindFolder](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.folder.findfolders%28v=exchg.80%29.aspx) . Значения некоторые атрибуты и элементы URL были сокращены для удобства чтения и некоторые папки не были включены для краткости. 
  
```XML
<?xml version="1.0" encoding="utf-8"?><s:Envelope xmlns:s="http://schemas.xmlsoap.org/soap/envelope/">
  <s:Header>
    <h:ServerVersionInfo MajorVersion="15"
                         MinorVersion="0"
                         MajorBuildNumber="815"
                         MinorBuildNumber="6"
                         Version="V2_7"
                         xmlns:h="http://schemas.microsoft.com/exchange/services/2006/types"
                         xmlns="http://schemas.microsoft.com/exchange/services/2006/types"
                         xmlns:xsd="http://www.w3.org/2001/XMLSchema"
                         xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance"/>
  </s:Header>
  <s:Body xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance"
          xmlns:xsd="http://www.w3.org/2001/XMLSchema">
    <m:FindFolderResponse xmlns:m="http://schemas.microsoft.com/exchange/services/2006/messages"
                          xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types">
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

## <a name="update-a-folder-by-using-the-ews-managed-api"></a>Изменение папки с помощью управляемого интерфейса API веб-служб Exchange
<a name="bk_updatefolderewsma"> </a>

В следующем примере кода показано, как обновить отображаемое имя папки с помощью управляемого интерфейса API веб-служб Exchange.
  
Во-первых создайте [PropertySet](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.propertyset%28v=exchg.80%29.aspx) , чтобы ограничить число свойств, которые сервер возвращает в ответе [Folder.Bind](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.folder.bind%28v=exchg.80%29.aspx) . Мы рекомендуем использовать **IdOnly** **BasePropertySet** для уменьшения обращений к базе данных Exchange. Затем используйте метод **Bind** для привязки к папке требуется обновить. Затем обновите свойство [DisplayName](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.folder.displayname%28v=exchg.80%29.aspx) и используйте метод [Folder.Update](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.folder.update%28v=exchg.80%29.aspx) для сохранения изменений. 
  
В этом примере мы предполагаем этой **службы** является допустимым объектом [ExchangeService](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.exchangeservice%28v=exchg.80%29.aspx) и пользователь прошел проверку подлинности на сервере Exchange. Локальной переменной *folderId* — это [идентификатор](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.folder.id%28v=exchg.80%29.aspx) папки для обновления. 
  
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

## <a name="update-a-folder-by-using-ews"></a>Изменение папки с помощью веб-служб Exchange
<a name="bk_updatefolderews"> </a>

В следующих примерах XML показано, как обновить отображаемое имя папки с помощью веб-служб Exchange.
  
Во-первых отправьте сообщение [GetFolder](http://msdn.microsoft.com/library/355bcf93-dc71-4493-b177-622afac5fdb9%28Office.15%29.aspx) операция запроса на получение папки для обновления, как показано в [Начало иерархии папок с помощью веб-служб Exchange](#bk_getfolderhierarchyews).
  
Затем отправьте сообщение [UpdateFolder](http://msdn.microsoft.com/library/3494c996-b834-4813-b1ca-d99642d8b4e7%28Office.15%29.aspx) операция запроса сервером, чтобы обновить папку. Запрос операции **UpdateFolder** обновляет [DisplayName](http://msdn.microsoft.com/library/42c04f3b-abaa-4197-a3d6-d21677ffb1c0%28Office.15%29.aspx) «Обновить папку Custom». 
  
Это также XML-запрос, который отправляет управляемый API EWS при обновлении папки с помощью метода [Folder.Update](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.folder.update%28v=exchg.80%29.aspx) . Для удобства чтения URL были сокращены значения некоторые атрибуты и элементы. 
  
```XML
<?xml version="1.0" encoding="utf-8"?>
<soap:Envelope xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" xmlns:m="http://schemas.microsoft.com/exchange/services/2006/messages" xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types" xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/">
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

Сервер отвечает на запрос **UpdateFolder** [UpdateFolderResponse](http://msdn.microsoft.com/library/31f47739-dc9c-46ba-9e3f-cce25dc85e6e%28Office.15%29.aspx) сообщение, содержащее значение [ResponseCode](http://msdn.microsoft.com/en-us/library/aa580757%28v=exchg.150%29.aspx) **NoError**и [FolderId](http://msdn.microsoft.com/library/00d14e3e-4365-4f21-8f88-eaeea73b9bf7%28Office.15%29.aspx) папки, которая была обновлена с обновленные ** ChangeKey** значение атрибута. 
  
## <a name="delete-a-folder-by-using-the-ews-managed-api"></a>Удаление папки с помощью управляемого интерфейса API веб-служб Exchange
<a name="bk_deletefolderewsma"> </a>

В этой статье приводятся основные пример, в котором показано, как удалить папку с помощью управляемого интерфейса API веб-служб Exchange. Для получения дополнительных сведений об удалении папок видеть [Удаление элементов с помощью веб-служб Exchange в Exchange](deleting-items-by-using-ews-in-exchange.md).
  
Чтобы удалить папку с помощью управляемого интерфейса API веб-служб Exchange, во-первых, используйте метод [Folder.Bind](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.folder.bind%28v=exchg.80%29.aspx) для привязки к объекту службы в папку для удаления. Затем используйте метод [Folder.Delete](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.folder.delete%28v=exchg.80%29.aspx) удалить папку с помощью режима удаления [HardDelete](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.deletemode%28v=exchg.80%29.aspx) . 
  
В этом примере предполагается, что эта **Служба** является допустимым объектом [ExchangeService](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.exchangeservice%28v=exchg.80%29.aspx) и пользователь прошел проверку подлинности на сервере Exchange. Локальной переменной *folderId* — это [идентификатор](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.folder.id%28v=exchg.80%29.aspx) папки для удаления. 
  
```cs
// Bind to an existing folder and get all its properties.
// This method call results in a GetFolder call to EWS.
Folder folder = Folder.Bind(service, folderId);
// HardDelete the folder.
// This method call results in a DeleteFolder call to EWS.
folder.Delete(DeleteMode.HardDelete);
```

## <a name="delete-a-folder-by-using-ews"></a>Удаление папки с помощью веб-служб Exchange
<a name="bk_deletefolderews"> </a>

В этой статье приводятся основные примере XML-кода показано, как удалить папку с помощью веб-служб Exchange. Для получения дополнительных сведений об удалении папок видеть [Удаление элементов с помощью веб-служб Exchange в Exchange](deleting-items-by-using-ews-in-exchange.md).
  
Удалить папку с помощью веб-служб Exchange, во-первых, отправьте сообщение [GetFolder](http://msdn.microsoft.com/library/355bcf93-dc71-4493-b177-622afac5fdb9%28Office.15%29.aspx) операция запроса на получение папки для обновления, как показано на [Получение папки с помощью веб-служб Exchange](#bk_getfolderews). 
  
Далее отправьте сообщение [DeleteFolder](http://msdn.microsoft.com/library/b0f92682-4895-4bcf-a4a1-e4c2e8403979%28Office.15%29.aspx) операция запроса сервером, чтобы удалить папку. Запрос операции **DeleteFolder** указывает, что **DeleteType** **HardDelete** и включает [FolderId](http://msdn.microsoft.com/library/00d14e3e-4365-4f21-8f88-eaeea73b9bf7%28Office.15%29.aspx) папки для удаления. 
  
Это также XML-запрос, который отправляет управляемый API EWS при удалении папки с помощью метода [Folder.Delete](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.folder.delete%28v=exchg.80%29.aspx) . Для удобства чтения URL были сокращены значения некоторые атрибуты и элементы. 
  
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
    <m:DeleteFolder DeleteType="HardDelete">
      <m:FolderIds>
        <t:FolderId Id="OrV9ZAAA=" ChangeKey="AQAAABYAAABVzRdyy/cHS4XTC9itCRdUAAAOrXWf" />
      </m:FolderIds>
    </m:DeleteFolder>
  </soap:Body>
</soap:Envelope>
```

Сервер отвечает на запрос **DeleteFolder** [DeleteFolderResponse](http://msdn.microsoft.com/library/27578bda-ef0a-4a33-bccc-2c1bc1735424%28Office.15%29.aspx) сообщение, содержащее значение [ResponseCode](http://msdn.microsoft.com/en-us/library/aa580757%28v=exchg.150%29.aspx) **NoError**, это означает, что удаление папки прошла успешно.
  
## <a name="next-steps"></a>Дальнейшие действия
<a name="bk_nextsteps"> </a>

После извлечения папок на сервере, или внесенные изменения к папкам, может потребоваться [Синхронизация иерархии папок](how-to-synchronize-folders-by-using-ews-in-exchange.md) или [подписаться на уведомления об изменениях в папку](notification-subscriptions-mailbox-events-and-ews-in-exchange.md) на сервере. 
  
## <a name="see-also"></a>См. также

- [Папки и элементы в веб-службах Exchange](folders-and-items-in-ews-in-exchange.md)   
- [Работа с элементами почтового ящика Exchange с помощью веб-служб Exchange в Exchange](how-to-work-with-exchange-mailbox-items-by-using-ews-in-exchange.md)    
- [Удаление элементов с помощью веб-служб Exchange в Exchange](deleting-items-by-using-ews-in-exchange.md)   
- [Разработка клиентов веб-служб для Exchange](develop-web-service-clients-for-exchange.md)
    

