---
title: Задание разрешений для папки другого пользователя с помощью EWS в Exchange
manager: sethgros
ms.date: 03/9/2015
ms.audience: Developer
localization_priority: Normal
ms.assetid: 7eb81676-a780-4c56-b4f2-c4ed2697107d
description: Узнайте, как задать уровни разрешений для папки с помощью управляемого API EWS или EWS в Exchange.
ms.openlocfilehash: e25f1a49a430e8c95829d404fa53451b76cab167
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/03/2020
ms.locfileid: "44455872"
---
# <a name="set-folder-permissions-for-another-user-by-using-ews-in-exchange"></a>Задание разрешений для папки другого пользователя с помощью EWS в Exchange

Узнайте, как задать уровни разрешений для папки с помощью управляемого API EWS или EWS в Exchange.
  
Разрешения уровня папки позволяют пользователям получать доступ к одной или нескольким папкам в почтовом ящике другого пользователя. Разрешения для папок аналогичны Делегированному доступу, но они отличаются следующими особенностями: 
  
- Разрешения для папок не позволяют пользователю "Отправить от имени" или "Отправить как" другого пользователя. Они позволяют получать доступ только к папкам. Пользователи могут создавать элементы в этих папках, но не могут их отправлять.
    
- Вы можете задать разрешения для папки в любой папке почтового ящика, но вы можете добавить делегата в папки "Календарь", "Контакты", "Входящие", "журнал", "Заметки" и "задачи".
    
