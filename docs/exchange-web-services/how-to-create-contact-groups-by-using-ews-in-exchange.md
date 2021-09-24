---
title: 'Как: создать группы контактов с помощью EWS в Exchange'
manager: sethgros
ms.date: 11/16/2014
ms.audience: Developer
ms.localizationpriority: medium
ms.assetid: acec6e73-c016-419d-be1a-8ec5d993addb
description: Узнайте, как создать контактную группу с помощью управляемого API или EWS EWS в Exchange.
ms.openlocfilehash: ade7fa68b00b055268cd5f0c34a75e0abbdb18ee
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/24/2021
ms.locfileid: "59513222"
---
# <a name="create-contact-groups-by-using-ews-in-exchange"></a>Как: создать группы контактов с помощью EWS в Exchange

Узнайте, как создать контактную группу с помощью управляемого API или EWS EWS в Exchange.
  
Вы можете создать контактную группу, которая является частной группой [рассылки,](distribution-groups-and-ews-in-exchange.md)с помощью управляемого API EWS или EWS. Для создания контактных групп используйте методы в классе управляемый API [ContactGroup](https://msdn.microsoft.com/library/office/microsoft.exchange.webservices.data.contactgroup%28v=exchg.80%29.aspx) EWS или используйте операцию [CreateItem](https://msdn.microsoft.com/library/78a52120-f1d0-4ed7-8748-436e554f75b6%28Office.15%29.aspx) EWS. 
  
Обратите внимание, что для создания универсальной группы рассылки или группы безопасности нельзя использовать управляемый API EWS или EWS. Чтобы создать универсальную группу рассылки или группу безопасности, можно использовать команды [New-DistributionGroup](https://technet.microsoft.com/library/aa998856%28v=exchg.150%29.aspx)[Exchange Management Shell.](https://msdn.microsoft.com/library/ff326159%28v=exchg.140%29.aspx) 
  
## <a name="create-a-contact-group-by-using-the-ews-managed-api"></a>Создание контактной группы с помощью управляемого API EWS
<a name="bk_EWSMA"> </a>

Чтобы создать контактную группу, необходимо просто добавить в группу несколько частей информации: имя группы и ее участников. В следующем примере показано, как создать простую контактную группу, которая содержит несколько членов группы.
  
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

## <a name="create-a-contact-group-by-using-ews"></a>Создание контактной группы с помощью EWS
<a name="bk_EWSMA"> </a>

Может потребоваться несколько строк кода, но можно создать контактную группу с помощью операции [CreateItem](https://msdn.microsoft.com/library/78a52120-f1d0-4ed7-8748-436e554f75b6%28Office.15%29.aspx) EWS. В следующем примере запроса XML показано, как создать контактную группу. Это также XML-запрос, который отправляется при использовании API управляемых [EWS для создания контактной группы.](#bk_EWSMA)
  
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

Ниже приводится пример успешного XML-ответа на запрос. Обратите внимание, что возвращенные значения включают код элемента для новой контактной группы и ключ изменения, который можно использовать в другом коде для изменения контактной группы или расширения группы, чтобы увидеть участников. ID элемента сокращается для читаемости.
  
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
    

