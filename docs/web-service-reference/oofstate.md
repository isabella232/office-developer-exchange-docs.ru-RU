---
title: OofState
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- OofState
api_type:
- schema
ms.assetid: 3c486a38-06da-4382-ad20-664d067d76ac
description: Элемент OofState используется для получения или задания состояния об отсутствии на работе Office (отсутствие на работе) пользователя.
ms.openlocfilehash: f97c050aec102b384fa4d98e6dee43befd4dc9ca
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/25/2018
ms.locfileid: "19834651"
---
# <a name="oofstate"></a><span data-ttu-id="afd56-103">OofState</span><span class="sxs-lookup"><span data-stu-id="afd56-103">OofState</span></span>

<span data-ttu-id="afd56-104">Элемент **OofState** используется для получения или задания состояния об отсутствии на работе Office (отсутствие на работе) пользователя.</span><span class="sxs-lookup"><span data-stu-id="afd56-104">The **OofState** element is used to get or set the user's Out of Office (OOF) state.</span></span> 
  
```xml
<OofState>Disabled or Enabled or Scheduled</OofState>
```

 <span data-ttu-id="afd56-105">**OofState**</span><span class="sxs-lookup"><span data-stu-id="afd56-105">**OofState**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="afd56-106">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="afd56-106">Attributes and elements</span></span>

<span data-ttu-id="afd56-107">В разделах ниже приводится описание атрибутов, дочерних и родительских элементов.</span><span class="sxs-lookup"><span data-stu-id="afd56-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="afd56-108">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="afd56-108">Attributes</span></span>

<span data-ttu-id="afd56-109">Нет.</span><span class="sxs-lookup"><span data-stu-id="afd56-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="afd56-110">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="afd56-110">Child elements</span></span>

<span data-ttu-id="afd56-111">Нет.</span><span class="sxs-lookup"><span data-stu-id="afd56-111">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="afd56-112">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="afd56-112">Parent elements</span></span>

|<span data-ttu-id="afd56-113">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="afd56-113">**Element**</span></span>|<span data-ttu-id="afd56-114">**Описание**</span><span class="sxs-lookup"><span data-stu-id="afd56-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="afd56-115">UserOofSettings</span><span class="sxs-lookup"><span data-stu-id="afd56-115">UserOofSettings</span></span>](useroofsettings.md) <br/> |<span data-ttu-id="afd56-116">Задает параметры об отсутствии на работе.</span><span class="sxs-lookup"><span data-stu-id="afd56-116">Specifies the OOF settings.</span></span>  <br/> <span data-ttu-id="afd56-117">Ниже приведен выражение XPath для этого элемента.</span><span class="sxs-lookup"><span data-stu-id="afd56-117">The following is the XPath expression to this element:</span></span>  <br/>  `/SetUserOofSettingsRequest/UserOofSettings` <br/> |
|[<span data-ttu-id="afd56-118">OofSettings</span><span class="sxs-lookup"><span data-stu-id="afd56-118">OofSettings</span></span>](oofsettings.md) <br/> |<span data-ttu-id="afd56-119">Содержит параметры об отсутствии на работе.</span><span class="sxs-lookup"><span data-stu-id="afd56-119">Contains the OOF settings.</span></span>  <br/> <span data-ttu-id="afd56-120">Ниже приведен выражение XPath для этого элемента.</span><span class="sxs-lookup"><span data-stu-id="afd56-120">The following is the XPath expression to this element:</span></span>  <br/>  `/GetUserOofSettingsResponse/OofSettings` <br/> |
   
## <a name="text-value"></a><span data-ttu-id="afd56-121">Текстовое значение</span><span class="sxs-lookup"><span data-stu-id="afd56-121">Text value</span></span>

<span data-ttu-id="afd56-122">Текстовое значение является обязательным для элемента **OofState** .</span><span class="sxs-lookup"><span data-stu-id="afd56-122">A text value is required for the **OofState** element.</span></span> <span data-ttu-id="afd56-123">Следующий список содержит возможные значения для этого элемента:</span><span class="sxs-lookup"><span data-stu-id="afd56-123">The following list contains the possible values for this element:</span></span> 
  
- <span data-ttu-id="afd56-124">**Отключено**</span><span class="sxs-lookup"><span data-stu-id="afd56-124">**Disabled**</span></span>
    
- <span data-ttu-id="afd56-125">**Включено**</span><span class="sxs-lookup"><span data-stu-id="afd56-125">**Enabled**</span></span>
    
