---
title: жетусеруфсеттингсрекуест
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- GetUserOofSettingsRequest
api_type:
- schema
ms.assetid: 15dea99c-7f5d-4af1-82ff-4255127fe567
description: Элемент Жетусеруфсеттингсрекуест является корневым элементом, который содержит аргументы, используемые для получения параметров отсутствия на работе пользователя почтового ящика (отсутствие на работе).
ms.openlocfilehash: f515e8cf016d3aff6c652ae92a0da71a8f0a5f6b
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/31/2020
ms.locfileid: "44457832"
---
# <a name="getuseroofsettingsrequest"></a><span data-ttu-id="70da7-103">жетусеруфсеттингсрекуест</span><span class="sxs-lookup"><span data-stu-id="70da7-103">GetUserOofSettingsRequest</span></span>

<span data-ttu-id="70da7-104">Элемент **жетусеруфсеттингсрекуест** является корневым элементом, который содержит аргументы, используемые для получения параметров отсутствия на работе пользователя почтового ящика (отсутствие на работе).</span><span class="sxs-lookup"><span data-stu-id="70da7-104">The **GetUserOofSettingsRequest** element is the root element that contains the arguments used to get a mailbox user's Out of Office (OOF) settings.</span></span> 
  
```xml
<GetUserOofSettingsRequest>
   <Mailbox>...</Mailbox>
</GetUserOofSettingsRequest>
```

 <span data-ttu-id="70da7-105">**жетусеруфсеттингсрекуест**</span><span class="sxs-lookup"><span data-stu-id="70da7-105">**GetUserOofSettingsRequest**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="70da7-106">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="70da7-106">Attributes and elements</span></span>

<span data-ttu-id="70da7-107">В следующих разделах описываются атрибуты, дочерние и родительские элементы.</span><span class="sxs-lookup"><span data-stu-id="70da7-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="70da7-108">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="70da7-108">Attributes</span></span>

<span data-ttu-id="70da7-109">Отсутствуют.</span><span class="sxs-lookup"><span data-stu-id="70da7-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="70da7-110">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="70da7-110">Child elements</span></span>

|<span data-ttu-id="70da7-111">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="70da7-111">**Element**</span></span>|<span data-ttu-id="70da7-112">**Описание**</span><span class="sxs-lookup"><span data-stu-id="70da7-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="70da7-113">Mailbox (доступность)</span><span class="sxs-lookup"><span data-stu-id="70da7-113">Mailbox (Availability)</span></span>](mailbox-availability.md) <br/> |<span data-ttu-id="70da7-114">Определяет пользователя почтового ящика для запроса SetUserOofSettings или GetUserOofSettings.</span><span class="sxs-lookup"><span data-stu-id="70da7-114">Identifies the mailbox user for a SetUserOofSettings or GetUserOofSettings request.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="70da7-115">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="70da7-115">Parent elements</span></span>

<span data-ttu-id="70da7-116">Нет.</span><span class="sxs-lookup"><span data-stu-id="70da7-116">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="70da7-117">Примечания</span><span class="sxs-lookup"><span data-stu-id="70da7-117">Remarks</span></span>

<span data-ttu-id="70da7-118">Схема, описывающая этот элемент, расположена в виртуальном каталоге EWS на компьютере с MicrosoftExchange Server 2007 и установленной ролью сервера клиентского доступа.</span><span class="sxs-lookup"><span data-stu-id="70da7-118">The schema that describes this element is located in the EWS virtual directory of the computer that is running MicrosoftExchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="example"></a><span data-ttu-id="70da7-119">Пример</span><span class="sxs-lookup"><span data-stu-id="70da7-119">Example</span></span>

<span data-ttu-id="70da7-120">Ниже приведен пример запроса GetUserOofSettings, который получает сведения об отсутствии на работе отдельных пользователей.</span><span class="sxs-lookup"><span data-stu-id="70da7-120">The following is an example of a GetUserOofSettings request that gets a single user's OOF information.</span></span>
  
```
<?xml version="1.0" encoding="utf-8"?>
<soap:Envelope xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" xmlns:xsd="http://www.w3.org/2001/XMLSchema" xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/">
  <soap:Body>
    <GetUserOofSettingsRequest xmlns="https://schemas.microsoft.com/exchange/services/2006/messages">
      <Mailbox xmlns="https://schemas.microsoft.com/exchange/services/2006/types">
        <Name>David Alexander</Name>
        <Address>someone@example.com</Address>
        <RoutingType>SMTP</RoutingType>
      </Mailbox>
    </GetUserOofSettingsRequest>
  </soap:Body>
</soap:Envelope>
```

## <a name="element-information"></a><span data-ttu-id="70da7-121">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="70da7-121">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="70da7-122">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="70da7-122">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="70da7-123">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="70da7-123">Schema Name</span></span>  <br/> |<span data-ttu-id="70da7-124">Схема Messages</span><span class="sxs-lookup"><span data-stu-id="70da7-124">Messages schema</span></span>  <br/> |
|<span data-ttu-id="70da7-125">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="70da7-125">Validation File</span></span>  <br/> |<span data-ttu-id="70da7-126">Messages. xsd</span><span class="sxs-lookup"><span data-stu-id="70da7-126">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="70da7-127">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="70da7-127">Can be Empty</span></span>  <br/> |<span data-ttu-id="70da7-128">False</span><span class="sxs-lookup"><span data-stu-id="70da7-128">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="70da7-129">См. также</span><span class="sxs-lookup"><span data-stu-id="70da7-129">See also</span></span>



[<span data-ttu-id="70da7-130">Операция GetUserOofSettings</span><span class="sxs-lookup"><span data-stu-id="70da7-130">GetUserOofSettings operation</span></span>](getuseroofsettings-operation.md)

