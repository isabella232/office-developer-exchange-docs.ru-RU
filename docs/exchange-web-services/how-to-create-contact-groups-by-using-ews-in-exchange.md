---
title: Создание группы контактов с помощью веб-служб Exchange в Exchange
manager: sethgros
ms.date: 11/16/2014
ms.audience: Developer
localization_priority: Normal
ms.assetid: acec6e73-c016-419d-be1a-8ec5d993addb
description: Узнайте, как создать группу контактов с помощью управляемого интерфейса API веб-служб Exchange или веб-служб Exchange в Exchange.
ms.openlocfilehash: b3357f24e07a9c1b3b37ccb63b0f4f0d0a1d6fcf
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/25/2018
ms.locfileid: "19760992"
---
# <a name="create-contact-groups-by-using-ews-in-exchange"></a>Создание группы контактов с помощью веб-служб Exchange в Exchange

Узнайте, как создать группу контактов с помощью управляемого интерфейса API веб-служб Exchange или веб-служб Exchange в Exchange.
  
Можно создать группу контактов, являющийся частной [группы рассылки](distribution-groups-and-ews-in-exchange.md), с помощью управляемого интерфейса API веб-служб Exchange или веб-служб Exchange. Создание группы контактов, использовать методы в классе управляемый API EWS [ContactGroup](http://msdn.microsoft.com/en-us/library/office/microsoft.exchange.webservices.data.contactgroup%28v=exchg.80%29.aspx) или с помощью операции [CreateItem](http://msdn.microsoft.com/library/78a52120-f1d0-4ed7-8748-436e554f75b6%28Office.15%29.aspx) веб-служб Exchange. 
  
Обратите внимание на то, что нельзя использовать управляемый API EWS или веб-служб Exchange для создания универсальная группа рассылки или группу безопасности. Чтобы создать универсальная группа рассылки или группу безопасности, можно использовать [New-DistributionGroup](http://technet.microsoft.com/en-us/library/aa998856%28v=exchg.150%29.aspx)[командлет командной консоли Exchange](http://msdn.microsoft.com/en-us/library/ff326159%28v=exchg.140%29.aspx). 
  
## <a name="create-a-contact-group-by-using-the-ews-managed-api"></a>Создание группы контактов с помощью управляемого интерфейса API веб-служб Exchange
<a name="bk_EWSMA"> </a>

Чтобы создать группу контактов, достаточно несколько видов информации: имя группы и элементы для добавления в группу. Приведенный ниже показано, как создать простой группы контактов, содержащий несколько членов группы.
  
```cs
// Create a new contact group object.
ContactGroup myContactGroup = new ContactGroup(service);
// Give the group a name.
myContactGroup.DisplayName = "My Contact Group";
// Add some members to the group.
myContactGroup.Members.Add(new GroupMember("sadie@contoso.com"));
myContactGroup.Members.Add(new GroupMember("alfred@contoso.com"));
// Save the group.
myContactGroup.Save();

```

## <a name="create-a-contact-group-by-using-ews"></a>Создание группы контактов с помощью веб-служб Exchange
<a name="bk_EWSMA"> </a>

Выполнение может занять несколько дополнительные строки кода, но можно создать группу контактов с помощью операции [CreateItem](http://msdn.microsoft.com/library/78a52120-f1d0-4ed7-8748-436e554f75b6%28Office.15%29.aspx) веб-служб Exchange. В следующем примере запрос XML показано, как создать группу контактов. Это также запроса XML, который отправляется, когда [использовать управляемый API веб-служб Exchange для создания группы контактов](#bk_EWSMA).
  
```XML
<?xml version="1.0" encoding="utf-8"?>
   <CreateItem xmlns="http://schemas.microsoft.com/exchange/services/2006/messages" 
MessageDisposition="SaveOnly">
      <Items xmlns:m="http://schemas.microsoft.com/exchange/services/2006/messages">
         <DistributionList xmlns="http://schemas.microsoft.com/exchange/services/2006/types">
            <DisplayName xmlns="http://schemas.microsoft.com/exchange/services/2006/types">
               My Contact Group
            </DisplayName>
            <Members xmlns="http://schemas.microsoft.com/exchange/services/2006/types">
               <Member xmlns="http://schemas.microsoft.com/exchange/services/2006/types">
                  <Mailbox xmlns="http://schemas.microsoft.com/exchange/services/2006/types">
                     <EmailAddress xmlns="http://schemas.microsoft.com/exchange/services/2006/types">
                        sadie@contoso.com
                     </EmailAddress>
                  </Mailbox>
               </Member>
               <Member xmlns="http://schemas.microsoft.com/exchange/services/2006/types">
                  <Mailbox xmlns="http://schemas.microsoft.com/exchange/services/2006/types">
                     <EmailAddress xmlns="http://schemas.microsoft.com/exchange/services/2006/types">
                        alfred@contoso.com
                     </EmailAddress>
                  </Mailbox>
               </Member>
            </Members>
         </DistributionList>
      </Items>
   </CreateItem>
```

Ниже приведен пример успешного ответа XML для запроса. Обратите внимание, что возвращаемые значения включают идентификатор элемента для новой группы контактов и изменить ключ, можно использовать в другой код для изменения группы контактов или разверните группу, чтобы просмотреть список членов. Идентификатор элемента сокращение для удобства чтения.
  
```XML
<?xml version="1.0" encoding="utf-8"?>
   <CreateItemResponse xmlns="http://schemas.microsoft.com/exchange/services/2006/messages">
      <ResponseMessages xmlns="http://schemas.microsoft.com/exchange/services/2006/messages">
         <CreateItemResponseMessage ResponseClass="Success" 
             xmlns="http://schemas.microsoft.com/exchange/services/2006/messages">
            <ResponseCode xmlns="http://schemas.microsoft.com/exchange/services/2006/messages">
               NoError
            </ResponseCode>
            <Items xmlns="http://schemas.microsoft.com/exchange/services/2006/messages">
               <DistributionList xmlns="http://schemas.microsoft.com/exchange/services/2006/types">
                  <ItemId xmlns="http://schemas.microsoft.com/exchange/services/2006/types" 
                          Id="AAMkADBlY…" 
                          ChangeKey="EgAAABYAAAAD7hO1SJPWTbICFWZ4U3NMAABXzQiK" />
               </DistributionList>
            </Items>
         </CreateItemResponseMessage>
      </ResponseMessages>
   </CreateItemResponse>
```

## <a name="see-also"></a>См. также


- [Группы рассылки и EWS в Exchange](distribution-groups-and-ews-in-exchange.md)
    
- [Разверните узел группы рассылки с помощью веб-служб Exchange в Exchange 2013](how-to-expand-distribution-groups-by-using-ews-in-exchange-2013.md)
    

