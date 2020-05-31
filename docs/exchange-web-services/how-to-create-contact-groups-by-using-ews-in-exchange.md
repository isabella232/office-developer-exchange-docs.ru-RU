---
title: 'Как: создать группы контактов с помощью EWS в Exchange'
manager: sethgros
ms.date: 11/16/2014
ms.audience: Developer
localization_priority: Normal
ms.assetid: acec6e73-c016-419d-be1a-8ec5d993addb
description: Узнайте, как создать группу контактов с помощью управляемого API EWS или EWS в Exchange.
ms.openlocfilehash: b3357f24e07a9c1b3b37ccb63b0f4f0d0a1d6fcf
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/25/2018
ms.locfileid: "19760992"
---
# <a name="create-contact-groups-by-using-ews-in-exchange"></a><span data-ttu-id="5fc48-103">Как: создать группы контактов с помощью EWS в Exchange</span><span class="sxs-lookup"><span data-stu-id="5fc48-103">Create contact groups by using EWS in Exchange</span></span>

<span data-ttu-id="5fc48-104">Узнайте, как создать группу контактов с помощью управляемого API EWS или EWS в Exchange.</span><span class="sxs-lookup"><span data-stu-id="5fc48-104">Learn how to create a contact group by using the EWS Managed API or EWS in Exchange.</span></span>
  
