---
title: Синхронизация папок с помощью EWS в Exchange
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.localizationpriority: medium
ms.assetid: d3bbacd1-8e4b-4fd0-8d27-4cbbc045ec3f
description: Узнайте, как использовать управляемый API или EWS EWS для получения списка папок или списка измененных папок, чтобы синхронизировать клиента.
ms.openlocfilehash: f22cb3b4ba92da9c044e08e7164d116293cf43ff
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/24/2021
ms.locfileid: "59521094"
---
# <a name="synchronize-folders-by-using-ews-in-exchange"></a>Синхронизация папок с помощью EWS в Exchange

Узнайте, как использовать управляемый API или EWS EWS для получения списка папок или списка измененных папок, чтобы синхронизировать клиента.
  
EWS Exchange синхронизации элементов и синхронизации папок для синхронизации контента почтовых ящиков между клиентом и сервером. Синхронизация папок получает начальный список папок из корневой папки, а затем со временем получает изменения, внесенные в эти папки, и получает новые папки.
  
Если выполняется синхронизация папок с помощью управляемого API EWS, сначала вы получите начальный список папок в корневой папке с помощью метода [ExchangeService.SyncFolderHierarchy.](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.exchangeservice.syncfolderhierarchy%28v=exchg.80%29.aspx) [](how-to-synchronize-folders-by-using-ews-in-exchange.md#bk_cesyncinitialewsma) Затем во время последующих вызовов обновляется значение параметра  _cSyncState,_ чтобы получить список новых и измененных папок. 
  
Чтобы выполнить синхронизацию папок с помощью EWS, вы запросите начальный список папок в корневой папке с помощью операции [SyncFolderHierarchy,](https://msdn.microsoft.com/library/b31916b1-bc6c-4451-a475-b7c5417f752d%28Office.15%29.aspx) разберите ответ, а затем в будущем получите изменения в папках в корне [и](how-to-synchronize-folders-by-using-ews-in-exchange.md#bk_cesyncrespews)разберите ответ. [](how-to-synchronize-folders-by-using-ews-in-exchange.md#bk_cesyncewsrequest) После получения клиентом списка начальных или измененных папок он делает обновления [локально.](how-to-synchronize-folders-by-using-ews-in-exchange.md#bk_nextsteps) Как и когда вы извлекаете изменения в будущем, зависит от шаблона проектирования [синхронизации,](mailbox-synchronization-and-ews-in-exchange.md#bk_syncpatterns) используемой вашим приложением. 
  
## <a name="get-the-list-of-all-folders-or-changed-folders-by-using-the-ews-managed-api"></a>Получите список всех папок или измененных папок с помощью управляемого API EWS
<a name="bk_cesyncinitialewsma"> </a>

В следующем примере кода показано, как получить начальный список папок в корневой папке, а затем получить список изменений папок в корневой папке, которые произошли после предыдущей синхронизации. Во время начального вызова метода [ExchangeService.SyncFolderHierarchy](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.exchangeservice.syncfolderhierarchy%28v=exchg.80%29.aspx) установите значение  _cSyncState_ на нуль. После завершения метода сохраните локальное значение _cSyncState_ для использования в следующем вызове **метода SyncFolderHierarchy.** В начальных и последующих вызовах папки извлекаются пакетами из десяти, используя последовательные вызовы к методу **SyncFolderHierarchy,** пока больше не будут внесены изменения. В этом примере параметр _propertySet_ задает IdOnly для уменьшения вызовов в базу данных Exchange, что является наилучшей практикой [синхронизации.](mailbox-synchronization-and-ews-in-exchange.md#bk_bestpractices) В этом примере  мы предполагаем, что служба является допустимой привязкой объекта **ExchangeService** и _что cSyncState_ представляет состояние синхронизации, которое было возвращено по предварительному вызову **в SyncFolderHierarchy**. 
  
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

После получения списка новых или измененных папок на сервере создайте или обновим [папки на клиенте.](how-to-synchronize-folders-by-using-ews-in-exchange.md#bk_nextsteps)
  
## <a name="get-the-initial-list-of-folders-by-using-ews"></a>Получите начальный список папок с помощью EWS
<a name="bk_cesyncewsrequest"> </a>

В следующем примере показан XML-запрос для получения начальной иерархии папок с помощью операции [SyncFolderHierarchy.](https://msdn.microsoft.com/library/b31916b1-bc6c-4451-a475-b7c5417f752d%28Office.15%29.aspx) Это также XML-запрос, который отправляет управляемый API EWS при ирисовке списка начальных папок с помощью метода [SyncFolderHierarchy.](how-to-synchronize-folders-by-using-ews-in-exchange.md#bk_cesyncinitialewsma) Элемент [SyncState](https://msdn.microsoft.com/library/e5ebaae3-0f07-481d-ac67-d9687a3c7ac3%28Office.15%29.aspx) операции [SyncFolderHierarchy](https://msdn.microsoft.com/library/7f0de089-8876-47ec-a871-df118ceae75d%28Office.15%29.aspx) не включен, так как это первоначальная синхронизация. В этом примере элемент [BaseShape](https://msdn.microsoft.com/library/42c04f3b-abaa-4197-a3d6-d21677ffb1c0%28Office.15%29.aspx) устанавливается **в IdOnly** для уменьшения вызовов в базу данных Exchange, что является наилучшей практикой [синхронизации.](mailbox-synchronization-and-ews-in-exchange.md#bk_bestpractices)
  
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

В следующем примере показан XML-ответ, который возвращается сервером после обработки запроса на операцию [SyncFolderHierarchy.](https://msdn.microsoft.com/library/b31916b1-bc6c-4451-a475-b7c5417f752d%28Office.15%29.aspx) Первоначальный ответ включает [создание](https://msdn.microsoft.com/library/6b463d0a-70e9-40c5-ade4-c7d9a5f36bc1%28Office.15%29.aspx) элементов для всех папок, так как все папки считаются новыми во время начальной синхронизации. Значения некоторых атрибутов и элементов были сокращены для читаемости, а некоторые блоки **элементов Create** были удалены для краткости. 
  
```xml
<?xml version="1.0" encoding="utf-8"?>
<s:Envelope xmlns:s="https://schemas.xmlsoap.org/soap/envelope/">
  <s:Header>
    <h:ServerVersionInfo MajorVersion="15"
                         MinorVersion="0"
                         MajorBuildNumber="785"
                         MinorBuildNumber="6"
                         Version="V2_6"
                         xmlns:h="https://schemas.microsoft.com/exchange/services/2006/types"
                         xmlns="https://schemas.microsoft.com/exchange/services/2006/types"
                         xmlns:xsd="http://www.w3.org/2001/XMLSchema"
                         xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance"/>
  </s:Header>
  <s:Body xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance"
          xmlns:xsd="http://www.w3.org/2001/XMLSchema">
    <m:SyncFolderHierarchyResponse xmlns:m="https://schemas.microsoft.com/exchange/services/2006/messages"
                                   xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types">
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

После получения списка новых папок на сервере создайте папки [на клиенте.](how-to-synchronize-folders-by-using-ews-in-exchange.md#bk_nextsteps)
  
## <a name="get-the-changes-since-the-last-sync-by-using-ews"></a>Получить изменения после последней синхронизации с помощью EWS
<a name="bk_cesyncrespews"> </a>

В следующем примере показан XML-запрос для получения списка изменений папок в корневой папке с помощью операции [SyncFolderHierarchy.](https://msdn.microsoft.com/library/b31916b1-bc6c-4451-a475-b7c5417f752d%28Office.15%29.aspx) Это также XML-запрос, который отправляет управляемый API EWS при ирисовке списка изменений в [корневой папке.](how-to-synchronize-folders-by-using-ews-in-exchange.md#bk_cesyncinitialewsma) В этом примере значение [элемента SyncState](https://msdn.microsoft.com/library/e5ebaae3-0f07-481d-ac67-d9687a3c7ac3%28Office.15%29.aspx) определяется значением, возвращенным в предыдущем ответе. В этом примере в демонстрационных целях элемент  BaseShape вместо **IdOnly** задает элемент [BaseShape](https://msdn.microsoft.com/library/42c04f3b-abaa-4197-a3d6-d21677ffb1c0%28Office.15%29.aspx) для показа возвращенных дополнительных свойств. Настройка элемента [BaseShape](https://msdn.microsoft.com/library/42c04f3b-abaa-4197-a3d6-d21677ffb1c0%28Office.15%29.aspx) **для IdOnly** — это передовая [практика синхронизации.](mailbox-synchronization-and-ews-in-exchange.md#bk_bestpractices) Значение **SyncState** было сокращено для читаемости. 
  
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

В следующем примере показан XML-ответ, который возвращается сервером после обработки запроса на операцию [SyncFolderHierarchy](https://msdn.microsoft.com/library/b31916b1-bc6c-4451-a475-b7c5417f752d%28Office.15%29.aspx) от клиента. В этом ответе указывается, что одна папка была обновлена, одна была создана, а одна папка была удалена с момента предыдущей синхронизации. Значение элемента [SyncState,](https://msdn.microsoft.com/library/e5ebaae3-0f07-481d-ac67-d9687a3c7ac3%28Office.15%29.aspx) **атрибутов Id** и **атрибутов ChangeKey** было сокращено для чтения. 
  
Помните, что запрос включал **базу AllProperties.**[](https://msdn.microsoft.com/library/42c04f3b-abaa-4197-a3d6-d21677ffb1c0%28Office.15%29.aspx) Это только для демонстрационных целей. Рекомендуется настроить элемент **BaseShape** на **IdOnly** в производстве. 
  
```XML
<?xml version="1.0" encoding="utf-8"?>
<s:Envelope xmlns:s="https://schemas.xmlsoap.org/soap/envelope/">
  <s:Header>
<h:ServerVersionInfo MajorVersion="15" MinorVersion="0" MajorBuildNumber="745" MinorBuildNumber="21" Version="V2_3" 
           xmlns:h="https://schemas.microsoft.com/exchange/services/2006/types" 
           xmlns="https://schemas.microsoft.com/exchange/services/2006/types" 
           xmlns:xsd="http://www.w3.org/2001/XMLSchema" 
           xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" />
  </s:Header>
  <s:Body xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" xmlns:xsd="http://www.w3.org/2001/XMLSchema">
    <m:SyncFolderHierarchyResponse xmlns:m="https://schemas.microsoft.com/exchange/services/2006/messages" 
            xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types">
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

Если вы используете управляемый API EWS, после получения списка новых или измененных папок используйте метод [Folder.Load,](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.folder.load%28v=exchg.80%29.aspx) чтобы получить свойства для новых или измененных элементов, сравнить свойства с локальными значениями и обновить или создать папки на клиенте. 
  
Если вы используете EWS, используйте операцию [GetFolder](https://msdn.microsoft.com/library/355bcf93-dc71-4493-b177-622afac5fdb9%28Office.15%29.aspx) для получения свойств в новых или измененных папках и обновления или создания папок на клиенте. 
  
## <a name="see-also"></a>См. также

- [Синхронизация почтового ящика и веб-службах Exchange](mailbox-synchronization-and-ews-in-exchange.md)   
- [Синхронизация элементов с помощью EWS в Exchange](how-to-synchronize-items-by-using-ews-in-exchange.md)   
- [Обработка ошибок, связанных с синхронизацией в EWS в Exchange](handling-synchronization-related-errors-in-ews-in-exchange.md)
    

