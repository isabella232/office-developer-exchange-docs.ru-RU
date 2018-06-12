---
title: GetUserOofSettingsRequest
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
description: Элемент GetUserOofSettingsRequest является корневым элементом, который содержит аргументы, используемые для получения параметров из Office (отсутствие на работе) пользователя почтового ящика.
ms.openlocfilehash: e64818961283f90e447e2044cf7f918eccd21f06
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/11/2018
ms.locfileid: "19833692"
---
# <a name="getuseroofsettingsrequest"></a><span data-ttu-id="b15c6-103">GetUserOofSettingsRequest</span><span class="sxs-lookup"><span data-stu-id="b15c6-103">GetUserOofSettingsRequest</span></span>

<span data-ttu-id="b15c6-104">Элемент **GetUserOofSettingsRequest** является корневым элементом, который содержит аргументы, используемые для получения параметров из Office (отсутствие на работе) пользователя почтового ящика.</span><span class="sxs-lookup"><span data-stu-id="b15c6-104">The **GetUserOofSettingsRequest** element is the root element that contains the arguments used to get a mailbox user's Out of Office (OOF) settings.</span></span> 
  
```xml
<GetUserOofSettingsRequest>
   <Mailbox>...</Mailbox>
</GetUserOofSettingsRequest>
```

 <span data-ttu-id="b15c6-105">**GetUserOofSettingsRequest**</span><span class="sxs-lookup"><span data-stu-id="b15c6-105">**GetUserOofSettingsRequest**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="b15c6-106">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="b15c6-106">Attributes and elements</span></span>

<span data-ttu-id="b15c6-107">В разделах ниже приводится описание атрибутов, дочерних и родительских элементов.</span><span class="sxs-lookup"><span data-stu-id="b15c6-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="b15c6-108">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="b15c6-108">Attributes</span></span>

<span data-ttu-id="b15c6-109">Нет.</span><span class="sxs-lookup"><span data-stu-id="b15c6-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="b15c6-110">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="b15c6-110">Child elements</span></span>

|<span data-ttu-id="b15c6-111">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="b15c6-111">**Element**</span></span>|<span data-ttu-id="b15c6-112">**Описание**</span><span class="sxs-lookup"><span data-stu-id="b15c6-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="b15c6-113">Почтовый ящик (доступность)</span><span class="sxs-lookup"><span data-stu-id="b15c6-113">Mailbox (Availability)</span></span>](mailbox-availability.md) <br/> |<span data-ttu-id="b15c6-114">Идентифицирует пользователя почтового ящика для SetUserOofSettings или GetUserOofSettings запроса.</span><span class="sxs-lookup"><span data-stu-id="b15c6-114">Identifies the mailbox user for a SetUserOofSettings or GetUserOofSettings request.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="b15c6-115">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="b15c6-115">Parent elements</span></span>

<span data-ttu-id="b15c6-116">Нет.</span><span class="sxs-lookup"><span data-stu-id="b15c6-116">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="b15c6-117">Замечания</span><span class="sxs-lookup"><span data-stu-id="b15c6-117">Remarks</span></span>

<span data-ttu-id="b15c6-118">Схема, описывающая этот элемент, расположена в виртуальном каталоге EWS на компьютере с MicrosoftExchange Server 2007 и установленной ролью сервера клиентского доступа.</span><span class="sxs-lookup"><span data-stu-id="b15c6-118">The schema that describes this element is located in the EWS virtual directory of the computer that is running MicrosoftExchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="example"></a><span data-ttu-id="b15c6-119">Пример</span><span class="sxs-lookup"><span data-stu-id="b15c6-119">Example</span></span>

<span data-ttu-id="b15c6-120">Ниже приведен пример GetUserOofSettings запрос, который получает сведения об отсутствии на работе одного пользователя.</span><span class="sxs-lookup"><span data-stu-id="b15c6-120">The following is an example of a GetUserOofSettings request that gets a single user's OOF information.</span></span>
  
```
<?xml version="1.0" encoding="utf-8"?>
<soap:Envelope xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" xmlns:xsd="http://www.w3.org/2001/XMLSchema" xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/">
  <soap:Body>
    <GetUserOofSettingsRequest xmlns="http://schemas.microsoft.com/exchange/services/2006/messages">
      <Mailbox xmlns="http://schemas.microsoft.com/exchange/services/2006/types">
        <Name>David Alexander</Name>
        <Address>someone@example.com</Address>
        <RoutingType>SMTP</RoutingType>
      </Mailbox>
    </GetUserOofSettingsRequest>
  </soap:Body>
</soap:Envelope>
```

## <a name="element-information"></a><span data-ttu-id="b15c6-121">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="b15c6-121">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="b15c6-122">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="b15c6-122">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="b15c6-123">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="b15c6-123">Schema Name</span></span>  <br/> |<span data-ttu-id="b15c6-124">Схема Messages</span><span class="sxs-lookup"><span data-stu-id="b15c6-124">Messages schema</span></span>  <br/> |
|<span data-ttu-id="b15c6-125">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="b15c6-125">Validation File</span></span>  <br/> |<span data-ttu-id="b15c6-126">Messages.xsd</span><span class="sxs-lookup"><span data-stu-id="b15c6-126">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="b15c6-127">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="b15c6-127">Can be Empty</span></span>  <br/> |<span data-ttu-id="b15c6-128">False</span><span class="sxs-lookup"><span data-stu-id="b15c6-128">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="b15c6-129">См. также</span><span class="sxs-lookup"><span data-stu-id="b15c6-129">See also</span></span>



[<span data-ttu-id="b15c6-130">Операция GetUserOofSettings</span><span class="sxs-lookup"><span data-stu-id="b15c6-130">GetUserOofSettings operation</span></span>](getuseroofsettings-operation.md)

