---
title: Установите разрешения папок для другого пользователя с помощью EWS в Exchange
manager: sethgros
ms.date: 03/9/2015
ms.audience: Developer
ms.localizationpriority: medium
ms.assetid: 7eb81676-a780-4c56-b4f2-c4ed2697107d
description: Узнайте, как установить уровни разрешений в папке с помощью управляемого API или EWS EWS в Exchange.
ms.openlocfilehash: 15288af0448a48c176529912604f628ae9bc2f19
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/24/2021
ms.locfileid: "59513089"
---
# <a name="set-folder-permissions-for-another-user-by-using-ews-in-exchange"></a>Установите разрешения папок для другого пользователя с помощью EWS в Exchange

Узнайте, как установить уровни разрешений в папке с помощью управляемого API или EWS EWS в Exchange.
  
Разрешения на уровне папок позволяют пользователям получать доступ к одной или более папок в почтовом ящике другого пользователя. Разрешения папок аналогичны делегированию доступа, но отличаются следующими способами: 
  
- Разрешения папок не позволяют пользователю "отправлять от имени" или "отправлять как" другого пользователя. Они позволяют получать доступ только к папкам. Пользователи могут создавать элементы в этих папках, но не могут отправлять их.
    
- Разрешения папок можно установить в любой папке в почтовом ящике, но можно добавить делегата только в папки "Календарь", "Контакты", "Входящие", "Журнал", "Заметки" и "Задачи".
    
