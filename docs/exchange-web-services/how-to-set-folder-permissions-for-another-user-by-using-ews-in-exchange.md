---
title: Настройка разрешений папки другого пользователя с помощью веб-служб Exchange в Exchange
manager: sethgros
ms.date: 03/9/2015
ms.audience: Developer
localization_priority: Normal
ms.assetid: 7eb81676-a780-4c56-b4f2-c4ed2697107d
description: Узнайте, как установить уровни разрешений для папки с помощью управляемого интерфейса API веб-служб Exchange или веб-служб Exchange в Exchange.
ms.openlocfilehash: 5bf570612d6349628e7f3abf858daa33daa13745
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/11/2018
ms.locfileid: "19761120"
---
# <a name="set-folder-permissions-for-another-user-by-using-ews-in-exchange"></a>Настройка разрешений папки другого пользователя с помощью веб-служб Exchange в Exchange

Узнайте, как установить уровни разрешений для папки с помощью управляемого интерфейса API веб-служб Exchange или веб-служб Exchange в Exchange.
  
Разрешения на уровне папки позволяют пользователям получать доступ к одной или нескольких папок в почтового ящика другого пользователя. Разрешения для папки, аналогичны делегированный доступ, но они отличаются следующими способами: 
  
- Разрешения для папки не следует включать пользователю «отправить от имени» или «отправить как» другому пользователю. Они только разрешение доступа к папкам. Пользователи могут создавать элементы в папках, но они не могут отправлять их.
    
- Можно задать разрешения для папки на любой папки в почтовом ящике, но можно только добавить делегата к папкам календаря, контакты, папки "Входящие", журнала, заметки и задачи.
    
