---
title: Синхронизация папок с помощью веб-служб Exchange в Exchange
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
localization_priority: Normal
ms.assetid: d3bbacd1-8e4b-4fd0-8d27-4cbbc045ec3f
description: Узнайте, как использовать управляемый API EWS или веб-служб Exchange, чтобы получить список папок или список папок, которые были изменены, чтобы синхронизировать вашего клиента.
ms.openlocfilehash: 4b0686134d642da34b2890a0e692e3d03e4a9fb1
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/11/2018
ms.locfileid: "19761124"
---
# <a name="synchronize-folders-by-using-ews-in-exchange"></a>Синхронизация папок с помощью веб-служб Exchange в Exchange

Узнайте, как использовать управляемый API EWS или веб-служб Exchange, чтобы получить список папок или список папок, которые были изменены, чтобы синхронизировать вашего клиента.
  
ВЕБ-службах Exchange с помощью синхронизации элемента и синхронизации папок для содержимого почтового ящика синхронизации между клиентом и сервером. Синхронизации папки Получает исходный список папок из корневой папки и затем постепенно, получает изменения, внесенные в эти папки и возвращает также новые папки.
  
При выполнении синхронизации папок с помощью управляемого API EWS, вы первый [получить исходный список папок, расположенных в корневую папку](how-to-synchronize-folders-by-using-ews-in-exchange.md#bk_cesyncinitialewsma) с помощью метода [ExchangeService.SyncFolderHierarchy](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.exchangeservice.syncfolderhierarchy%28v=exchg.80%29.aspx) . Затем обновите значение параметра _cSyncState_ во время последующих вызовов, чтобы получить список папок, новые и измененные. 
  
Для выполнения синхронизации папки с помощью веб-служб Exchange, запрос [исходный список папок, расположенных в корневую папку](how-to-synchronize-folders-by-using-ews-in-exchange.md#bk_cesyncewsrequest) с помощью операции [SyncFolderHierarchy](http://msdn.microsoft.com/library/b31916b1-bc6c-4451-a475-b7c5417f752d%28Office.15%29.aspx) , проанализировать ответ и к определенному моменту в будущем [внесения изменений в папки в корневой](how-to-synchronize-folders-by-using-ews-in-exchange.md#bk_cesyncrespews)и разбор ответа. После получения список папок, начальной или измененные, оно [делает обновления локально](how-to-synchronize-folders-by-using-ews-in-exchange.md#bk_nextsteps). Как и когда в будущем извлечения изменений, зависит от [шаблона разработки синхронизации](mailbox-synchronization-and-ews-in-exchange.md#bk_syncpatterns) с помощью приложения. 
  
## <a name="get-the-list-of-all-folders-or-changed-folders-by-using-the-ews-managed-api"></a>Получение списка всех папок и папок, измененные с помощью управляемого интерфейса API веб-служб Exchange
<a name="bk_cesyncinitialewsma"> </a>

В следующем примере кода показано, как получить исходный список папок, расположенных в корневую папку и затем получите список изменений в папки в корневой папке, произошедшие с момента предыдущей синхронизации. Во время первого вызова метода [ExchangeService.SyncFolderHierarchy](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.exchangeservice.syncfolderhierarchy%28v=exchg.80%29.aspx) задайте значение _cSyncState_ значения NULL. После завершения работы метода, сохраните значение _cSyncState_ локально для использования в следующем вызове метода **SyncFolderHierarchy** . В первого вызова и последующих вызовов папок извлекаются в пакетах десять, с помощью успешные вызовы метода **SyncFolderHierarchy** , пока остаются больше нет изменений. В этом примере задается параметр _propertySet_ IdOnly для уменьшения обращений к базе данных Exchange, который является [Рекомендация синхронизации](mailbox-synchronization-and-ews-in-exchange.md#bk_bestpractices). В этом примере предполагается, что **Служба** — допустимый объект привязки **ExchangeService** и _cSyncState_ , представляющий состояние синхронизации, возвращаемые предыдущего вызова **SyncFolderHierarchy**. 
  
```cs
// Get a list of all folders in the mailbox by calling SyncFolderHierarchy.
// The folderId parameter must be set to the root folder to synchronize. 
// The propertySet parameter is set to IdOnly to reduce calls to the Exchange database
// because any additional properties result in additional calls to the Exchange database. 
// The syncState parameter is set to cSyncState, which should be null in the initial call, 
// and should be set to the sync state returned by the previous SyncFolderHierarchy call 
// in subsequent calls.
ChangeCollection<FolderChange> fcc = service.SyncFolderHierarchy(new FolderId(WellKnownFolderName.Root), PropertySet.IdOnly, cSyncState);
// If the count of changes is zero, there are no changes to synchronize.
if (fcc.Count == 0)
{
    Console.WriteLine("There are no folders to synchronize.");
}
// Otherwise, write all the changes included in the response 
// to the console. 
// For the initial synchronization, all the changes will be of type
// ChangeType.Create.
else
{
    foreach (FolderChange fc in fcc)
    {
        Console.WriteLine("ChangeType: " + fc.ChangeType.ToString());
        Console.WriteLine("FolderId: " + fc.FolderId);
        Console.WriteLine("===========");
    }
}
// Save the sync state for use in future SyncFolderItems requests.
// The sync state is used by the server to determine what changes to report
// to the client.
string fSyncState = fcc.SyncState;

```

После можно получить список новые или измененные папок на сервере, [Создайте или обновите папок на стороне клиента](how-to-synchronize-folders-by-using-ews-in-exchange.md#bk_nextsteps).
  
## <a name="get-the-initial-list-of-folders-by-using-ews"></a>Получение исходный список папок с помощью веб-служб Exchange
<a name="bk_cesyncewsrequest"> </a>

В следующем примере показано XML-запрос для получения иерархии начальной папки с помощью операции [SyncFolderHierarchy](http://msdn.microsoft.com/library/b31916b1-bc6c-4451-a475-b7c5417f752d%28Office.15%29.aspx) . Это также запроса XML, что управляемый API EWS отправляет при [получении списка начальной папки с помощью метода SyncFolderHierarchy](how-to-synchronize-folders-by-using-ews-in-exchange.md#bk_cesyncinitialewsma). Элемент [состояние](http://msdn.microsoft.com/library/e5ebaae3-0f07-481d-ac67-d9687a3c7ac3%28Office.15%29.aspx) операции [SyncFolderHierarchy](http://msdn.microsoft.com/library/7f0de089-8876-47ec-a871-df118ceae75d%28Office.15%29.aspx) не включена, так как это начальная синхронизация. В этом примере задается элемент [BaseShape](http://msdn.microsoft.com/library/42c04f3b-abaa-4197-a3d6-d21677ffb1c0%28Office.15%29.aspx) **IdOnly** для уменьшения обращений к базе данных Exchange, который является [Рекомендация синхронизации](mailbox-synchronization-and-ews-in-exchange.md#bk_bestpractices).
  
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
    <m:SyncFolderHierarchy>
      <m:FolderShape>
        <t:BaseShape>IdOnly</t:BaseShape>
      </m:FolderShape>
      <m:SyncFolderId>
        <t:DistinguishedFolderId Id="root" />
      </m:SyncFolderId>
    </m:SyncFolderHierarchy>
  </soap:Body>
</soap:Envelope>
```

В следующем примере показано XML-ответ, возвращенный сервером, после обработки запроса операции [SyncFolderHierarchy](http://msdn.microsoft.com/library/b31916b1-bc6c-4451-a475-b7c5417f752d%28Office.15%29.aspx) . Первоначального отклика включает [Создать](http://msdn.microsoft.com/library/6b463d0a-70e9-40c5-ade4-c7d9a5f36bc1%28Office.15%29.aspx) элементы для всех папок, так как все папках считаются new во время начальной синхронизации. Значения некоторые атрибуты и элементы URL были сокращены для удобства чтения и некоторые блоки **Создать** элемент были удалены для краткости. 
  
```xml
<?xml version="1.0" encoding="utf-8"?>
<s:Envelope xmlns:s="http://schemas.xmlsoap.org/soap/envelope/">
  <s:Header>
    <h:ServerVersionInfo MajorVersion="15"
                         MinorVersion="0"
                         MajorBuildNumber="785"
                         MinorBuildNumber="6"
                         Version="V2_6"
                         xmlns:h="http://schemas.microsoft.com/exchange/services/2006/types"
                         xmlns="http://schemas.microsoft.com/exchange/services/2006/types"
                         xmlns:xsd="http://www.w3.org/2001/XMLSchema"
                         xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance"/>
  </s:Header>
  <s:Body xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance"
          xmlns:xsd="http://www.w3.org/2001/XMLSchema">
    <m:SyncFolderHierarchyResponse xmlns:m="http://schemas.microsoft.com/exchange/services/2006/messages"
                                   xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types">
      <m:ResponseMessages>
        <m:SyncFolderHierarchyResponseMessage ResponseClass="Success">
          <m:ResponseCode>NoError</m:ResponseCode>
          <m:SyncState>H4sIAA==</m:SyncState>
          <m:IncludesLastFolderInRange>true</m:IncludesLastFolderInRange>
          <m:Changes>
            <t:Create>
              <t:Folder>
                <t:FolderId Id="AAMkADM="
                            ChangeKey="AQAAABYA"/>
              </t:Folder>
            </t:Create>
            <t:Create>
              <t:Folder>
                <t:FolderId Id="AAMkADMzM="
                            ChangeKey="AQAAABY"/>
              </t:Folder>
            </t:Create>
            <t:Create>
              <t:Folder>
                <t:FolderId Id="AAMkAD/AAA="
                            ChangeKey="AQAAABYA"/>
              </t:Folder>
            </t:Create>
            <t:Create>
              <t:Folder>
                <t:FolderId Id="AAMkADBh="
                            ChangeKey="AQAAABYA"/>
              </t:Folder>
            </t:Create>
            ...
          </m:Changes>
        </m:SyncFolderHierarchyResponseMessage>
      </m:ResponseMessages>
    </m:SyncFolderHierarchyResponse>
  </s:Body>
</s:Envelope>
```

После можно извлечь список новые папки на сервере, [Создайте папки на стороне клиента](how-to-synchronize-folders-by-using-ews-in-exchange.md#bk_nextsteps).
  
## <a name="get-the-changes-since-the-last-sync-by-using-ews"></a>Получение изменений с момента последней синхронизации с помощью веб-служб Exchange
<a name="bk_cesyncrespews"> </a>

В следующем примере показано запроса XML для получения списка изменения папки в корневую папку с помощью операции [SyncFolderHierarchy](http://msdn.microsoft.com/library/b31916b1-bc6c-4451-a475-b7c5417f752d%28Office.15%29.aspx) . Это также запроса XML, что управляемый API EWS отправляет при [получении списка изменений в корневую папку](how-to-synchronize-folders-by-using-ews-in-exchange.md#bk_cesyncinitialewsma). В этом примере задается значение элемента [состояние](http://msdn.microsoft.com/library/e5ebaae3-0f07-481d-ac67-d9687a3c7ac3%28Office.15%29.aspx) значению, возвращенному в предыдущем ответе. И в целях демонстрации в этом примере задается элемент [BaseShape](http://msdn.microsoft.com/library/42c04f3b-abaa-4197-a3d6-d21677ffb1c0%28Office.15%29.aspx) **AllProperties** вместо **IdOnly** для отображения возвращаемые дополнительные свойства. Установка для элемента [BaseShape](http://msdn.microsoft.com/library/42c04f3b-abaa-4197-a3d6-d21677ffb1c0%28Office.15%29.aspx) **IdOnly** является [Рекомендация синхронизации](mailbox-synchronization-and-ews-in-exchange.md#bk_bestpractices). Для удобства чтения был усечен значение **состояние** . 
  
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
    <m:SyncFolderHierarchy>
      <m:FolderShape>
        <t:BaseShape>AllProperties</t:BaseShape>
      </m:FolderShape>
      <m:SyncFolderId>
        <t:DistinguishedFolderId Id="root" />
      </m:SyncFolderId>
      <m:SyncState>H4sIAA==</m:SyncState>
    </m:SyncFolderHierarchy>
  </soap:Body>
</soap:Envelope>
```

В следующем примере показано XML-ответ, возвращенный сервером, после обработки запроса [операции SyncFolderHierarchy](http://msdn.microsoft.com/library/b31916b1-bc6c-4451-a475-b7c5417f752d%28Office.15%29.aspx) от клиента. Этот ответ указывает, что были добавлены в одной папке, один папка была создана и один папка была удалена с момента предыдущей синхронизации. Значение элемента [состояние](http://msdn.microsoft.com/library/e5ebaae3-0f07-481d-ac67-d9687a3c7ac3%28Office.15%29.aspx) , **идентификатор** атрибуты и атрибуты **ChangeKey** URL-были сокращены для удобства чтения. 
  
Имейте в виду, что запрос включены **AllProperties**[BaseShape](http://msdn.microsoft.com/library/42c04f3b-abaa-4197-a3d6-d21677ffb1c0%28Office.15%29.aspx). Это только в целях демонстрации. Рекомендуется устанавливать элемент **BaseShape** в **IdOnly** в рабочей среде. 
  
```XML
<?xml version="1.0" encoding="utf-8"?>
<s:Envelope xmlns:s="http://schemas.xmlsoap.org/soap/envelope/">
  <s:Header>
<h:ServerVersionInfo MajorVersion="15" MinorVersion="0" MajorBuildNumber="745" MinorBuildNumber="21" Version="V2_3" 
           xmlns:h="http://schemas.microsoft.com/exchange/services/2006/types" 
           xmlns="http://schemas.microsoft.com/exchange/services/2006/types" 
           xmlns:xsd="http://www.w3.org/2001/XMLSchema" 
           xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" />
  </s:Header>
  <s:Body xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" xmlns:xsd="http://www.w3.org/2001/XMLSchema">
    <m:SyncFolderHierarchyResponse xmlns:m="http://schemas.microsoft.com/exchange/services/2006/messages" 
            xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types">
      <m:ResponseMessages>
        <m:SyncFolderHierarchyResponseMessage ResponseClass="Success">
          <m:ResponseCode>NoError</m:ResponseCode>
          <m:SyncState>H4sIAAA</m:SyncState>
          <m:IncludesLastFolderInRange>true</m:IncludesLastFolderInRange>
          <m:Changes>
            <t:Update>
              <t:Folder>
                <t:FolderId Id="AAMkADM=" ChangeKey="AQAAABY" />
                <t:ParentFolderId Id="AQMkADMzADI1==" ChangeKey="AQAAAA==" />
                <t:FolderClass>IPF.Note</t:FolderClass>
                <t:DisplayName>Meeting Notes</t:DisplayName>
                <t:TotalCount>3</t:TotalCount>
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
              </t:Folder>
            </t:Update>
            <t:Create>
              <t:Folder>
                <t:FolderId Id="AAMkADMzM=" ChangeKey="AQAAABYAA" />
                <t:ParentFolderId Id="AQMkO67A==" ChangeKey="AQAAAA==" />
                <t:FolderClass>IPF.Note</t:FolderClass>
                <t:DisplayName>Schedules</t:DisplayName>
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
                <t:UnreadCount>0</t:UnreadCount>
              </t:Folder>
            </t:Create>
            <t:Delete>
              <t:FolderId Id="AAMkAD/AAA=" ChangeKey="AQAAAA==" />
            </t:Delete>
          </m:Changes>
        </m:SyncFolderHierarchyResponseMessage>
      </m:ResponseMessages>
    </m:SyncFolderHierarchyResponse>
  </s:Body>
</s:Envelope>

```

## <a name="update-the-client"></a>Обновление клиента
<a name="bk_nextsteps"> </a>

Если вы используете управляемый API веб-служб Exchange, после получить список папок, новые или измененные, используйте метод [Folder.Load](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.folder.load%28v=exchg.80%29.aspx) на получение свойств для новых и измененных элементов, сравните свойства в локальном значения и обновление или создание папок на стороне клиента. 
  
Если вы используете веб-служб Exchange, с помощью [операции GetFolder](http://msdn.microsoft.com/library/355bcf93-dc71-4493-b177-622afac5fdb9%28Office.15%29.aspx) для получения свойств папки новые или измененные и обновления или создания папки на стороне клиента. 
  
## <a name="see-also"></a>См. также

- [Синхронизация почтового ящика и веб-службах Exchange](mailbox-synchronization-and-ews-in-exchange.md)   
- [Синхронизация элементов с помощью веб-служб Exchange в Exchange](how-to-synchronize-items-by-using-ews-in-exchange.md)   
- [Обработка ошибок, связанных с синхронизации в веб-служб Exchange в Exchange](handling-synchronization-related-errors-in-ews-in-exchange.md)
    