<span data-ttu-id="5fc48-105">Вы можете создать группу контактов, которая представляет собой частную [группу рассылки](distribution-groups-and-ews-in-exchange.md), с помощью управляемого API EWS или EWS.</span><span class="sxs-lookup"><span data-stu-id="5fc48-105">You can create a contact group, which is a private [distribution group](distribution-groups-and-ews-in-exchange.md), by using the EWS Managed API or EWS.</span></span> <span data-ttu-id="5fc48-106">Для создания групп контактов используйте методы в классе управляемого API [ContactGroup](http://msdn.microsoft.com/en-us/library/office/microsoft.exchange.webservices.data.contactgroup%28v=exchg.80%29.aspx) EWS или используйте операцию [CreateItem](http://msdn.microsoft.com/library/78a52120-f1d0-4ed7-8748-436e554f75b6%28Office.15%29.aspx) EWS.</span><span class="sxs-lookup"><span data-stu-id="5fc48-106">To create contact groups, use the methods in the [ContactGroup](http://msdn.microsoft.com/en-us/library/office/microsoft.exchange.webservices.data.contactgroup%28v=exchg.80%29.aspx) EWS Managed API class, or use the [CreateItem](http://msdn.microsoft.com/library/78a52120-f1d0-4ed7-8748-436e554f75b6%28Office.15%29.aspx) EWS operation.</span></span> 
  
<span data-ttu-id="5fc48-107">Обратите внимание, что вы не можете создать универсальную группу рассылки или группу безопасности с помощью управляемого API EWS или EWS.</span><span class="sxs-lookup"><span data-stu-id="5fc48-107">Note that you can't use the EWS Managed API or EWS to create a universal distribution group or security group.</span></span> <span data-ttu-id="5fc48-108">Чтобы создать универсальную группу рассылки или группу безопасности, можно использовать командлет [New – DistributionGroup](http://technet.microsoft.com/en-us/library/aa998856%28v=exchg.150%29.aspx)[Exchange Management Shell](http://msdn.microsoft.com/en-us/library/ff326159%28v=exchg.140%29.aspx).</span><span class="sxs-lookup"><span data-stu-id="5fc48-108">To create a universal distribution group or security group, you can use the [New-DistributionGroup](http://technet.microsoft.com/en-us/library/aa998856%28v=exchg.150%29.aspx)[Exchange Management Shell cmdlet](http://msdn.microsoft.com/en-us/library/ff326159%28v=exchg.140%29.aspx).</span></span> 
  
## <a name="create-a-contact-group-by-using-the-ews-managed-api"></a><span data-ttu-id="5fc48-109">Создание группы контактов с помощью управляемого API EWS</span><span class="sxs-lookup"><span data-stu-id="5fc48-109">Create a contact group by using the EWS Managed API</span></span>
<span data-ttu-id="5fc48-110"><a name="bk_EWSMA"> </a></span><span class="sxs-lookup"><span data-stu-id="5fc48-110"><a name="bk_EWSMA"> </a></span></span>

<span data-ttu-id="5fc48-111">Для создания группы контактов необходимо всего несколько сведений: имя группы и членов, добавляемых в группу.</span><span class="sxs-lookup"><span data-stu-id="5fc48-111">To create a contact group, you just need a couple pieces of information: a name for the group, and the members to add to the group.</span></span> <span data-ttu-id="5fc48-112">В приведенном ниже примере показано, как создать простую группу контактов, содержащую пару участников группы.</span><span class="sxs-lookup"><span data-stu-id="5fc48-112">The following example shows how to create a simple contact group that contains a couple of group members.</span></span>
  
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

## <a name="create-a-contact-group-by-using-ews"></a><span data-ttu-id="5fc48-113">Создание группы контактов с помощью EWS</span><span class="sxs-lookup"><span data-stu-id="5fc48-113">Create a contact group by using EWS</span></span>
<span data-ttu-id="5fc48-114"><a name="bk_EWSMA"> </a></span><span class="sxs-lookup"><span data-stu-id="5fc48-114"><a name="bk_EWSMA"> </a></span></span>

<span data-ttu-id="5fc48-115">Может потребоваться еще несколько строк кода, но вы можете создать группу контактов с помощью операции [CreateItem](http://msdn.microsoft.com/library/78a52120-f1d0-4ed7-8748-436e554f75b6%28Office.15%29.aspx) EWS.</span><span class="sxs-lookup"><span data-stu-id="5fc48-115">It might take a few more lines of code, but you can create a contact group by using the [CreateItem](http://msdn.microsoft.com/library/78a52120-f1d0-4ed7-8748-436e554f75b6%28Office.15%29.aspx) EWS operation.</span></span> <span data-ttu-id="5fc48-116">В приведенном ниже примере XML-запроса показано, как можно создать группу контактов.</span><span class="sxs-lookup"><span data-stu-id="5fc48-116">The following XML request example shows how you can create a contact group.</span></span> <span data-ttu-id="5fc48-117">Это также XML-запрос, который отправляется при [использовании управляемого API EWS для создания группы контактов](#bk_EWSMA).</span><span class="sxs-lookup"><span data-stu-id="5fc48-117">This is also the XML request that is sent when you [use the EWS Managed API to create a contact group](#bk_EWSMA).</span></span>
  
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

<span data-ttu-id="5fc48-118">Ниже приведен пример успешного XML-ответа на запрос.</span><span class="sxs-lookup"><span data-stu-id="5fc48-118">The following is an example of a successful XML response to the request.</span></span> <span data-ttu-id="5fc48-119">Обратите внимание, что возвращаемые значения включают идентификатор элемента для новой группы контактов и ключ изменения, который можно использовать в другом коде для изменения группы контактов или для развертывания группы, чтобы увидеть ее участников.</span><span class="sxs-lookup"><span data-stu-id="5fc48-119">Notice that the values returned include an item ID for the new contact group and a change key that you can use in other code to modify the contact group or expand the group to see the members.</span></span> <span data-ttu-id="5fc48-120">Идентификатор элемента сокращается для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="5fc48-120">The item ID is shortened for readability.</span></span>
  
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

## <a name="see-also"></a><span data-ttu-id="5fc48-121">См. также</span><span class="sxs-lookup"><span data-stu-id="5fc48-121">See also</span></span>


- [<span data-ttu-id="5fc48-122">Группы рассылки и EWS в Exchange</span><span class="sxs-lookup"><span data-stu-id="5fc48-122">Distribution groups and EWS in Exchange</span></span>](distribution-groups-and-ews-in-exchange.md)
    
- [<span data-ttu-id="5fc48-123">Как: развернуть группы рассылки с помощью EWS в Exchange 2013</span><span class="sxs-lookup"><span data-stu-id="5fc48-123">Expand distribution groups by using EWS in Exchange 2013</span></span>](how-to-expand-distribution-groups-by-using-ews-in-exchange-2013.md)
    