- Можно задать число [разрешения для указанной папки](#bk_folderperms). При добавлении делегата, можно назначить один из только [пять уровней разрешений](delegate-access-and-ews-in-exchange.md#bk_delegateperms).
    
- Можно задать разрешения для папки для анонимных и по умолчанию пользователи. Можно предоставить делегированный доступ к учетной записи электронной почты.
    
Если вы знакомы с помощью элементов управления доступом (ACE) и списки управления доступом (доступом), значит, что пользователь может иметь только один набор разрешений для каждой папки. При попытке добавить набор разрешений для пользователя, и они уже имеют набор разрешений, приведет к ошибке. При Добавление, удаление или обновление разрешений для папки, вы получение текущего на уровне пользователей, добавьте или удалите все элементы управления доступом и выберите отправить обновленные на уровне пользователей. Не удается добавить несколько элементов управления доступом для одного пользователя. При обновлении разрешения с помощью управляемого интерфейса API веб-служб Exchange, необходимо удалить элемент управления ДОСТУПОМ текущего пользователя, а затем добавьте свой новый элемент управления ДОСТУПОМ к коллекции. Если вы используете веб-служб Exchange, просто замените предыдущий набор элементов ACE с помощью новых структур.
  
Если вы выполняете нескольких изменения разрешений в одной папке, можно batch добавления, удаления или обновления — только что Обратите внимание на то, что нельзя пакета обновления пользователя на несколько папок. Для получения разрешений для одной папке необходимо один звонок, а второй вызов требуется обновить разрешения для этой папки. При Добавление, удаление или обновление разрешений пользователя, используется один и тот же вызовы двух методов или операции для каждой задачи.
  
**В таблице 1. Управляемый API EWS методы и операции веб-служб Exchange для настройки разрешений папки**

|Задача|Используйте этот метод управляемый API EWS...|Используйте эту операцию EWS...|
|:-----|:-----|:-----|
|Включение, удаление или обновление разрешений для папки  <br/> |[Folder.Bind](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.folder.bind%28v=exchg.80%29.aspx) , а затем [Folder.Update](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.emailmessage.reply%28v=exchg.80%29.aspx) <br/> |[GetFolder](http://msdn.microsoft.com/library/355bcf93-dc71-4493-b177-622afac5fdb9%28Office.15%29.aspx) следуют [UpdateFolder](http://msdn.microsoft.com/library/3494c996-b834-4813-b1ca-d99642d8b4e7%28Office.15%29.aspx) <br/> |
|Создайте папку и определите разрешения для папки  <br/> |[Folder.Save](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.folder.save%28v=exchg.80%29.aspx) <br/> |[CreateFolder](http://msdn.microsoft.com/library/6f6c334c-b190-4e55-8f0a-38f2a018d1b3%28Office.15%29.aspx) <br/> |
   
## <a name="folder-permissions"></a>Разрешения для папки
<a name="bk_folderperms"> </a>

Имеется довольно много параметров, когда речь идет о Установка разрешений для папки на указанной папки. Можно задать уровень разрешений для папки для каждого пользователя, который добавляет набор предварительно заданных отдельных разрешений в СПИСКЕ, или можно задать отдельные разрешения на папку, но нельзя смешивать и соответствует.
  
Доступны следующие отдельные разрешения:
  
- Можно создать
- Можно создать вложенные папки    
- — Это владелец    
- Отображается папки    
- — Это папка контактов    
- Изменение элементов    
- Удаление элементов    
- Чтение элементов
    
Кроме того следующие уровни разрешений доступны, который определять подмножество отдельные разрешения и значения, как показано в таблице 2:
  
- Нет    
- Owner    
- PublishingEditor    
- Редактор    
- PublishingAuthor    
- Author    
- NoneditingAuthor    
- Редактор    
- Участник   
- Custom — это значение не могут задаваться для приложения. Сервер задает это значение, если приложение включает пользовательский набор отдельных разрешений.    
- FreeBusyTimeOnly — это может устанавливаться только для папок календаря.   
- FreeBusyTimeAndSubjectAndLocation — это может устанавливаться только для папок календаря.
    
В следующей таблице показаны какие отдельных разрешений по умолчанию, в зависимости от уровня разрешений.
  
**В таблице 2. Отдельные разрешения, уровень разрешений**

|Уровень разрешений|Можно создавать элементы|Можно создать вложенные папки|— Это владелец|Отображается папки|— Это папка контактов|Изменение элементов|Удаление элементов|Чтение элементов|
|:-----|:-----|:-----|:-----|:-----|:-----|:-----|:-----|:-----|
|Нет  <br/> |Ложь  <br/> |Ложь  <br/> |Ложь  <br/> |Ложь  <br/> |Ложь  <br/> |Нет  <br/> |Нет  <br/> |Нет  <br/> |
|Owner  <br/> |True  <br/> |True  <br/> |True  <br/> |True  <br/> |True  <br/> |Все  <br/> |Все  <br/> |FullDetails  <br/> |
|PublishingEditor  <br/> |True  <br/> |Истина  <br/> |Ложь  <br/> |Истина  <br/> |Ложь  <br/> |Все  <br/> |Все  <br/> |FullDetails  <br/> |
|Редактор  <br/> |Истина  <br/> |Ложь  <br/> |Ложь  <br/> |Истина  <br/> |Ложь  <br/> |Все  <br/> |Все  <br/> |FullDetails  <br/> |
|PublishingAuthor  <br/> |True  <br/> |Истина  <br/> |Ложь  <br/> |Истина  <br/> |Ложь  <br/> |Владельцем  <br/> |Владельцем  <br/> |FullDetails  <br/> |
|Author  <br/> |Истина  <br/> |Ложь  <br/> |Ложь  <br/> |Истина  <br/> |Ложь  <br/> |Владельцем  <br/> |Владельцем  <br/> |FullDetails  <br/> |
|NoneditingAuthor  <br/> |Истина  <br/> |Ложь  <br/> |Ложь  <br/> |Истина  <br/> |Ложь  <br/> |Нет  <br/> |Владельцем  <br/> |FullDetails  <br/> |
|Редактор  <br/> |Ложь  <br/> |Ложь  <br/> |Ложь  <br/> |Истина  <br/> |Ложь  <br/> |Нет  <br/> |Нет  <br/> |FullDetails  <br/> |
|Участник  <br/> |Истина  <br/> |Ложь  <br/> |Ложь  <br/> |Истина  <br/> |Ложь  <br/> |Нет  <br/> |Нет  <br/> |Нет  <br/> |
   
При указании уровня разрешений ненастраиваемых в запросе на разрешения на уровне папки, не нужно указать параметры отдельных разрешений. При указании отдельных разрешений при установке на уровень разрешений, ошибка **ErrorInvalidPermissionSettings** , возвращается в ответе. 
  
## <a name="adding-folder-permissions-by-using-the-ews-managed-api"></a>Добавление разрешений для папки с помощью управляемого интерфейса API веб-служб Exchange
<a name="bk_enableewsma"> </a>

В следующем примере кода показано, как использовать управляемый API EWS для: 
  
- Создание нового объекта [FolderPermission](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.folderpermission%28v=exchg.80%29.aspx) для нового пользователя. 
    
- Получение текущих разрешений для папки с помощью метода [привязки](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.folder.bind%28v=exchg.80%29.aspx) . 
    
- Добавьте новый **FolderPermissions** свойство [Folder.Permissions](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.folder.permissions%28v=exchg.80%29.aspx) . 
    
- Вызовите метод [Update](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.folder.update%28v=exchg.80%29.aspx) , чтобы сохранить новые разрешения на сервере. 
    
В этом примере предполагается, что эта **Служба** является допустимым объектом [ExchangeService](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.exchangeservice%28v=exchg.80%29.aspx) владельца почтового ящика, который пользователь прошел проверку подлинности на сервере Exchange. 
  
```cs
static void EnableFolderPermissions(ExchangeService service)
{
    // Create a property set to use for folder binding.
    PropertySet propSet = new PropertySet(BasePropertySet.IdOnly, FolderSchema.Permissions);
    // Specify the SMTP address of the new user and the folder permissions level.
    FolderPermission fldperm = new FolderPermission("sadie@contoso.com", FolderPermissionLevel.Editor);
    
    // Bind to the folder and get the current permissions. 
    // This call results in a GetFolder call to EWS.
    Folder sentItemsFolder = Folder.Bind(service, WellKnownFolderName.SentItems, propSet);
 
    // Add the permissions for the new user to the Sent Items DACL.
    sentItemsFolder.Permissions.Add(fldperm);
    // This call results in a UpdateFolder call to EWS.
    sentItemsFolder.Update();
}
```

Следующая строка кода указывает уровень разрешений.
  
```cs
    FolderPermission fldperm = new FolderPermission("sadie@contoso.com", FolderPermissionLevel.Editor);
```

Если вы хотите использовать пользовательский уровень разрешений, используйте следующий код.
  
```cs
FolderPermission fldperm = new FolderPermission();
fldperm.UserId = "sadie@Contoso1000.onmicrosoft.com";
fldperm.CanCreateItems = true;
fldperm.CanCreateSubFolders = true;
…
```

Можно установить одно или несколько для записи [FolderPermission свойства](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.folderpermission_properties%28v=exchg.80%29.aspx) при создании объекта **FolderPermission** с пользовательский уровень разрешений. Тем не менее, [FolderPermissionLevel](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.folderpermissionlevel%28v=exchg.80%29.aspx) включена никогда не явным образом для **настраиваемого** приложения. **FolderPermissionLevel** настраиваемых имеет значение только в том случае, если создание объекта **FolderPermission** и задать отдельные разрешения. 
  
## <a name="adding-folder-permissions-by-using-ews"></a>Добавление разрешений для папки с помощью веб-служб Exchange
<a name="bk_enableews"> </a>

В следующих примерах кода веб-служб Exchange показано, как для добавления разрешений к конкретной папке путем получения текущих разрешений и затем отправить список новые разрешения.
  
Первый шаг — отправить запрос [GetFolder](http://msdn.microsoft.com/library/355bcf93-dc71-4493-b177-622afac5fdb9%28Office.15%29.aspx) , где значение [DistinguishedFolderId](http://msdn.microsoft.com/library/50018162-2941-4227-8a5b-d6b4686bb32f%28Office.15%29.aspx) указывает папку, в которой для добавления разрешений (папка Отправленные в данном примере), а значение [FieldURI](http://msdn.microsoft.com/library/24af8e3b-3074-4c8c-8d0a-52446508d044%28Office.15%29.aspx) включает в себя папки: PermissionSet. Этот запрос будет получить параметры разрешений для указанной папки. 
  
Это также XML-запрос, который отправляет управляемый API EWS при вызове метода **привязки** для [добавления разрешений для папки](#bk_enableewsma).
  
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
            <t:FieldURI FieldURI="folder:PermissionSet" />
          </t:AdditionalProperties>
        </m:FolderShape>
        <m:FolderIds>
          <t:DistinguishedFolderId Id="sentitems" />
        </m:FolderIds>
      </m:GetFolder>
    </soap:Body>
  </soap:Envelope>
```

Сервер отвечает на запрос **GetFolder** [GetFolderResponse](http://msdn.microsoft.com/library/47abeec8-78dd-4297-8525-099174ec880d%28Office.15%29.aspx) сообщение, которое содержит значение элемента [ResponseCode](http://msdn.microsoft.com/library/4b84d670-74c9-4d6d-84e7-f0a9f76f0d93%28Office.15%29.aspx) **NoError**, это означает, что папка был успешно извлечен. Для удобства чтения URL были сокращены [FolderId](http://msdn.microsoft.com/library/00d14e3e-4365-4f21-8f88-eaeea73b9bf7%28Office.15%29.aspx) и [ParentFolderId](http://msdn.microsoft.com/library/258f4b1f-367e-4c7d-9c29-eb775a2398c7%28Office.15%29.aspx) значения. 
  
```XML
<?xml version="1.0" encoding="utf-8"?>
<s:Envelope xmlns:s="http://schemas.xmlsoap.org/soap/envelope/">
  <s:Header>
    <h:ServerVersionInfo MajorVersion="15"
                         MinorVersion="0"
                         MajorBuildNumber="893"
                         MinorBuildNumber="17"
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
              <t:FolderId Id="CgAAAA=="
                          ChangeKey="AQAAABYAAADOilbYa8KaT7ZgMoTz2P+hAAABiRd1" />
              <t:PermissionSet>
                <t:Permissions>
                  <t:Permission>
                    <t:UserId>
                      <t:DistinguishedUser>Default</t:DistinguishedUser>
                    </t:UserId>
                    <t:CanCreateItems>false</t:CanCreateItems>
                    <t:CanCreateSubFolders>false</t:CanCreateSubFolders>
                    <t:IsFolderOwner>false</t:IsFolderOwner>
                    <t:IsFolderVisible>false</t:IsFolderVisible>
                    <t:IsFolderContact>false</t:IsFolderContact>
                    <t:EditItems>None</t:EditItems>
                    <t:DeleteItems>None</t:DeleteItems>
                    <t:ReadItems>None</t:ReadItems>
                    <t:PermissionLevel>None</t:PermissionLevel>
                  </t:Permission>
                  <t:Permission>
                    <t:UserId>
                      <t:DistinguishedUser>Anonymous</t:DistinguishedUser>
                    </t:UserId>
                    <t:CanCreateItems>false</t:CanCreateItems>
                    <t:CanCreateSubFolders>false</t:CanCreateSubFolders>
                    <t:IsFolderOwner>false</t:IsFolderOwner>
                    <t:IsFolderVisible>false</t:IsFolderVisible>
                    <t:IsFolderContact>false</t:IsFolderContact>
                    <t:EditItems>None</t:EditItems>
                    <t:DeleteItems>None</t:DeleteItems>
                    <t:ReadItems>None</t:ReadItems>
                    <t:PermissionLevel>None</t:PermissionLevel>
                  </t:Permission>
                </t:Permissions>
              </t:PermissionSet>
            </t:Folder>
          </m:Folders>
        </m:GetFolderResponseMessage>
      </m:ResponseMessages>
    </m:GetFolderResponse>
  </s:Body>
</s:Envelope>
```

Затем используйте операцию **UpdateFolder** для отправки обновленные [PermissionSet](http://msdn.microsoft.com/library/6ac1bd17-a089-46bb-b9e6-f5b1dfe1076d%28Office.15%29.aspx), которая включает в себя [разрешения](http://msdn.microsoft.com/library/b8d0429a-0e58-4480-9847-4901970c7033%28Office.15%29.aspx) для нового пользователя. Обратите внимание на то, что включение элемент [SetFolderField](http://msdn.microsoft.com/library/8c69db7b-54b5-4ae2-abca-4d6e0937a790%28Office.15%29.aspx) для соответствующей папке в операции [UpdateFolder](http://msdn.microsoft.com/library/3494c996-b834-4813-b1ca-d99642d8b4e7%28Office.15%29.aspx) перезапишет все параметры разрешений на папку. Аналогичным образом включая параметр [DeleteFolderField](http://msdn.microsoft.com/library/f9c2187b-4c60-4358-b4b4-ede50eadae48%28Office.15%29.aspx) **UpdateFolder** операции приведет к удалению всех параметров разрешений на папку. 
  
Это также XML-запрос, который отправляет управляемый API EWS при вызове метода **Update** для [добавления разрешений для папки](#bk_enableewsma).
  
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
          <t:FolderId Id="CgAAAA=="
                      ChangeKey="AQAAABYAAADOilbYa8KaT7ZgMoTz2P+hAAABiRd1" />
          <t:Updates>
            <t:SetFolderField>
              <t:FieldURI FieldURI="folder:PermissionSet" />
              <t:Folder>
                <t:PermissionSet>
                  <t:Permissions>
                    <t:Permission>
                      <t:UserId>
                        <t:DistinguishedUser>Default</t:DistinguishedUser>
                      </t:UserId>
                      <t:PermissionLevel>None</t:PermissionLevel>
                    </t:Permission>
                    <t:Permission>
                      <t:UserId>
                        <t:DistinguishedUser>Anonymous</t:DistinguishedUser>
                      </t:UserId>
                      <t:PermissionLevel>None</t:PermissionLevel>
                    </t:Permission>
                    <t:Permission>
                      <t:UserId>
                        <t:PrimarySmtpAddress>sadie@contoso.com</t:PrimarySmtpAddress>
                      </t:UserId>
                      <t:PermissionLevel>Editor</t:PermissionLevel>
                    </t:Permission>
                  </t:Permissions>
                </t:PermissionSet>
              </t:Folder>
            </t:SetFolderField>
          </t:Updates>
        </t:FolderChange>
      </m:FolderChanges>
    </m:UpdateFolder>
  </soap:Body>
</soap:Envelope>
```

Следующая строка кода указывает уровень разрешений.
  
```xml
<t:Permission>
    <t:UserId>
        <t:PrimarySmtpAddress>sadie@contoso.com</t:PrimarySmtpAddress>
    </t:UserId>
    <t:PermissionLevel>Editor</t:PermissionLevel>
</t:Permission>
```

Если вы хотите использовать пользовательский уровень разрешений, используйте следующий код.
  
```xml
<t:Permission>
    <t:UserId>
        <t:PrimarySmtpAddress> sadie@contoso.com </t:PrimarySmtpAddress>
    </t:UserId>
    <t:CanCreateItems>true</t:CanCreateItems>
    <t:CanCreateSubFolders>true</t:CanCreateSubFolders>
    <t:IsFolderOwner>false</t:IsFolderOwner>
    <t:IsFolderVisible>false</t:IsFolderVisible>
    <t:IsFolderContact>false</t:IsFolderContact>
    <t:EditItems>None</t:EditItems>
    <t:DeleteItems>None</t:DeleteItems>
    <t:ReadItems>None</t:ReadItems>
    <t:PermissionLevel>Custom</t:PermissionLevel>
</t:Permission>
```

Сервер отвечает на запрос **UpdateFolder** с [UpdateFolderResponse](http://msdn.microsoft.com/library/31f47739-dc9c-46ba-9e3f-cce25dc85e6e%28Office.15%29.aspx) сообщения, которое содержит значение элемента [ResponseCode](http://msdn.microsoft.com/library/4b84d670-74c9-4d6d-84e7-f0a9f76f0d93%28Office.15%29.aspx) **NoError**, это означает, что папка успешно обновлены.
  
## <a name="removing-folder-permissions-by-using-the-ews-managed-api"></a>Удаление разрешений для папки с помощью управляемого интерфейса API веб-служб Exchange
<a name="bk_removeewsma"> </a>

В следующем примере кода показано, как использовать управляемый API веб-служб Exchange для удаления всех разрешений на доступ пользователей указанной папки, за исключением разрешения анонимного доступа и по умолчанию с:
  
1. Получение текущих разрешений для папки с помощью метода **привязки** . 
    
2. Итерации по коллекции **разрешения** и удаление разрешений для отдельных пользователей. 
    
3. Вызов метода **обновления** , чтобы сохранить изменения. 
    
В этом примере удаляются все разрешения на папку пользователя. Если требуется внести изменения в этом примере для удаления разрешений только для определенного пользователя, измените следующую строку кода для идентификации либо отображаемое имя или адрес SMTP пользователя.
  
```cs
if (sentItemsFolder.Permissions[t].UserId.DisplayName != null || sentItemsFolder.Permissions[t].UserId.PrimarySmtpAddress != null)
```

В этом примере предполагается, что эта **Служба** является допустимым объектом [ExchangeService](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.exchangeservice%28v=exchg.80%29.aspx) владельца почтового ящика, который пользователь прошел проверку подлинности на сервере Exchange. 
  
```cs
static void RemoveFolderPermissions(ExchangeService service)
{
    // Create a property set to use for folder binding.
    PropertySet propSet = new PropertySet(BasePropertySet.FirstClassProperties, FolderSchema.Permissions);
    // Bind to the folder and get the current permissions. 
    // This call results in a GetFolder call to EWS.
    Folder sentItemsFolder = Folder.Bind(service, new FolderId(WellKnownFolderName.SentItems, "primary@contoso.com"), propSet);
    // Iterate through the collection of permissions and remove permissions for any 
    // user with a display name or SMTP address. This leaves the anonymous and 
    // default user permissions unchanged. 
    if (sentItemsFolder.Permissions.Count != 0)
    {
        for (int t = 0; t < sentItemsFolder.Permissions.Count; t++)
        {
            // Find any permissions associated with the specified user and remove them from the DACL
            if (sentItemsFolder.Permissions[t].UserId.DisplayName != null || sentItemsFolder.Permissions[t].UserId.PrimarySmtpAddress != null)
            {
                sentItemsFolder.Permissions.Remove(sentItemsFolder.Permissions[t]);
            }
        }
    }
    // This call results in an UpdateFolder call to EWS.
    sentItemsFolder.Update();
}
```

## <a name="removing-folder-permissions-by-using-ews"></a>Удаление разрешений для папки с помощью веб-служб Exchange
<a name="bk_removeews"> </a>

В следующих примерах кода веб-служб Exchange показано, как удалить все разрешения пользователя на определенную папку, за исключением по умолчанию и разрешения для анонимных пользователей.
  
Во-первых отправьте запрос [GetFolder](http://msdn.microsoft.com/library/355bcf93-dc71-4493-b177-622afac5fdb9%28Office.15%29.aspx) , где значение [DistinguishedFolderId](http://msdn.microsoft.com/library/50018162-2941-4227-8a5b-d6b4686bb32f%28Office.15%29.aspx) указывает папку, в которой для удаления разрешений (папка Отправленные в данном примере), а значение [FieldURI](http://msdn.microsoft.com/library/24af8e3b-3074-4c8c-8d0a-52446508d044%28Office.15%29.aspx) включает в себя папки: PermissionSet. Этот запрос будет извлекать [PermissionSet](http://msdn.microsoft.com/library/6ac1bd17-a089-46bb-b9e6-f5b1dfe1076d%28Office.15%29.aspx) для указанной папки. 
  
Это также XML-запрос, который отправляет управляемый API EWS при вызове метода **привязки** для [удаления разрешений для папки](#bk_removeewsma).
  
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
        <t:BaseShape>AllProperties</t:BaseShape>
        <t:AdditionalProperties>
          <t:FieldURI FieldURI="folder:PermissionSet" />
        </t:AdditionalProperties>
      </m:FolderShape>
      <m:FolderIds>
        <t:DistinguishedFolderId Id="drafts">
          <t:Mailbox>
            <t:EmailAddress>primary@contoso.com</t:EmailAddress>
          </t:Mailbox>
        </t:DistinguishedFolderId>
      </m:FolderIds>
    </m:GetFolder>
  </soap:Body>
</soap:Envelope>
```

Сервер отвечает на запрос **GetFolder** [GetFolderResponse](http://msdn.microsoft.com/library/47abeec8-78dd-4297-8525-099174ec880d%28Office.15%29.aspx) сообщение, которое содержит значение элемента [ResponseCode](http://msdn.microsoft.com/library/4b84d670-74c9-4d6d-84e7-f0a9f76f0d93%28Office.15%29.aspx) **NoError**, это означает, что папка был успешно извлечен. Значения элементов **FolderId** и **ParentFolderId** URL-были сокращены для удобства чтения. 
  
```XML
<?xml version="1.0" encoding="utf-8"?>
<s:Envelope xmlns:s="http://schemas.xmlsoap.org/soap/envelope/">
  <s:Header>
    <h:ServerVersionInfo MajorVersion="15"
                         MinorVersion="0"
                         MajorBuildNumber="893"
                         MinorBuildNumber="17"
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
              <t:FolderId Id="EAAAAA=="
                          ChangeKey="AQAAABYAAADOilbYa8KaT7ZgMoTz2P+hAAABiRd5" />
              <t:ParentFolderId Id="CQAAAA=="
                                ChangeKey="AQAAAA==" />
              <t:FolderClass>IPF.Note</t:FolderClass>
              <t:DisplayName>Drafts</t:DisplayName>
              <t:TotalCount>0</t:TotalCount>
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
              <t:PermissionSet>
                <t:Permissions>
                  <t:Permission>
                    <t:UserId>
                      <t:DistinguishedUser>Default</t:DistinguishedUser>
                    </t:UserId>
                    <t:CanCreateItems>false</t:CanCreateItems>
                    <t:CanCreateSubFolders>false</t:CanCreateSubFolders>
                    <t:IsFolderOwner>false</t:IsFolderOwner>
                    <t:IsFolderVisible>false</t:IsFolderVisible>
                    <t:IsFolderContact>false</t:IsFolderContact>
                    <t:EditItems>None</t:EditItems>
                    <t:DeleteItems>None</t:DeleteItems>
                    <t:ReadItems>None</t:ReadItems>
                    <t:PermissionLevel>None</t:PermissionLevel>
                  </t:Permission>
                  <t:Permission>
                    <t:UserId>
                      <t:DistinguishedUser>Anonymous</t:DistinguishedUser>
                    </t:UserId>
                    <t:CanCreateItems>false</t:CanCreateItems>
                    <t:CanCreateSubFolders>false</t:CanCreateSubFolders>
                    <t:IsFolderOwner>false</t:IsFolderOwner>
                    <t:IsFolderVisible>false</t:IsFolderVisible>
                    <t:IsFolderContact>false</t:IsFolderContact>
                    <t:EditItems>None</t:EditItems>
                    <t:DeleteItems>None</t:DeleteItems>
                    <t:ReadItems>None</t:ReadItems>
                    <t:PermissionLevel>None</t:PermissionLevel>
                  </t:Permission>
                  <t:Permission>
                    <t:UserId>
                      <t:SID>S-1-5-21-1337771579-694202782-848329751-1535223</t:SID>
                      <t:PrimarySmtpAddress>sadie@Contoso.com</t:PrimarySmtpAddress>
                      <t:DisplayName>Sadie Daniels</t:DisplayName>
                    </t:UserId>
                    <t:CanCreateItems>true</t:CanCreateItems>
                    <t:CanCreateSubFolders>false</t:CanCreateSubFolders>
                    <t:IsFolderOwner>false</t:IsFolderOwner>
                    <t:IsFolderVisible>true</t:IsFolderVisible>
                    <t:IsFolderContact>false</t:IsFolderContact>
                    <t:EditItems>All</t:EditItems>
                    <t:DeleteItems>All</t:DeleteItems>
                    <t:ReadItems>FullDetails</t:ReadItems>
                    <t:PermissionLevel>Editor</t:PermissionLevel>
                  </t:Permission>
                </t:Permissions>
              </t:PermissionSet>
              <t:UnreadCount>0</t:UnreadCount>
            </t:Folder>
          </m:Folders>
        </m:GetFolderResponseMessage>
      </m:ResponseMessages>
    </m:GetFolderResponse>
  </s:Body>
</s:Envelope>
```

Затем используйте операцию **UpdateFolder** для отправки обновленные **PermissionSet**, которая не включает **разрешения** для удаленных пользователей. 
  
Это также XML-запрос, который отправляет управляемый API EWS при вызове метода **Update** для [удаления разрешений для папки](#bk_removeewsma).
  
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
          <t:FolderId Id="EAAAAA=="
                      ChangeKey="AQAAABYAAADOilbYa8KaT7ZgMoTz2P+hAAABiRd5" />
          <t:Updates>
            <t:SetFolderField>
              <t:FieldURI FieldURI="folder:PermissionSet" />
              <t:Folder>
                <t:PermissionSet>
                  <t:Permissions>
                    <t:Permission>
                      <t:UserId>
                        <t:DistinguishedUser>Default</t:DistinguishedUser>
                      </t:UserId>
                      <t:PermissionLevel>None</t:PermissionLevel>
                    </t:Permission>
                    <t:Permission>
                      <t:UserId>
                        <t:DistinguishedUser>Anonymous</t:DistinguishedUser>
                      </t:UserId>
                      <t:PermissionLevel>None</t:PermissionLevel>
                    </t:Permission>
                  </t:Permissions>
                </t:PermissionSet>
              </t:Folder>
            </t:SetFolderField>
          </t:Updates>
        </t:FolderChange>
      </m:FolderChanges>
    </m:UpdateFolder>
  </soap:Body>
</soap:Envelope>
```

Сервер отвечает на запрос **UpdateFolder** с **UpdateFolderResponse** сообщения, которое содержит значение элемента [ResponseCode](http://msdn.microsoft.com/library/4b84d670-74c9-4d6d-84e7-f0a9f76f0d93%28Office.15%29.aspx) **NoError**, это означает, что обновление выполнено успешно.
  
## <a name="updating-folder-permissions-by-using-the-ews-managed-api"></a>Обновление разрешений для папки с помощью управляемого интерфейса API веб-служб Exchange
<a name="bk_updateewsma"> </a>

Также можно обновить разрешения для папки для указанной папки с помощью управляемого интерфейса API веб-служб Exchange. Чтобы обновить разрешения: 
  
1. [Удаление разрешений папки](#bk_removeewsma) для устаревших разрешений, но не вызовите метод **Update** (пока). 
    
2. [Добавление разрешений для пользователей новые или измененные папки](#bk_enableewsma).
    
3. Вызовите метод **Update** для сохранения изменений. 
    
При попытке добавить два набора разрешений для одного пользователя, появится сообщение об ошибке **ServiceResponseException** с следующее описание: «набор указанное разрешение содержит повторяющиеся UserIds». В этом случае удалить текущие разрешения из набора **разрешений** , а затем добавить новые разрешения в коллекцию **разрешений** . 
  
## <a name="updating-folder-permissions-by-using-ews"></a>Обновление разрешений для папки с помощью веб-служб Exchange
<a name="bk_updateews"> </a>

Можно также обновить разрешения папок для конкретных папок с помощью веб-служб Exchange, объединяя в процессе удаления и добавления. Чтобы обновить разрешения: 
  
1. Получение разрешений текущей папки с помощью операции **GetFolder** . 
    
2. Отправьте обновленный список разрешений с помощью операции **UpdateFolder** . 
    
Далее представлены два такие же операции, используемые для [включения](#bk_enableews) или [удаления доступа](#bk_removeews) с помощью веб-служб Exchange. Единственное отличие заключается в том, что при получении ответа **GetFolder** она будет содержать **разрешений** для пользователя. Просто заменить существующий элемент **разрешение** новый элемент **разрешения** , а затем отправьте **UpdateFolder** операции с новое значение **разрешения** или значения. 
  
При попытке добавить два набора разрешений для одного пользователя, вы получите значение **ResponseCode** **ErrorDuplicateUserIdsSpecified**. В этом случае удалите значение устаревшие разрешения для пользователя из запроса и повторите попытку запроса.

## <a name="next-steps"></a>Дальнейшие действия

После предоставить пользователю разрешения в указанную папку, пользователь может получить доступ папку роли представителя. Для получения дополнительных сведений см.
  
- [Доступ к электронной почте в качестве делегата с помощью веб-служб Exchange в Exchange](how-to-access-email-as-a-delegate-by-using-ews-in-exchange.md)
    
- [Доступ к календарю в качестве делегата с помощью веб-служб Exchange в Exchange](how-to-access-a-calendar-as-a-delegate-by-using-ews-in-exchange.md)
    
- [Контакты доступа роли представителя с помощью веб-служб Exchange в Exchange](how-to-access-contacts-as-a-delegate-by-using-ews-in-exchange.md)
    
## <a name="see-also"></a>См. также

- [Передача прав доступа и EWS в Exchange](delegate-access-and-ews-in-exchange.md)   
- [Добавление и удаление делегаты с помощью веб-служб Exchange в Exchange](how-to-add-and-remove-delegates-by-using-ews-in-exchange.md)    
- [Папки и элементы в веб-службах Exchange](folders-and-items-in-ews-in-exchange.md)
    