- <span data-ttu-id="afd56-126">**Запланировано**</span><span class="sxs-lookup"><span data-stu-id="afd56-126">**Scheduled**</span></span>
    
<span data-ttu-id="afd56-127">Значение **Запланировано** указывает, что состояние об отсутствии на работе выбрано значение **Enabled** период времени, обнаруженных в элементе [продолжительность (UserOofSettings)](duration-useroofsettings.md) .</span><span class="sxs-lookup"><span data-stu-id="afd56-127">A value of **Scheduled** indicates that the OOF status is set to **Enabled** during a time period identified by the [Duration (UserOofSettings)](duration-useroofsettings.md) element.</span></span> 
  
## <a name="remarks"></a><span data-ttu-id="afd56-128">Замечания</span><span class="sxs-lookup"><span data-stu-id="afd56-128">Remarks</span></span>

<span data-ttu-id="afd56-129">Этот элемент является обязательным в SetUsersOofSettingRequest сообщений и сообщений GetUserOofSettingResponse.</span><span class="sxs-lookup"><span data-stu-id="afd56-129">This element is required in both the SetUsersOofSettingRequest message and the GetUserOofSettingResponse message.</span></span>
  
<span data-ttu-id="afd56-130">Схема, описывающая этот элемент, расположена в виртуальном каталоге EWS на компьютере с MicrosoftExchange Server 2007 и установленной ролью сервера клиентского доступа.</span><span class="sxs-lookup"><span data-stu-id="afd56-130">The schema that describes this element is located in the EWS virtual directory of the computer that is running MicrosoftExchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="example"></a><span data-ttu-id="afd56-131">Пример</span><span class="sxs-lookup"><span data-stu-id="afd56-131">Example</span></span>

<span data-ttu-id="afd56-132">В следующем примере запрос SetUserOofSettings включается **OofState**.</span><span class="sxs-lookup"><span data-stu-id="afd56-132">The following example of a SetUserOofSettings request enables the **OofState**.</span></span>
  
```
<?xml version="1.0" encoding="utf-8"?>
<soap:Envelope xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" xmlns:xsd="http://www.w3.org/2001/XMLSchema" xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/">
  <soap:Body>
    <SetUserOofSettingsRequest xmlns="http://schemas.microsoft.com/exchange/services/2006/messages">
      <Mailbox xmlns="http://schemas.microsoft.com/exchange/services/2006/types">
        <Name>David Alexander</Name>
        <Address>someone@example.com</Address>
        <RoutingType>SMTP</RoutingType>
      </Mailbox>
      <UserOofSettings xmlns="http://schemas.microsoft.com/exchange/services/2006/types">
        <OofState>Enabled</OofState>
        <ExternalAudience>All</ExternalAudience>
        <Duration>
          <StartTime>2005-10-05T00:00:00</StartTime>
          <EndTime>2005-10-25T00:00:00</EndTime>
        </Duration>
        <InternalReply>
          <Message>I am out of office.  This is my internal reply.</Message>
        </InternalReply>
        <ExternalReply>
          <Message>I am out of office. This is my external reply.</Message>
        </ExternalReply>
      </UserOofSettings>
    </SetUserOofSettingsRequest>
  </soap:Body>
</soap:Envelope>
```

## <a name="element-information"></a><span data-ttu-id="afd56-133">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="afd56-133">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="afd56-134">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="afd56-134">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="afd56-135">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="afd56-135">Schema Name</span></span>  <br/> |<span data-ttu-id="afd56-136">Схема Types</span><span class="sxs-lookup"><span data-stu-id="afd56-136">Types schema</span></span>  <br/> |
|<span data-ttu-id="afd56-137">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="afd56-137">Validation File</span></span>  <br/> |<span data-ttu-id="afd56-138">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="afd56-138">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="afd56-139">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="afd56-139">Can be Empty</span></span>  <br/> |<span data-ttu-id="afd56-140">False</span><span class="sxs-lookup"><span data-stu-id="afd56-140">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="afd56-141">См. также</span><span class="sxs-lookup"><span data-stu-id="afd56-141">See also</span></span>



[<span data-ttu-id="afd56-142">Операция GetUserOofSettings</span><span class="sxs-lookup"><span data-stu-id="afd56-142">GetUserOofSettings operation</span></span>](getuseroofsettings-operation.md)
  
[<span data-ttu-id="afd56-143">Операция SetUserOofSettings</span><span class="sxs-lookup"><span data-stu-id="afd56-143">SetUserOofSettings operation</span></span>](setuseroofsettings-operation.md)

