---
title: 'Как: создать группы контактов с помощью EWS в Exchange'
manager: sethgros
ms.date: 11/16/2014
ms.audience: Developer
localization_priority: Normal
ms.assetid: acec6e73-c016-419d-be1a-8ec5d993addb
description: Узнайте, как создать группу контактов с помощью управляемого API EWS или EWS в Exchange.
ms.openlocfilehash: 1da876bbda72f5bea08fd9855aa3f554135d54aa
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/03/2020
ms.locfileid: "44528141"
---
# <a name="create-contact-groups-by-using-ews-in-exchange"></a>Как: создать группы контактов с помощью EWS в Exchange

Узнайте, как создать группу контактов с помощью управляемого API EWS или EWS в Exchange.
  
Вы можете создать группу контактов, которая представляет собой частную [группу рассылки](distribution-groups-and-ews-in-exchange.md), с помощью управляемого API EWS или EWS. Для создания групп контактов используйте методы в классе управляемого API [ContactGroup](https://msdn.microsoft.com/library/office/microsoft.exchange.webservices.data.contactgroup%28v=exchg.80%29.aspx) EWS или используйте операцию [CreateItem](https://msdn.microsoft.com/library/78a52120-f1d0-4ed7-8748-436e554f75b6%28Office.15%29.aspx) EWS. 
  
Обратите внимание, что вы не можете создать универсальную группу рассылки или группу безопасности с помощью управляемого API EWS или EWS. Чтобы создать универсальную группу рассылки или группу безопасности, можно использовать командлет [New – DistributionGroup](https://technet.microsoft.com/library/aa998856%28v=exchg.150%29.aspx)[Exchange Management Shell](https://msdn.microsoft.com/library/ff326159%28v=exchg.140%29.aspx). 
  
## <a name="create-a-contact-group-by-using-the-ews-managed-api"></a>Создание группы контактов с помощью управляемого API EWS
<a name="bk_EWSMA"> </a>

Для создания группы контактов необходимо всего несколько сведений: имя группы и членов, добавляемых в группу. В приведенном ниже примере показано, как создать простую группу контактов, содержащую пару участников группы.
  
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

## <a name="create-a-contact-group-by-using-ews"></a>Создание группы контактов с помощью EWS
<a name="bk_EWSMA"> </a>

Может потребоваться еще несколько строк кода, но вы можете создать группу контактов с помощью операции [CreateItem](https://msdn.microsoft.com/library/78a52120-f1d0-4ed7-8748-436e554f75b6%28Office.15%29.aspx) EWS. В приведенном ниже примере XML-запроса показано, как можно создать группу контактов. Это также XML-запрос, который отправляется при [использовании управляемого API EWS для создания группы контактов](#bk_EWSMA).
  
```XML
<?xml version="1.0" encoding="utf-8"?>
   <CreateItem xmlns="https://schemas.microsoft.com/exchange/services/2006/messages" 
MessageDisposition="SaveOnly">
      <Items xmlns:m="https://schemas.microsoft.com/exchange/services/2006/messages">
         <DistributionList xmlns="https://schemas.microsoft.com/exchange/services/2006/types">
            <DisplayName xmlns="https://schemas.microsoft.com/exchange/services/2006/types">
               My Contact Group
            </DisplayName>
            <Members xmlns="https://schemas.microsoft.com/exchange/services/2006/types">
               <Member xmlns="https://schemas.microsoft.com/exchange/services/2006/types">
                  <Mailbox xmlns="https://schemas.microsoft.com/exchange/services/2006/types">
                     <EmailAddress xmlns="https://schemas.microsoft.com/exchange/services/2006/types">
                        sadie@contoso.com
                     </EmailAddress>
                  </Mailbox>
               </Member>
               <Member xmlns="https://schemas.microsoft.com/exchange/services/2006/types">
                  <Mailbox xmlns="https://schemas.microsoft.com/exchange/services/2006/types">
                     <EmailAddress xmlns="https://schemas.microsoft.com/exchange/services/2006/types">
                        alfred@contoso.com
                     </EmailAddress>
                  </Mailbox>
               </Member>
            </Members>
         </DistributionList>
      </Items>
   </CreateItem>
```

Ниже приведен пример успешного XML-ответа на запрос. Обратите внимание, что возвращаемые значения включают идентификатор элемента для новой группы контактов и ключ изменения, который можно использовать в другом коде для изменения группы контактов или для развертывания группы, чтобы увидеть ее участников. Идентификатор элемента сокращается для удобочитаемости.
  
```XML
<?xml version="1.0" encoding="utf-8"?>
   <CreateItemResponse xmlns="https://schemas.microsoft.com/exchange/services/2006/messages">
      <ResponseMessages xmlns="https://schemas.microsoft.com/exchange/services/2006/messages">
         <CreateItemResponseMessage ResponseClass="Success" 
             xmlns="https://schemas.microsoft.com/exchange/services/2006/messages">
            <ResponseCode xmlns="https://schemas.microsoft.com/exchange/services/2006/messages">
               NoError
            </ResponseCode>
            <Items xmlns="https://schemas.microsoft.com/exchange/services/2006/messages">
               <DistributionList xmlns="https://schemas.microsoft.com/exchange/services/2006/types">
                  <ItemId xmlns="https://schemas.microsoft.com/exchange/services/2006/types" 
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
    
- [Как: развернуть группы рассылки с помощью EWS в Exchange 2013](how-to-expand-distribution-groups-by-using-ews-in-exchange-2013.md)
    