- Вы можете установить ряд [разрешений в определенной папке.](#bk_folderperms) При добавлении делегата можно назначить один из пяти [уровней разрешений.](delegate-access-and-ews-in-exchange.md#bk_delegateperms)
    
- Вы можете установить разрешения папок для анонимных и по умолчанию пользователей. Вы можете предоставить только делегатский доступ к учетной записи с включенной почтой.
    
Если вы знакомы со списками управления доступом (ACEs) и Дискреционными списками управления доступом (DACLs), вы знаете, что у пользователя может быть только один набор разрешений для каждой папки. Если вы попробуете добавить набор разрешений для пользователя и у них уже есть набор разрешений, вы получите ошибку. При добавлении, удалите или обновите разрешения на папку, вы получите текущий DACL, добавьте или удалите все acEs, а затем отправьте обновленный DACL. Нельзя добавить несколько acEs для одного пользователя. При обновлении разрешений с помощью управляемого API EWS необходимо удалить текущий ACE пользователя, а затем добавить его новый ACE в коллекцию. Если вы используете EWS, просто замените предыдущий набор acEs новыми.
  
Если вы делаете несколько изменений разрешений в одной папке, вы можете пакетные добавления, удаления или обновления , просто обратите внимание, что вы не можете пакетные обновления пользователей в нескольких папок. Для получения разрешений в одной папке требуется один вызов, а для обновления разрешений в этой папке требуется второй вызов. При добавлении, удалите или обновите разрешения пользователей, для каждой задачи используются одинаковые два метода вызовов или операций.
  
**Таблица 1. Методы управляемого API EWS и операции EWS для установки разрешений папок**

|Что требуется сделать|Используйте этот метод управляемого API EWS...|Используйте эту операцию EWS...|
|:-----|:-----|:-----|
|Включить, удалить или обновить разрешения папок  <br/> |[Folder.Bind](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.folder.bind%28v=exchg.80%29.aspx) с [последующим обновлением folder.Update](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.emailmessage.reply%28v=exchg.80%29.aspx) <br/> |[GetFolder](https://msdn.microsoft.com/library/355bcf93-dc71-4493-b177-622afac5fdb9%28Office.15%29.aspx) с [последующим обновлениемFolder](https://msdn.microsoft.com/library/3494c996-b834-4813-b1ca-d99642d8b4e7%28Office.15%29.aspx) <br/> |
|Создание папки и определение разрешений папок  <br/> |[Folder.Save](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.folder.save%28v=exchg.80%29.aspx) <br/> |[CreateFolder](https://msdn.microsoft.com/library/6f6c334c-b190-4e55-8f0a-38f2a018d1b3%28Office.15%29.aspx) <br/> |
   
## <a name="folder-permissions"></a>Разрешения для папок
<a name="bk_folderperms"> </a>

У вас есть довольно много вариантов, когда дело доходит до установки разрешений папок в определенной папке. Вы можете установить уровень разрешений в папке для каждого пользователя, который добавляет набор заранее установленных отдельных разрешений в DACL, или вы можете установить отдельные разрешения на папку , но вы не можете смешивать и соответствовать.
  
Доступны следующие отдельные разрешения:
  
- Можно создать
- Может создавать подмостки    
- Является ли владелец папки    
- Отображается ли папка    
- Контакт папки    
- Изменение элементов    
- Удаление элементов    
- Чтение элементов
    
Кроме того, доступны следующие уровни разрешений, которые определяют подмножество отдельных разрешений и значений, как показано в таблице 2:
  
- Нет    
- Владелец    
- PublishingEditor    
- Редактор    
- PublishingAuthor    
- Автор    
- NoneditingAuthor    
- Reviewer    
- Участник   
- Настраиваемый . Это значение не может быть установлено приложением. Сервер задает это значение, если приложение включает настраиваемую коллекцию отдельных разрешений.    
- FreeBusyTimeOnly . Это можно установить только в папках Calendar.   
- FreeBusyTimeAndSubjectAndAndLocation — это может быть установлено только в папках Calendar.
    
В следующей таблице показано, какие отдельные разрешения применяются по умолчанию на основе уровня разрешений.
  
**Таблица 2. Отдельные разрешения по уровню разрешений**

|Уровень разрешений.|Может создавать элементы|Можно создать папки sub|Является ли владелец папки|Отображается ли папка|Контакт папки|Изменение элементов|Удаление элементов|Может читать элементы|
|:-----|:-----|:-----|:-----|:-----|:-----|:-----|:-----|:-----|
|Нет  <br/> |Неверно  <br/> |Неверно  <br/> |Неверно  <br/> |Неверно  <br/> |Неверно  <br/> |Нет  <br/> |Нет  <br/> |Нет  <br/> |
|Владелец  <br/> |Да  <br/> |Да  <br/> |Да  <br/> |Да  <br/> |Да  <br/> |Все  <br/> |Все  <br/> |FullDetails  <br/> |
|PublishingEditor  <br/> |Да  <br/> |Да  <br/> |False  <br/> |Да  <br/> |Неверно  <br/> |Все  <br/> |Все  <br/> |FullDetails  <br/> |
|Редактор  <br/> |Верно  <br/> |Неверно  <br/> |False  <br/> |Да  <br/> |Неверно  <br/> |Все  <br/> |Все  <br/> |FullDetails  <br/> |
|PublishingAuthor  <br/> |Да  <br/> |Да  <br/> |False  <br/> |Да  <br/> |Неверно  <br/> |Owned  <br/> |Owned  <br/> |FullDetails  <br/> |
|Автор  <br/> |Верно  <br/> |Неверно  <br/> |False  <br/> |Да  <br/> |Неверно  <br/> |Owned  <br/> |Owned  <br/> |FullDetails  <br/> |
|NoneditingAuthor  <br/> |Верно  <br/> |Неверно  <br/> |False  <br/> |Да  <br/> |Неверно  <br/> |Нет  <br/> |Owned  <br/> |FullDetails  <br/> |
|Reviewer  <br/> |Неверно  <br/> |Неверно  <br/> |False  <br/> |Да  <br/> |Неверно  <br/> |Нет  <br/> |Нет  <br/> |FullDetails  <br/> |
|Участник  <br/> |Верно  <br/> |Неверно  <br/> |False  <br/> |Да  <br/> |Неверно  <br/> |Нет  <br/> |Нет  <br/> |Нет  <br/> |
   
Если в запросе разрешений на уровне папок указывается нестандартный уровень разрешений, не нужно указывать отдельные параметры разрешений. Если вы укажите отдельное разрешение при задании уровня разрешений, в ответ будет возвращена ошибка **ErrorInvalidPermissionSettings.** 
  
## <a name="adding-folder-permissions-by-using-the-ews-managed-api"></a>Добавление разрешений папок с помощью управляемого API EWS
<a name="bk_enableewsma"> </a>

В следующем примере кода показано, как использовать управляемый API EWS для: 
  
- Создайте новый [объект FolderPermission](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.folderpermission%28v=exchg.80%29.aspx) для нового пользователя. 
    
- Получите текущие разрешения для папки с помощью метода [Bind.](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.folder.bind%28v=exchg.80%29.aspx) 
    
- Добавьте новые **folderPermissions в** свойство [Folder.Permissions.](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.folder.permissions%28v=exchg.80%29.aspx) 
    
- Вызов метода [Update,](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.folder.update%28v=exchg.80%29.aspx) чтобы сохранить новые разрешения на сервер. 
    
В этом примере предполагается, что служба является допустимым объектом [ExchangeService](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.exchangeservice%28v=exchg.80%29.aspx) для владельца почтового ящика и что пользователь был аутентификацией Exchange сервера.  
  
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

Если вы хотите использовать настраиваемый уровень разрешений, используйте этот код.
  
```cs
FolderPermission fldperm = new FolderPermission();
fldperm.UserId = "sadie@Contoso1000.onmicrosoft.com";
fldperm.CanCreateItems = true;
fldperm.CanCreateSubFolders = true;
…
```

При создании объекта [FolderPermission](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.folderpermission_properties%28v=exchg.80%29.aspx) с настраиваемым уровнем разрешений можно установить любые или все свойства writable **FolderPermission.** Обратите внимание, однако, что [folderPermissionLevel](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.folderpermissionlevel%28v=exchg.80%29.aspx) никогда  явно не за набор настраивается приложением. **FolderPermissionLevel** настраивается только при создании объекта **FolderPermission** и наборе отдельных разрешений. 
  
## <a name="adding-folder-permissions-by-using-ews"></a>Добавление разрешений папок с помощью EWS
<a name="bk_enableews"> </a>

В следующих примерах кода EWS покажите, как добавлять разрешения в определенную папку, ирисовка текущих разрешений и отправка списка новых разрешений.
  
Первым шагом является отправка запроса [GetFolder,](https://msdn.microsoft.com/library/355bcf93-dc71-4493-b177-622afac5fdb9%28Office.15%29.aspx) в котором значение [DistinguishedFolderId](https://msdn.microsoft.com/library/50018162-2941-4227-8a5b-d6b4686bb32f%28Office.15%29.aspx) указывает папку, в которой необходимо добавить разрешения (папка отправленных элементов в этом примере), а значение [FieldURI](https://msdn.microsoft.com/library/24af8e3b-3074-4c8c-8d0a-52446508d044%28Office.15%29.aspx) включает папку:PermissionSet. Этот запрос позволит получить параметры разрешений для указанной папки. 
  
Это также XML-запрос, который отправляет управляемый API EWS при вызове метода **Bind** для добавления разрешений [папок.](#bk_enableewsma)
  
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

Сервер отвечает на запрос **GetFolder** с сообщением [GetFolderResponse,](https://msdn.microsoft.com/library/47abeec8-78dd-4297-8525-099174ec880d%28Office.15%29.aspx) которое включает в себя значение элемента [ResponseCode](https://msdn.microsoft.com/library/4b84d670-74c9-4d6d-84e7-f0a9f76f0d93%28Office.15%29.aspx) **NoError,** что указывает на успешное извлечение папки. Значения [FolderId](https://msdn.microsoft.com/library/00d14e3e-4365-4f21-8f88-eaeea73b9bf7%28Office.15%29.aspx) и [ParentFolderId](https://msdn.microsoft.com/library/258f4b1f-367e-4c7d-9c29-eb775a2398c7%28Office.15%29.aspx) были сокращены для читаемости. 
  
```XML
<?xml version="1.0" encoding="utf-8"?>
<s:Envelope xmlns:s="https://schemas.xmlsoap.org/soap/envelope/">
  <s:Header>
    <h:ServerVersionInfo MajorVersion="15"
                         MinorVersion="0"
                         MajorBuildNumber="893"
                         MinorBuildNumber="17"
                         Version="V2_10"
                         xmlns:h="https://schemas.microsoft.com/exchange/services/2006/types"
                         xmlns="https://schemas.microsoft.com/exchange/services/2006/types"
                         xmlns:xsd="http://www.w3.org/2001/XMLSchema"
                         xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" />
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

Далее используйте **операцию UpdateFolder** для отправки обновленного [PermissionSet,](https://msdn.microsoft.com/library/6ac1bd17-a089-46bb-b9e6-f5b1dfe1076d%28Office.15%29.aspx)который включает [разрешение](https://msdn.microsoft.com/library/b8d0429a-0e58-4480-9847-4901970c7033%28Office.15%29.aspx) для нового пользователя. Обратите внимание, что в том числе элемент [SetFolderField](https://msdn.microsoft.com/library/8c69db7b-54b5-4ae2-abca-4d6e0937a790%28Office.15%29.aspx) для соответствующей папки в операции [UpdateFolder](https://msdn.microsoft.com/library/3494c996-b834-4813-b1ca-d99642d8b4e7%28Office.15%29.aspx) будет перезаписывать все параметры разрешений в папке. Кроме того, в том числе параметр [DeleteFolderField](https://msdn.microsoft.com/library/f9c2187b-4c60-4358-b4b4-ede50eadae48%28Office.15%29.aspx) операции **UpdateFolder** также удаляет все параметры разрешений в папке. 
  
Это также XML-запрос, который отправляет управляемый API EWS при вызове метода **Update** для добавления разрешений [папок.](#bk_enableewsma)
  
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

Если вы хотите использовать настраиваемый уровень разрешений, используйте этот код.
  
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

Сервер отвечает на запрос **UpdateFolder** [сообщением UpdateFolderResponse,](https://msdn.microsoft.com/library/31f47739-dc9c-46ba-9e3f-cce25dc85e6e%28Office.15%29.aspx) которое включает элемент [ResponseCode](https://msdn.microsoft.com/library/4b84d670-74c9-4d6d-84e7-f0a9f76f0d93%28Office.15%29.aspx) значения **NoError,** что указывает на успешное обновление папки.
  
## <a name="removing-folder-permissions-by-using-the-ews-managed-api"></a>Удаление разрешений папок с помощью управляемого API EWS
<a name="bk_removeewsma"> </a>

В следующем примере кода показано, как использовать управляемый API EWS для удаления всех разрешений пользователей в определенной папке, за исключением разрешений по умолчанию и анонимных, путем:
  
1. Получение текущих разрешений для папки с помощью метода **Bind.** 
    
2. Итерирование через коллекцию **Разрешений** и удаление разрешений для отдельных пользователей. 
    
3. Вызов метода **Update** для сохранения изменений. 
    
В этом примере удаляются все разрешения пользователей в папке. Если вы хотите изменить этот пример, чтобы удалить разрешения только для конкретного пользователя, измените следующую строку кода, чтобы определить имя отображения или SMTP-адрес пользователя.
  
```cs
if (sentItemsFolder.Permissions[t].UserId.DisplayName != null || sentItemsFolder.Permissions[t].UserId.PrimarySmtpAddress != null)
```

В этом примере предполагается, что служба является допустимым объектом [ExchangeService](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.exchangeservice%28v=exchg.80%29.aspx) для владельца почтового ящика и что пользователь был аутентификацией Exchange сервера.  
  
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

## <a name="removing-folder-permissions-by-using-ews"></a>Удаление разрешений папок с помощью EWS
<a name="bk_removeews"> </a>

В следующих примерах кода EWS покажите, как удалить все разрешения пользователей в определенной папке, за исключением разрешений по умолчанию и анонимных.
  
Сначала отправьте запрос [GetFolder,](https://msdn.microsoft.com/library/355bcf93-dc71-4493-b177-622afac5fdb9%28Office.15%29.aspx) в котором значение [DistinguishedFolderId](https://msdn.microsoft.com/library/50018162-2941-4227-8a5b-d6b4686bb32f%28Office.15%29.aspx) указывает папку, в которой удаляются разрешения (папка отправленных элементов в этом примере), а значение [FieldURI](https://msdn.microsoft.com/library/24af8e3b-3074-4c8c-8d0a-52446508d044%28Office.15%29.aspx) включает папку:PermissionSet. Этот запрос позволит получить [PermissionSet для](https://msdn.microsoft.com/library/6ac1bd17-a089-46bb-b9e6-f5b1dfe1076d%28Office.15%29.aspx) указанной папки. 
  
Это также XML-запрос, который отправляет управляемый API EWS при вызове метода **Bind** для удаления разрешений [папок.](#bk_removeewsma)
  
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

Сервер отвечает на запрос **GetFolder** с сообщением [GetFolderResponse,](https://msdn.microsoft.com/library/47abeec8-78dd-4297-8525-099174ec880d%28Office.15%29.aspx) которое включает в себя значение элемента [ResponseCode](https://msdn.microsoft.com/library/4b84d670-74c9-4d6d-84e7-f0a9f76f0d93%28Office.15%29.aspx) **NoError,** что указывает на успешное извлечение папки. Для читаемости сокращены значения элементов **FolderId** и **ParentFolderId.** 
  
```XML
<?xml version="1.0" encoding="utf-8"?>
<s:Envelope xmlns:s="https://schemas.xmlsoap.org/soap/envelope/">
  <s:Header>
    <h:ServerVersionInfo MajorVersion="15"
                         MinorVersion="0"
                         MajorBuildNumber="893"
                         MinorBuildNumber="17"
                         Version="V2_10"
                         xmlns:h="https://schemas.microsoft.com/exchange/services/2006/types"
                         xmlns="https://schemas.microsoft.com/exchange/services/2006/types"
                         xmlns:xsd="http://www.w3.org/2001/XMLSchema"
                         xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" />
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

Далее используйте **операцию UpdateFolder** для отправки обновленного  **PermissionSet,** который не включает разрешение для удаленного пользователя. 
  
Это также XML-запрос, который отправляет управляемый API EWS при вызове метода **Update** для удаления разрешений [папок.](#bk_removeewsma)
  
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

Сервер отвечает на запрос **UpdateFolder** **сообщением UpdateFolderResponse,** которое включает значение элемента [ResponseCode](https://msdn.microsoft.com/library/4b84d670-74c9-4d6d-84e7-f0a9f76f0d93%28Office.15%29.aspx) **NoError,** которое указывает на успешность обновления.
  
## <a name="updating-folder-permissions-by-using-the-ews-managed-api"></a>Обновление разрешений папок с помощью управляемого API EWS
<a name="bk_updateewsma"> </a>

Вы также можете обновить разрешения папок для определенной папки с помощью управляемого API EWS. Чтобы обновить разрешения: 
  
1. [Удалите разрешения папок](#bk_removeewsma) для устаревших разрешений, но не вызывайте метод **Update** (пока). 
    
2. [Добавление разрешений папок для новых или измененных пользователей.](#bk_enableewsma)
    
3. Чтобы **сохранить** изменения, вызываем метод Update. 
    
Если вы попробуете добавить два набора разрешений для одного пользователя, вы получите ошибку **ServiceResponseException** со следующим описанием: "Указанный набор разрешений содержит дубликаты UserIds". В этом случае удалите текущие разрешения из коллекции **разрешений,** а затем добавьте новые разрешения **в** коллекцию разрешений. 
  
## <a name="updating-folder-permissions-by-using-ews"></a>Обновление разрешений папок с помощью EWS
<a name="bk_updateews"> </a>

Кроме того, можно обновить разрешения папок для определенных папок с помощью EWS, объединив процесс удаления и добавления. Чтобы обновить разрешения: 
  
1. Извлечение текущих разрешений папки с помощью **операции GetFolder.** 
    
2. Отправьте обновленный список разрешений с помощью операции **UpdateFolder.** 
    
Это те же две операции, которые вы используете, чтобы [включить](#bk_enableews) или [удалить доступ](#bk_removeews) с помощью EWS. Единственное отличие состоит в том, что при приеме **ответа GetFolder** он будет содержать **набор** разрешений для пользователя. Просто замените существующий элемент **Permission** новым элементом **Permission** и отправьте операцию **UpdateFolder** новым значением **или** значениями разрешения. 
  
Если вы попробуете добавить два набора разрешений для одного пользователя, вы получите значение **ResponseCode** **errorDuplicateUserIdsSpecified.** В этом случае удалите устаревшее значение разрешения для пользователя из запроса, а затем повторно обнажите запрос.

## <a name="next-steps"></a>Дальнейшие действия

После получения разрешения пользователя в определенной папке пользователь может получить доступ к папке в качестве делегата. Дополнительные сведения см. в статьях:
  
- [Доступ к электронной почте в качестве делегата с помощью EWS в Exchange](how-to-access-email-as-a-delegate-by-using-ews-in-exchange.md)
    
- [Доступ к календарю в качестве делегата с помощью EWS в Exchange](how-to-access-a-calendar-as-a-delegate-by-using-ews-in-exchange.md)
    
- [Доступ к контактам в качестве делегата с помощью EWS в Exchange](how-to-access-contacts-as-a-delegate-by-using-ews-in-exchange.md)
    
## <a name="see-also"></a>См. также

- [Передача прав доступа и EWS в Exchange](delegate-access-and-ews-in-exchange.md)   
- [Добавление и удаление делегатов с помощью EWS в Exchange](how-to-add-and-remove-delegates-by-using-ews-in-exchange.md)    
- [Папки и элементы в веб-службах Exchange](folders-and-items-in-ews-in-exchange.md)
    

