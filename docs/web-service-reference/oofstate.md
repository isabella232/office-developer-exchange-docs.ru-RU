---
title: уфстате
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
description: Элемент Уфстате используется для получения или задания состояния отсутствия на работе пользователя.
ms.openlocfilehash: 6aef7d989ee6978019a483f2673895e68a88a7c5
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/31/2020
ms.locfileid: "44459737"
---
# <a name="oofstate"></a><span data-ttu-id="7bfc4-103">уфстате</span><span class="sxs-lookup"><span data-stu-id="7bfc4-103">OofState</span></span>

<span data-ttu-id="7bfc4-104">Элемент **уфстате** используется для получения или задания состояния отсутствия на работе пользователя.</span><span class="sxs-lookup"><span data-stu-id="7bfc4-104">The **OofState** element is used to get or set the user's Out of Office (OOF) state.</span></span> 
  
```xml
<OofState>Disabled or Enabled or Scheduled</OofState>
```

 <span data-ttu-id="7bfc4-105">**уфстате**</span><span class="sxs-lookup"><span data-stu-id="7bfc4-105">**OofState**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="7bfc4-106">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="7bfc4-106">Attributes and elements</span></span>

<span data-ttu-id="7bfc4-107">В следующих разделах описываются атрибуты, дочерние и родительские элементы.</span><span class="sxs-lookup"><span data-stu-id="7bfc4-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="7bfc4-108">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="7bfc4-108">Attributes</span></span>

<span data-ttu-id="7bfc4-109">Отсутствуют.</span><span class="sxs-lookup"><span data-stu-id="7bfc4-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="7bfc4-110">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="7bfc4-110">Child elements</span></span>

<span data-ttu-id="7bfc4-111">Отсутствуют.</span><span class="sxs-lookup"><span data-stu-id="7bfc4-111">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="7bfc4-112">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="7bfc4-112">Parent elements</span></span>

|<span data-ttu-id="7bfc4-113">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="7bfc4-113">**Element**</span></span>|<span data-ttu-id="7bfc4-114">**Описание**</span><span class="sxs-lookup"><span data-stu-id="7bfc4-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="7bfc4-115">усеруфсеттингс</span><span class="sxs-lookup"><span data-stu-id="7bfc4-115">UserOofSettings</span></span>](useroofsettings.md) <br/> |<span data-ttu-id="7bfc4-116">Задает параметры отсутствия на работе.</span><span class="sxs-lookup"><span data-stu-id="7bfc4-116">Specifies the OOF settings.</span></span>  <br/> <span data-ttu-id="7bfc4-117">Ниже приведено выражение XPath для этого элемента:</span><span class="sxs-lookup"><span data-stu-id="7bfc4-117">The following is the XPath expression to this element:</span></span>  <br/>  `/SetUserOofSettingsRequest/UserOofSettings` <br/> |
|[<span data-ttu-id="7bfc4-118">уфсеттингс</span><span class="sxs-lookup"><span data-stu-id="7bfc4-118">OofSettings</span></span>](oofsettings.md) <br/> |<span data-ttu-id="7bfc4-119">Содержит параметры отсутствия на работе.</span><span class="sxs-lookup"><span data-stu-id="7bfc4-119">Contains the OOF settings.</span></span>  <br/> <span data-ttu-id="7bfc4-120">Ниже приведено выражение XPath для этого элемента:</span><span class="sxs-lookup"><span data-stu-id="7bfc4-120">The following is the XPath expression to this element:</span></span>  <br/>  `/GetUserOofSettingsResponse/OofSettings` <br/> |
   
## <a name="text-value"></a><span data-ttu-id="7bfc4-121">Текстовое значение</span><span class="sxs-lookup"><span data-stu-id="7bfc4-121">Text value</span></span>

<span data-ttu-id="7bfc4-122">Для элемента **уфстате** необходимо указать текстовое значение.</span><span class="sxs-lookup"><span data-stu-id="7bfc4-122">A text value is required for the **OofState** element.</span></span> <span data-ttu-id="7bfc4-123">Следующий список содержит возможные значения для этого элемента:</span><span class="sxs-lookup"><span data-stu-id="7bfc4-123">The following list contains the possible values for this element:</span></span> 
  
- <span data-ttu-id="7bfc4-124">**Disabled**</span><span class="sxs-lookup"><span data-stu-id="7bfc4-124">**Disabled**</span></span>
    
