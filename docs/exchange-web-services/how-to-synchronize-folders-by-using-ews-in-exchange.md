---
title: Синхронизация папок с помощью EWS в Exchange
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
localization_priority: Normal
ms.assetid: d3bbacd1-8e4b-4fd0-8d27-4cbbc045ec3f
description: Узнайте, как использовать управляемый API EWS или EWS для получения списка папок или списка папок, которые были изменены, чтобы синхронизировать клиент.
ms.openlocfilehash: 4b0686134d642da34b2890a0e692e3d03e4a9fb1
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/25/2018
ms.locfileid: "19761124"
---
# <a name="synchronize-folders-by-using-ews-in-exchange"></a>Синхронизация папок с помощью EWS в Exchange

Узнайте, как использовать управляемый API EWS или EWS для получения списка папок или списка папок, которые были изменены, чтобы синхронизировать клиент.
  
Служба EWS в Exchange использует синхронизацию элементов и синхронизацию папок для синхронизации содержимого почтовых ящиков между клиентом и сервером. Синхронизация папок получает исходный список папок из корневой папки, а затем получает изменения, внесенные в эти папки, а также создает новые папки.
  
Если вы выполняете синхронизацию папок с помощью управляемого API EWS, сначала необходимо [получить исходный список папок в корневой папке](how-to-synchronize-folders-by-using-ews-in-exchange.md#bk_cesyncinitialewsma) с помощью метода [ExchangeService. SyncFolderHierarchy](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.exchangeservice.syncfolderhierarchy%28v=exchg.80%29.aspx) . Затем необходимо обновить значение параметра _ксинкстате_ во время последующих вызовов, чтобы получить список новых и измененных папок. 
  
Чтобы выполнить синхронизацию папок с помощью EWS, запросите [исходный список папок в корневой папке](how-to-synchronize-folders-by-using-ews-in-exchange.md#bk_cesyncewsrequest) с помощью операции [SyncFolderHierarchy](http://msdn.microsoft.com/library/b31916b1-bc6c-4451-a475-b7c5417f752d%28Office.15%29.aspx) , выполните синтаксический анализ ответа, а затем в некоторый момент в будущем [получите изменения папок в корне](how-to-synchronize-folders-by-using-ews-in-exchange.md#bk_cesyncrespews)и проанализируйте ответ. После получения клиентом списка начальной или измененной папки он [выполняет локальное обновление](how-to-synchronize-folders-by-using-ews-in-exchange.md#bk_nextsteps). Как и когда вы извлечете изменения в будущем, зависит от [шаблона проекта синхронизации](mailbox-synchronization-and-ews-in-exchange.md#bk_syncpatterns) , используемого приложением. 
  
## <a name="get-the-list-of-all-folders-or-changed-folders-by-using-the-ews-managed-api"></a>Получение списка всех папок или измененных папок с помощью управляемого API EWS
<a name="bk_cesyncinitialewsma"> </a>

В приведенном ниже примере кода показано, как получить исходный список папок в корневой папке, а затем получить список изменений в папках корневой папки, произошедших с момента предыдущей синхронизации. Во время начального вызова метода [ExchangeService. SyncFolderHierarchy](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.exchangeservice.syncfolderhierarchy%28v=exchg.80%29.aspx) задайте для параметра _ксинкстате_ значение null. После выполнения метода сохраните значение _ксинкстате_ локально, чтобы использовать его в следующем вызове метода **SyncFolderHierarchy** . При первом вызове и последующих вызовах папки извлекаются в пакетах десяти, с помощью последовательных вызовов метода **SyncFolderHierarchy** , пока не будут сохранены другие изменения. В этом примере параметру _Property_ присваивается значение идонли для уменьшения числа вызовов к базе данных Exchange, что является [наилучшим вариантом синхронизации](mailbox-synchronization-and-ews-in-exchange.md#bk_bestpractices). В этом примере предполагается, что **Служба** является допустимой привязкой объекта **ExchangeService** и _ксинкстате_ представляет состояние синхронизации, возвращенное предыдущим вызовом в **SyncFolderHierarchy**. 
  
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

После получения списка новых или измененных папок на сервере [Создайте или обновите папки на клиенте](how-to-synchronize-folders-by-using-ews-in-exchange.md#bk_nextsteps).
  
## <a name="get-the-initial-list-of-folders-by-using-ews"></a>Получение исходного списка папок с помощью EWS
<a name="bk_cesyncewsrequest"> </a>

В следующем примере показан XML-запрос для получения исходной иерархии папок с помощью операции [SyncFolderHierarchy](http://msdn.microsoft.com/library/b31916b1-bc6c-4451-a475-b7c5417f752d%28Office.15%29.aspx) . Это также запрос XML, который управляемый API EWS отправляет при [получении списка исходных папок с помощью метода SyncFolderHierarchy](how-to-synchronize-folders-by-using-ews-in-exchange.md#bk_cesyncinitialewsma). Элемент [синкстате](http://msdn.microsoft.com/library/e5ebaae3-0f07-481d-ac67-d9687a3c7ac3%28Office.15%29.aspx) операции [SyncFolderHierarchy](http://msdn.microsoft.com/library/7f0de089-8876-47ec-a871-df118ceae75d%28Office.15%29.aspx) не включается, так как это начальная синхронизация. В этом примере для элемента [басешапе](http://msdn.microsoft.com/library/42c04f3b-abaa-4197-a3d6-d21677ffb1c0%28Office.15%29.aspx) задается значение **идонли** для уменьшения числа вызовов к базе данных Exchange, что является [наилучшим вариантом синхронизации](mailbox-synchronization-and-ews-in-exchange.md#bk_bestpractices).
  
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

В следующем примере показан ответ XML, возвращенный сервером после обработки запроса операции [SyncFolderHierarchy](http://msdn.microsoft.com/library/b31916b1-bc6c-4451-a475-b7c5417f752d%28Office.15%29.aspx) . Исходный ответ содержит элементы [CREATE](http://msdn.microsoft.com/library/6b463d0a-70e9-40c5-ade4-c7d9a5f36bc1%28Office.15%29.aspx) для всех папок, так как во время начальной синхронизации все папки считаются новыми. Значения некоторых атрибутов и элементов были сокращены для удобочитаемости, а некоторые блоки элементов **создания** были удалены для краткости. 
  
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

После получения списка новых папок на сервере [Создайте папки на клиенте](how-to-synchronize-folders-by-using-ews-in-exchange.md#bk_nextsteps).
  
## <a name="get-the-changes-since-the-last-sync-by-using-ews"></a>Получение изменений с момента последней синхронизации с помощью EWS
<a name="bk_cesyncrespews"> </a>

В следующем примере показан XML-запрос для получения списка изменений в папках корневой папки с помощью операции [SyncFolderHierarchy](http://msdn.microsoft.com/library/b31916b1-bc6c-4451-a475-b7c5417f752d%28Office.15%29.aspx) . Это также запрос XML, который отправляет управляемый API EWS при [получении списка изменений в корневой папке](how-to-synchronize-folders-by-using-ews-in-exchange.md#bk_cesyncinitialewsma). В этом примере для элемента [синкстате](http://msdn.microsoft.com/library/e5ebaae3-0f07-481d-ac67-d9687a3c7ac3%28Office.15%29.aspx) задается значение, возвращенное в предыдущем ответе. Для демонстрационных целей в этом примере для элемента [басешапе](http://msdn.microsoft.com/library/42c04f3b-abaa-4197-a3d6-d21677ffb1c0%28Office.15%29.aspx) задается значение **аллпропертиес** вместо **идонли** для отображения возвращаемых дополнительных свойств. Задание элемента [басешапе](http://msdn.microsoft.com/library/42c04f3b-abaa-4197-a3d6-d21677ffb1c0%28Office.15%29.aspx) равным **идонли** является [наилучшим методом синхронизации](mailbox-synchronization-and-ews-in-exchange.md#bk_bestpractices). Значение **синкстате** было сокращено для удобочитаемости. 
  
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

В следующем примере показан ответ XML, возвращенный сервером после обработки запроса [операции SyncFolderHierarchy](http://msdn.microsoft.com/library/b31916b1-bc6c-4451-a475-b7c5417f752d%28Office.15%29.aspx) от клиента. Этот ответ указывает на то, что одна папка была обновлена, была создана одна папка и удалена одна папка с момента предыдущей синхронизации. Значение элемента [синкстате](http://msdn.microsoft.com/library/e5ebaae3-0f07-481d-ac67-d9687a3c7ac3%28Office.15%29.aspx) , атрибуты **ID** и атрибуты **чанжекэй** были сокращены для удобочитаемости. 
  
Помните, что запрос включал в себя **аллпропертиес**[басешапе](http://msdn.microsoft.com/library/42c04f3b-abaa-4197-a3d6-d21677ffb1c0%28Office.15%29.aspx). Это только для демонстрационных целей. Рекомендуется присвоить элементу **басешапе** значение **идонли** в рабочей среде. 
  
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

Если вы используете управляемый API EWS, после получения списка новых или измененных папок используйте метод [Folder. Load](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.folder.load%28v=exchg.80%29.aspx) для получения свойств новых или измененных элементов, сравнения свойств с локальными значениями, а также для обновления или создания папок на клиенте. 
  
Если вы используете EWS, используйте операцию " [операция с папкой](http://msdn.microsoft.com/library/355bcf93-dc71-4493-b177-622afac5fdb9%28Office.15%29.aspx) " для получения свойств новых или измененных папок и обновления или создания папок на клиенте. 
  
## <a name="see-also"></a>См. также

- [Синхронизация почтового ящика и веб-службах Exchange](mailbox-synchronization-and-ews-in-exchange.md)   
- [Синхронизация элементов с помощью EWS в Exchange](how-to-synchronize-items-by-using-ews-in-exchange.md)   
- [Обработка ошибок, связанных с синхронизацией, в EWS в Exchange](handling-synchronization-related-errors-in-ews-in-exchange.md)
    