- Вы можете задать ряд [разрешений для конкретной папки](#bk_folderperms). При добавлении делегата можно назначить один из [пяти уровней разрешений](delegate-access-and-ews-in-exchange.md#bk_delegateperms).
    
- Вы можете задать разрешения для папок анонимных пользователей и пользователей по умолчанию. Вы можете предоставить представителю доступ только к учетной записи с включенной поддержкой почты.
    
Если вы знакомы с записями управления доступом и избирательными списками управления доступом (DACL), то вы знаете, что у пользователя может быть только один набор разрешений для каждой папки. Если вы попытаетесь добавить набор разрешений для пользователя и у него уже есть набор разрешений, возникнет ошибка. При добавлении, удалении или обновлении разрешений для папки вы получаете текущий список DACL, добавляете или удаляете все записи управления доступом, а затем отправляете обновленный список DACL. Вы не можете добавить несколько элементов управления доступом для одного и того же пользователя. При обновлении разрешений с помощью управляемого API EWS необходимо удалить текущую запись ACE пользователя, а затем добавить в нее новый элемент управления доступом. Если вы используете EWS, вы просто замените предыдущий набор записей ACE на новые.
  
Если вы вносите несколько изменений разрешений в одну папку, вы можете пакетным добавлением, удалением или обновлениям, просто обратите внимание на то, что вы не можете выполнять пакетное обновление для нескольких папок. Один вызов необходим для получения разрешений для одной папки, а второй вызов необходим для обновления разрешений для этой папки. При добавлении, удалении или обновлении разрешений пользователя используются одинаковые два вызова метода или операции для каждой задачи.
  
**Таблица 1. Методы управляемого API EWS и операции EWS для установки разрешений для папки**

|Что требуется сделать|Используйте этот метод управляемого API EWS...|Используйте эту операцию EWS...|
|:-----|:-----|:-----|
|Включение, удаление и обновление разрешений для папки  <br/> |[Folder. Bind](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.folder.bind%28v=exchg.80%29.aspx) , за которым следует [Папка. Update](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.emailmessage.reply%28v=exchg.80%29.aspx) <br/> |[Папка](https://msdn.microsoft.com/library/355bcf93-dc71-4493-b177-622afac5fdb9%28Office.15%29.aspx) , за которой следует [операцию UpdateFolder](https://msdn.microsoft.com/library/3494c996-b834-4813-b1ca-d99642d8b4e7%28Office.15%29.aspx) <br/> |
|Создание папки и определение разрешений для папки  <br/> |[Folder. Save](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.folder.save%28v=exchg.80%29.aspx) <br/> |[CreateFolder](https://msdn.microsoft.com/library/6f6c334c-b190-4e55-8f0a-38f2a018d1b3%28Office.15%29.aspx) <br/> |
   
## <a name="folder-permissions"></a>Разрешения для папок
<a name="bk_folderperms"> </a>

При настройке разрешений для папки в определенной папке есть несколько вариантов. Вы можете задать уровень разрешений для папки для каждого пользователя, который добавляет набор предварительно определенных разрешений в список DACL или устанавливает индивидуальные разрешения для папки, но не позволяет смешивать и сопоставлять их.
  
Доступны следующие отдельные разрешения:
  
- Могут создавать
- Может создавать вложенные папки    
- Является владельцем папки    
- Является видимой папкой    
- Является контактом папки    
- Изменение элементов    
- удалять элементы.    
- Чтение элементов
    
Кроме того, доступны следующие уровни разрешений, которые определяют подмножество отдельных разрешений и значений, как показано в таблице 2:
  
- Нет    
- Владелец    
- PublishingEditor    
- Корректор    
- PublishingAuthor    
- Автор    
- Noneditingauthorcreateitems    
- Reviewer    
- Участник   
- Custom — это значение не может быть задано приложением. Сервер задает это значение, если приложение включает настраиваемую коллекцию отдельных разрешений.    
- Фрибуситимеонли — можно задать только для папок календаря.   
- Фрибуситимеандсубжектандлокатион — можно задать только для папок календаря.
    
В следующей таблице показано, какие индивидуальные разрешения применяются по умолчанию на основе уровня разрешений.
  
**Таблица 2. Индивидуальные разрешения по уровню разрешений**

|Уровень разрешений|Может создавать элементы|Может создавать вложенные папки|Является владельцем папки|Является видимой папкой|Является контактом папки|Изменение элементов|удалять элементы.|Возможность чтения элементов|
|:-----|:-----|:-----|:-----|:-----|:-----|:-----|:-----|:-----|
|Нет  <br/> |False  <br/> |False  <br/> |False  <br/> |False  <br/> |False  <br/> |Нет  <br/> |Нет  <br/> |Нет  <br/> |
|Владелец  <br/> |Да  <br/> |Да  <br/> |Да  <br/> |Да  <br/> |Да  <br/> |Все  <br/> |Все  <br/> |фуллдетаилс  <br/> |
|PublishingEditor  <br/> |Да  <br/> |Да  <br/> |False  <br/> |Верно.  <br/> |False  <br/> |Все  <br/> |Все  <br/> |фуллдетаилс  <br/> |
|Корректор  <br/> |Верно.  <br/> |False  <br/> |False  <br/> |Верно.  <br/> |False  <br/> |Все  <br/> |Все  <br/> |фуллдетаилс  <br/> |
|PublishingAuthor  <br/> |Да  <br/> |Да  <br/> |False  <br/> |Верно.  <br/> |False  <br/> |Он  <br/> |Он  <br/> |фуллдетаилс  <br/> |
|Автор  <br/> |Верно.  <br/> |False  <br/> |False  <br/> |Верно.  <br/> |False  <br/> |Он  <br/> |Он  <br/> |фуллдетаилс  <br/> |
|Noneditingauthorcreateitems  <br/> |Верно.  <br/> |False  <br/> |False  <br/> |Верно.  <br/> |False  <br/> |Нет  <br/> |Он  <br/> |фуллдетаилс  <br/> |
|Reviewer  <br/> |False  <br/> |False  <br/> |False  <br/> |Верно.  <br/> |False  <br/> |Нет  <br/> |Нет  <br/> |фуллдетаилс  <br/> |
|Участник  <br/> |Верно.  <br/> |False  <br/> |False  <br/> |Верно.  <br/> |False  <br/> |Нет  <br/> |Нет  <br/> |Нет  <br/> |
   
Если вы укажете ненастраиваемый уровень разрешений в запросе разрешений на уровне папки, вам не нужно указывать индивидуальные параметры разрешений. Если вы задаете отдельное разрешение, когда вы задаете уровень разрешений, в отклике будет возвращена ошибка **ерроринвалидпермиссионсеттингс** . 
  
## <a name="adding-folder-permissions-by-using-the-ews-managed-api"></a>Добавление разрешений для папки с помощью управляемого API EWS
<a name="bk_enableewsma"> </a>

В приведенном ниже примере кода показано, как использовать управляемый API EWS для: 
  
- Создайте новый объект [фолдерпермиссион](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.folderpermission%28v=exchg.80%29.aspx) для нового пользователя. 
    
- Получение текущих разрешений для папки с помощью метода [BIND](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.folder.bind%28v=exchg.80%29.aspx) . 
    
- Добавьте новый **фолдерпермиссионс** в свойство [Folder. Permissions](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.folder.permissions%28v=exchg.80%29.aspx) . 
    
- Вызовите метод [Update](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.folder.update%28v=exchg.80%29.aspx) , чтобы сохранить новые разрешения на сервере. 
    
В этом примере предполагается, что **Служба** является допустимым объектом [ExchangeService](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.exchangeservice%28v=exchg.80%29.aspx) для владельца почтового ящика, а пользователь прошел проверку подлинности на сервере Exchange. 
  
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

В следующей строке кода указывается уровень разрешений.
  
```cs
    FolderPermission fldperm = new FolderPermission("sadie@contoso.com", FolderPermissionLevel.Editor);
```

Если вы хотите использовать пользовательский уровень разрешений, используйте вместо этого этот код.
  
```cs
FolderPermission fldperm = new FolderPermission();
fldperm.UserId = "sadie@Contoso1000.onmicrosoft.com";
fldperm.CanCreateItems = true;
fldperm.CanCreateSubFolders = true;
…
```

Вы можете задать любое или все доступные для записи [Свойства фолдерпермиссион](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.folderpermission_properties%28v=exchg.80%29.aspx) при создании объекта **фолдерпермиссион** с пользовательским уровнем разрешений. Однако обратите внимание, что [фолдерпермиссионлевел](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.folderpermissionlevel%28v=exchg.80%29.aspx) не имеет явное значение, **настраиваемое** приложением. Для **фолдерпермиссионлевел** задано значение Custom только при создании объекта **фолдерпермиссион** и настройке отдельных разрешений. 
  
## <a name="adding-folder-permissions-by-using-ews"></a>Добавление разрешений для папки с помощью EWS
<a name="bk_enableews"> </a>

В следующих примерах кода EWS показано, как добавить разрешения в определенную папку, получая текущие разрешения, а затем отправляя список новых разрешений.
  
Первый шаг — Отправка запроса на получение [папки](https://msdn.microsoft.com/library/355bcf93-dc71-4493-b177-622afac5fdb9%28Office.15%29.aspx) , где значение [дистингуишедфолдерид](https://msdn.microsoft.com/library/50018162-2941-4227-8a5b-d6b4686bb32f%28Office.15%29.aspx) указывает папку, в которую добавляются разрешения (папка "Отправленные" в этом примере), а значение [фиелдури](https://msdn.microsoft.com/library/24af8e3b-3074-4c8c-8d0a-52446508d044%28Office.15%29.aspx) включает в себя папку: набор разрешений. Этот запрос получает параметры разрешений для указанной папки. 
  
Это также запрос XML, который отправляет управляемый API EWS при вызове метода **BIND** для [добавления разрешений для папки](#bk_enableewsma).
  
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

Сервер отвечает на запрос к **папке** жетфолдерреспонсе с сообщением [GetFolderResponse](https://msdn.microsoft.com/library/47abeec8-78dd-4297-8525-099174ec880d%28Office.15%29.aspx) , которое содержит значение **ошибки**элемента [респонсекоде](https://msdn.microsoft.com/library/4b84d670-74c9-4d6d-84e7-f0a9f76f0d93%28Office.15%29.aspx) , которое указывает, что папка была получена успешно. Значения [FolderId](https://msdn.microsoft.com/library/00d14e3e-4365-4f21-8f88-eaeea73b9bf7%28Office.15%29.aspx) и [ParentFolderId](https://msdn.microsoft.com/library/258f4b1f-367e-4c7d-9c29-eb775a2398c7%28Office.15%29.aspx) были сокращены для удобочитаемости. 
  
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

Затем используйте операцию **операцию UpdateFolder** , чтобы отправить обновленный уровень [разрешений](https://msdn.microsoft.com/library/6ac1bd17-a089-46bb-b9e6-f5b1dfe1076d%28Office.15%29.aspx), включающий [разрешение](https://msdn.microsoft.com/library/b8d0429a-0e58-4480-9847-4901970c7033%28Office.15%29.aspx) для нового пользователя. Обратите внимание, что при включении элемента [сетфолдерфиелд](https://msdn.microsoft.com/library/8c69db7b-54b5-4ae2-abca-4d6e0937a790%28Office.15%29.aspx) для соответствующей папки в операции [операцию UpdateFolder](https://msdn.microsoft.com/library/3494c996-b834-4813-b1ca-d99642d8b4e7%28Office.15%29.aspx) все параметры разрешений для папки будут перезаписаны. Аналогично, при включении параметра [делетефолдерфиелд](https://msdn.microsoft.com/library/f9c2187b-4c60-4358-b4b4-ede50eadae48%28Office.15%29.aspx) операции **операцию UpdateFolder** также будут удалены все параметры разрешений для папки. 
  
Это также запрос XML, который отправляет управляемый API EWS при вызове метода **Update** для [добавления разрешений для папки](#bk_enableewsma).
  
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

В следующей строке кода указывается уровень разрешений.
  
```xml
<t:Permission>
    <t:UserId>
        <t:PrimarySmtpAddress>sadie@contoso.com</t:PrimarySmtpAddress>
    </t:UserId>
    <t:PermissionLevel>Editor</t:PermissionLevel>
</t:Permission>
```

Если вы хотите использовать пользовательский уровень разрешений, используйте вместо этого этот код.
  
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

Сервер отвечает на запрос **операцию UpdateFolder** с сообщением [упдатефолдерреспонсе](https://msdn.microsoft.com/library/31f47739-dc9c-46ba-9e3f-cce25dc85e6e%28Office.15%29.aspx) , которое содержит значение **ошибки**элемента [респонсекоде](https://msdn.microsoft.com/library/4b84d670-74c9-4d6d-84e7-f0a9f76f0d93%28Office.15%29.aspx) , которое указывает, что папка обновлена успешно.
  
## <a name="removing-folder-permissions-by-using-the-ews-managed-api"></a>Удаление разрешений для папки с помощью управляемого API EWS
<a name="bk_removeewsma"> </a>

В приведенном ниже примере кода показано, как использовать управляемый API EWS для удаления всех разрешений пользователя в определенной папке, за исключением разрешений по умолчанию и анонимности:
  
1. Извлечение текущих разрешений для папки с помощью метода **BIND** . 
    
2. Итерация по коллекции **разрешений** и удаление разрешений для отдельных пользователей. 
    
3. Вызов метода **Update** для сохранения изменений. 
    
В этом примере удаляются все разрешения пользователя на папку. Если вы хотите изменить этот пример, чтобы удалить разрешения только для определенного пользователя, измените следующую строку кода, чтобы определить отображаемое имя или SMTP-адрес пользователя.
  
```cs
if (sentItemsFolder.Permissions[t].UserId.DisplayName != null || sentItemsFolder.Permissions[t].UserId.PrimarySmtpAddress != null)
```

В этом примере предполагается, что **Служба** является допустимым объектом [ExchangeService](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.exchangeservice%28v=exchg.80%29.aspx) для владельца почтового ящика, а пользователь прошел проверку подлинности на сервере Exchange. 
  
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

## <a name="removing-folder-permissions-by-using-ews"></a>Удаление разрешений для папки с помощью EWS
<a name="bk_removeews"> </a>

В следующих примерах кода EWS показано, как удалить все разрешения пользователя для конкретной папки, за исключением разрешений по умолчанию и анонимности.
  
Сначала отправьте запрос на получение [папки](https://msdn.microsoft.com/library/355bcf93-dc71-4493-b177-622afac5fdb9%28Office.15%29.aspx) , где значение [дистингуишедфолдерид](https://msdn.microsoft.com/library/50018162-2941-4227-8a5b-d6b4686bb32f%28Office.15%29.aspx) указывает папку для удаления разрешений (папка "Отправленные" в этом примере), а значение [Фиелдури](https://msdn.microsoft.com/library/24af8e3b-3074-4c8c-8d0a-52446508d044%28Office.15%29.aspx) включает папку: набор разрешений. Этот запрос получает заданный для папки уровень [разрешений](https://msdn.microsoft.com/library/6ac1bd17-a089-46bb-b9e6-f5b1dfe1076d%28Office.15%29.aspx) . 
  
Это также запрос XML, который отправляет управляемый API EWS при вызове метода **BIND** для [удаления разрешений для папки](#bk_removeewsma).
  
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

Сервер отвечает на запрос к **папке** жетфолдерреспонсе с сообщением [GetFolderResponse](https://msdn.microsoft.com/library/47abeec8-78dd-4297-8525-099174ec880d%28Office.15%29.aspx) , которое содержит значение **ошибки**элемента [респонсекоде](https://msdn.microsoft.com/library/4b84d670-74c9-4d6d-84e7-f0a9f76f0d93%28Office.15%29.aspx) , которое указывает, что папка была получена успешно. Значения элементов **FolderId** и **ParentFolderId** были сокращены для удобочитаемости. 
  
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

Затем используйте операцию **операцию UpdateFolder** , чтобы отправить обновленный уровень **разрешений**, не включающий в себя **разрешение** для удаленного пользователя. 
  
Это также запрос XML, который отправляет управляемый API EWS при вызове метода **Update** для [удаления разрешений для папки](#bk_removeewsma).
  
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

Сервер отвечает на запрос **операцию UpdateFolder** с сообщением **упдатефолдерреспонсе** , которое содержит значение **ошибки**элемента [респонсекоде](https://msdn.microsoft.com/library/4b84d670-74c9-4d6d-84e7-f0a9f76f0d93%28Office.15%29.aspx) , которое указывает, что обновление прошло успешно.
  
## <a name="updating-folder-permissions-by-using-the-ews-managed-api"></a>Обновление разрешений для папки с помощью управляемого API EWS
<a name="bk_updateewsma"> </a>

Вы также можете обновить разрешения для папки для определенной папки с помощью управляемого API EWS. Чтобы обновить разрешения, выполните следующие действия. 
  
1. [Удалите разрешения для папки](#bk_removeewsma) с устаревшими разрешениями, но не вызывайте метод **обновления** (пока). 
    
2. [Добавление разрешений на доступ к папке для новых или измененных пользователей](#bk_enableewsma).
    
3. Вызовите метод **Update** , чтобы сохранить изменения. 
    
Если попытаться добавить два набора разрешений для одного и того же пользователя, появится сообщение об ошибке **сервицереспонсиксцептион** со следующим описанием: "указанный набор разрешений содержит дублирующиеся UserID". В этом случае удалите текущие разрешения из коллекции **разрешений** , а затем добавьте новые разрешения в коллекцию **разрешений** . 
  
## <a name="updating-folder-permissions-by-using-ews"></a>Обновление разрешений для папки с помощью EWS
<a name="bk_updateews"> </a>

Вы также можете обновить разрешения для папок для определенных папок с помощью EWS, объединив процесс удаления и добавления. Чтобы обновить разрешения, выполните следующие действия. 
  
1. Получение текущих разрешений папки с помощью операции "операция с **папкой** ". 
    
2. Отправьте обновленный список разрешений с помощью операции **операцию UpdateFolder** . 
    
Это те же две операции, которые используются для [включения](#bk_enableews) или [отключения доступа](#bk_removeews) с помощью EWS. Единственное отличие заключается в том, что при получении ответа на **папку** он будет содержать набор **разрешений** для пользователя. Просто замените существующий элемент **Permission** на новый элемент **Permission** , а затем отправьте операцию **операцию UpdateFolder** с новым значением или значениями **разрешений** . 
  
Если вы попытаетесь добавить два набора разрешений для одного и того же пользователя, вы получите значение **респонсекоде** для **еррордупликатеусеридсспеЦифиед**. В этом случае удалите устаревшее значение разрешения для пользователя из запроса и повторите запрос.

## <a name="next-steps"></a>Дальнейшие действия

После предоставления пользователю разрешения на доступ к определенной папке пользователь может получить доступ к папке в качестве делегата. Дополнительные сведения см. в указанных ниже статьях.
  
- [Доступ к электронной почте как представителю с помощью EWS в Exchange](how-to-access-email-as-a-delegate-by-using-ews-in-exchange.md)
    
- [Доступ к календарю как представителю с помощью EWS в Exchange](how-to-access-a-calendar-as-a-delegate-by-using-ews-in-exchange.md)
    
- [Доступ к контактам как представителю с помощью EWS в Exchange](how-to-access-contacts-as-a-delegate-by-using-ews-in-exchange.md)
    
## <a name="see-also"></a>См. также

- [Передача прав доступа и EWS в Exchange](delegate-access-and-ews-in-exchange.md)   
- [Добавление и удаление делегатов с помощью EWS в Exchange](how-to-add-and-remove-delegates-by-using-ews-in-exchange.md)    
- [Папки и элементы в веб-службах Exchange](folders-and-items-in-ews-in-exchange.md)
    

