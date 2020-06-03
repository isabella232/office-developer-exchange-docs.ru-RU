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
# <a name="create-contact-groups-by-using-ews-in-exchange"></a><span data-ttu-id="b3026-103">Как: создать группы контактов с помощью EWS в Exchange</span><span class="sxs-lookup"><span data-stu-id="b3026-103">Create contact groups by using EWS in Exchange</span></span>

<span data-ttu-id="b3026-104">Узнайте, как создать группу контактов с помощью управляемого API EWS или EWS в Exchange.</span><span class="sxs-lookup"><span data-stu-id="b3026-104">Learn how to create a contact group by using the EWS Managed API or EWS in Exchange.</span></span>
  
<span data-ttu-id="b3026-105">Вы можете создать группу контактов, которая представляет собой частную [группу рассылки](distribution-groups-and-ews-in-exchange.md), с помощью управляемого API EWS или EWS.</span><span class="sxs-lookup"><span data-stu-id="b3026-105">You can create a contact group, which is a private [distribution group](distribution-groups-and-ews-in-exchange.md), by using the EWS Managed API or EWS.</span></span> <span data-ttu-id="b3026-106">Для создания групп контактов используйте методы в классе управляемого API [ContactGroup](https://msdn.microsoft.com/library/office/microsoft.exchange.webservices.data.contactgroup%28v=exchg.80%29.aspx) EWS или используйте операцию [CreateItem](https://msdn.microsoft.com/library/78a52120-f1d0-4ed7-8748-436e554f75b6%28Office.15%29.aspx) EWS.</span><span class="sxs-lookup"><span data-stu-id="b3026-106">To create contact groups, use the methods in the [ContactGroup](https://msdn.microsoft.com/library/office/microsoft.exchange.webservices.data.contactgroup%28v=exchg.80%29.aspx) EWS Managed API class, or use the [CreateItem](https://msdn.microsoft.com/library/78a52120-f1d0-4ed7-8748-436e554f75b6%28Office.15%29.aspx) EWS operation.</span></span> 
  
<span data-ttu-id="b3026-107">Обратите внимание, что вы не можете создать универсальную группу рассылки или группу безопасности с помощью управляемого API EWS или EWS.</span><span class="sxs-lookup"><span data-stu-id="b3026-107">Note that you can't use the EWS Managed API or EWS to create a universal distribution group or security group.</span></span> <span data-ttu-id="b3026-108">Чтобы создать универсальную группу рассылки или группу безопасности, можно использовать командлет [New – DistributionGroup](https://technet.microsoft.com/library/aa998856%28v=exchg.150%29.aspx)[Exchange Management Shell](https://msdn.microsoft.com/library/ff326159%28v=exchg.140%29.aspx).</span><span class="sxs-lookup"><span data-stu-id="b3026-108">To create a universal distribution group or security group, you can use the [New-DistributionGroup](https://technet.microsoft.com/library/aa998856%28v=exchg.150%29.aspx)[Exchange Management Shell cmdlet](https://msdn.microsoft.com/library/ff326159%28v=exchg.140%29.aspx).</span></span> 
  
## <a name="create-a-contact-group-by-using-the-ews-managed-api"></a><span data-ttu-id="b3026-109">Создание группы контактов с помощью управляемого API EWS</span><span class="sxs-lookup"><span data-stu-id="b3026-109">Create a contact group by using the EWS Managed API</span></span>
<span data-ttu-id="b3026-110"><a name="bk_EWSMA"> </a></span><span class="sxs-lookup"><span data-stu-id="b3026-110"><a name="bk_EWSMA"> </a></span></span>

<span data-ttu-id="b3026-111">Для создания группы контактов необходимо всего несколько сведений: имя группы и членов, добавляемых в группу.</span><span class="sxs-lookup"><span data-stu-id="b3026-111">To create a contact group, you just need a couple pieces of information: a name for the group, and the members to add to the group.</span></span> <span data-ttu-id="b3026-112">В приведенном ниже примере показано, как создать простую группу контактов, содержащую пару участников группы.</span><span class="sxs-lookup"><span data-stu-id="b3026-112">The following example shows how to create a simple contact group that contains a couple of group members.</span></span>
  
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

## <a name="create-a-contact-group-by-using-ews"></a><span data-ttu-id="b3026-113">Создание группы контактов с помощью EWS</span><span class="sxs-lookup"><span data-stu-id="b3026-113">Create a contact group by using EWS</span></span>
<span data-ttu-id="b3026-114"><a name="bk_EWSMA"> </a></span><span class="sxs-lookup"><span data-stu-id="b3026-114"><a name="bk_EWSMA"> </a></span></span>

<span data-ttu-id="b3026-115">Может потребоваться еще несколько строк кода, но вы можете создать группу контактов с помощью операции [CreateItem](https://msdn.microsoft.com/library/78a52120-f1d0-4ed7-8748-436e554f75b6%28Office.15%29.aspx) EWS.</span><span class="sxs-lookup"><span data-stu-id="b3026-115">It might take a few more lines of code, but you can create a contact group by using the [CreateItem](https://msdn.microsoft.com/library/78a52120-f1d0-4ed7-8748-436e554f75b6%28Office.15%29.aspx) EWS operation.</span></span> <span data-ttu-id="b3026-116">В приведенном ниже примере XML-запроса показано, как можно создать группу контактов.</span><span class="sxs-lookup"><span data-stu-id="b3026-116">The following XML request example shows how you can create a contact group.</span></span> <span data-ttu-id="b3026-117">Это также XML-запрос, который отправляется при [использовании управляемого API EWS для создания группы контактов](#bk_EWSMA).</span><span class="sxs-lookup"><span data-stu-id="b3026-117">This is also the XML request that is sent when you [use the EWS Managed API to create a contact group](#bk_EWSMA).</span></span>
  
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

<span data-ttu-id="b3026-118">Ниже приведен пример успешного XML-ответа на запрос.</span><span class="sxs-lookup"><span data-stu-id="b3026-118">The following is an example of a successful XML response to the request.</span></span> <span data-ttu-id="b3026-119">Обратите внимание, что возвращаемые значения включают идентификатор элемента для новой группы контактов и ключ изменения, который можно использовать в другом коде для изменения группы контактов или для развертывания группы, чтобы увидеть ее участников.</span><span class="sxs-lookup"><span data-stu-id="b3026-119">Notice that the values returned include an item ID for the new contact group and a change key that you can use in other code to modify the contact group or expand the group to see the members.</span></span> <span data-ttu-id="b3026-120">Идентификатор элемента сокращается для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="b3026-120">The item ID is shortened for readability.</span></span>
  
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

## <a name="see-also"></a><span data-ttu-id="b3026-121">См. также</span><span class="sxs-lookup"><span data-stu-id="b3026-121">See also</span></span>


- [<span data-ttu-id="b3026-122">Группы рассылки и EWS в Exchange</span><span class="sxs-lookup"><span data-stu-id="b3026-122">Distribution groups and EWS in Exchange</span></span>](distribution-groups-and-ews-in-exchange.md)
    
- [<span data-ttu-id="b3026-123">Как: развернуть группы рассылки с помощью EWS в Exchange 2013</span><span class="sxs-lookup"><span data-stu-id="b3026-123">Expand distribution groups by using EWS in Exchange 2013</span></span>](how-to-expand-distribution-groups-by-using-ews-in-exchange-2013.md)
    