- <span data-ttu-id="7bfc4-125">**Enabled**</span><span class="sxs-lookup"><span data-stu-id="7bfc4-125">**Enabled**</span></span>
    
- <span data-ttu-id="7bfc4-126">**Scheduled**</span><span class="sxs-lookup"><span data-stu-id="7bfc4-126">**Scheduled**</span></span>
    
<span data-ttu-id="7bfc4-127">Значение **Schedule** указывает на то, что состояние неизвестных состояний " **включено** " в течение периода времени, определяемого элементом [Duration (усеруфсеттингс)](duration-useroofsettings.md) .</span><span class="sxs-lookup"><span data-stu-id="7bfc4-127">A value of **Scheduled** indicates that the OOF status is set to **Enabled** during a time period identified by the [Duration (UserOofSettings)](duration-useroofsettings.md) element.</span></span> 
  
## <a name="remarks"></a><span data-ttu-id="7bfc4-128">Примечания</span><span class="sxs-lookup"><span data-stu-id="7bfc4-128">Remarks</span></span>

<span data-ttu-id="7bfc4-129">Этот элемент является обязательным в сообщениях Сетусерсуфсеттингрекуест и Жетусеруфсеттингреспонсе.</span><span class="sxs-lookup"><span data-stu-id="7bfc4-129">This element is required in both the SetUsersOofSettingRequest message and the GetUserOofSettingResponse message.</span></span>
  
<span data-ttu-id="7bfc4-130">Схема, описывающая этот элемент, расположена в виртуальном каталоге EWS на компьютере с MicrosoftExchange Server 2007 и установленной ролью сервера клиентского доступа.</span><span class="sxs-lookup"><span data-stu-id="7bfc4-130">The schema that describes this element is located in the EWS virtual directory of the computer that is running MicrosoftExchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="example"></a><span data-ttu-id="7bfc4-131">Пример</span><span class="sxs-lookup"><span data-stu-id="7bfc4-131">Example</span></span>

<span data-ttu-id="7bfc4-132">Следующий пример запроса SetUserOofSettings включает **уфстате**.</span><span class="sxs-lookup"><span data-stu-id="7bfc4-132">The following example of a SetUserOofSettings request enables the **OofState**.</span></span>
  
```
<?xml version="1.0" encoding="utf-8"?>
<soap:Envelope xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" xmlns:xsd="http://www.w3.org/2001/XMLSchema" xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/">
  <soap:Body>
    <SetUserOofSettingsRequest xmlns="https://schemas.microsoft.com/exchange/services/2006/messages">
      <Mailbox xmlns="https://schemas.microsoft.com/exchange/services/2006/types">
        <Name>David Alexander</Name>
        <Address>someone@example.com</Address>
        <RoutingType>SMTP</RoutingType>
      </Mailbox>
      <UserOofSettings xmlns="https://schemas.microsoft.com/exchange/services/2006/types">
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

## <a name="element-information"></a><span data-ttu-id="7bfc4-133">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="7bfc4-133">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="7bfc4-134">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="7bfc4-134">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="7bfc4-135">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="7bfc4-135">Schema Name</span></span>  <br/> |<span data-ttu-id="7bfc4-136">Схема Types</span><span class="sxs-lookup"><span data-stu-id="7bfc4-136">Types schema</span></span>  <br/> |
|<span data-ttu-id="7bfc4-137">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="7bfc4-137">Validation File</span></span>  <br/> |<span data-ttu-id="7bfc4-138">Types. xsd</span><span class="sxs-lookup"><span data-stu-id="7bfc4-138">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="7bfc4-139">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="7bfc4-139">Can be Empty</span></span>  <br/> |<span data-ttu-id="7bfc4-140">False</span><span class="sxs-lookup"><span data-stu-id="7bfc4-140">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="7bfc4-141">См. также</span><span class="sxs-lookup"><span data-stu-id="7bfc4-141">See also</span></span>



[<span data-ttu-id="7bfc4-142">Операция GetUserOofSettings</span><span class="sxs-lookup"><span data-stu-id="7bfc4-142">GetUserOofSettings operation</span></span>](getuseroofsettings-operation.md)
  
[<span data-ttu-id="7bfc4-143">Операция SetUserOofSettings</span><span class="sxs-lookup"><span data-stu-id="7bfc4-143">SetUserOofSettings operation</span></span>](setuseroofsettings-operation.md)

