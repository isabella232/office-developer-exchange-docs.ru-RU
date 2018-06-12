---
title: SetUserOofSettingsRequest
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- SetUserOofSettingsRequest
api_type:
- schema
ms.assetid: 628acf0b-3ebc-42f1-8ce2-7a02b4c8141f
description: Элемент SetUserOofSettingsRequest содержит аргументы, используемые для настройки почтового ящика пользователя об отсутствии на работе Office (отсутствие на работе).
ms.openlocfilehash: ed54bb1d066da7b15605fb81931a6ef75dfc61bf
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/11/2018
ms.locfileid: "19835474"
---
# <a name="setuseroofsettingsrequest"></a><span data-ttu-id="42585-103">SetUserOofSettingsRequest</span><span class="sxs-lookup"><span data-stu-id="42585-103">SetUserOofSettingsRequest</span></span>

<span data-ttu-id="42585-104">Элемент **SetUserOofSettingsRequest** содержит аргументы, используемые для настройки почтового ящика пользователя об отсутствии на работе Office (отсутствие на работе).</span><span class="sxs-lookup"><span data-stu-id="42585-104">The **SetUserOofSettingsRequest** element contains the arguments used to set a mailbox user's Out of Office (OOF) settings.</span></span> 
  
```xml
<SetUserOofSettingsRequest>
   <Mailbox>...</Mailbox>
   <UserOofSettings>...</UserOofSettings>
<SetUserOofSettingsRequest>
```

 <span data-ttu-id="42585-105">**SetUserOofSettingsRequest**</span><span class="sxs-lookup"><span data-stu-id="42585-105">**SetUserOofSettingsRequest**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="42585-106">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="42585-106">Attributes and elements</span></span>

<span data-ttu-id="42585-107">В разделах ниже приводится описание атрибутов, дочерних и родительских элементов.</span><span class="sxs-lookup"><span data-stu-id="42585-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="42585-108">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="42585-108">Attributes</span></span>

<span data-ttu-id="42585-109">Нет.</span><span class="sxs-lookup"><span data-stu-id="42585-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="42585-110">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="42585-110">Child elements</span></span>

|<span data-ttu-id="42585-111">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="42585-111">**Element**</span></span>|<span data-ttu-id="42585-112">**Описание**</span><span class="sxs-lookup"><span data-stu-id="42585-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="42585-113">Почтовый ящик (доступность)</span><span class="sxs-lookup"><span data-stu-id="42585-113">Mailbox (Availability)</span></span>](mailbox-availability.md) <br/> |<span data-ttu-id="42585-114">Идентифицирует пользователя почтового ящика для SetUserOofSettings или GetUserOofSettings запроса.</span><span class="sxs-lookup"><span data-stu-id="42585-114">Identifies the mailbox user for a SetUserOofSettings or GetUserOofSettings request.</span></span>  <br/> |
|[<span data-ttu-id="42585-115">UserOofSettings</span><span class="sxs-lookup"><span data-stu-id="42585-115">UserOofSettings</span></span>](useroofsettings.md) <br/> |<span data-ttu-id="42585-116">Задает параметры об отсутствии на работе.</span><span class="sxs-lookup"><span data-stu-id="42585-116">Specifies the OOF settings.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="42585-117">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="42585-117">Parent elements</span></span>

<span data-ttu-id="42585-118">Нет.</span><span class="sxs-lookup"><span data-stu-id="42585-118">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="42585-119">Замечания</span><span class="sxs-lookup"><span data-stu-id="42585-119">Remarks</span></span>

<span data-ttu-id="42585-120">Схема, описывающая этот элемент, расположена в виртуальном каталоге EWS на компьютере с MicrosoftExchange Server 2007 и установленной ролью сервера клиентского доступа.</span><span class="sxs-lookup"><span data-stu-id="42585-120">The schema that describes this element is located in the EWS virtual directory of the computer that is running MicrosoftExchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="example"></a><span data-ttu-id="42585-121">Пример</span><span class="sxs-lookup"><span data-stu-id="42585-121">Example</span></span>

<span data-ttu-id="42585-122">В следующем примере запрос SetUserOofSettings задается параметром об отсутствии на работе для 10 дней.</span><span class="sxs-lookup"><span data-stu-id="42585-122">The following example of a SetUserOofSettings request sets an OOF setting for ten days.</span></span>
  
```xml
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

## <a name="element-information"></a><span data-ttu-id="42585-123">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="42585-123">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="42585-124">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="42585-124">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="42585-125">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="42585-125">Schema Name</span></span>  <br/> |<span data-ttu-id="42585-126">Схема Messages</span><span class="sxs-lookup"><span data-stu-id="42585-126">Messages schema</span></span>  <br/> |
|<span data-ttu-id="42585-127">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="42585-127">Validation File</span></span>  <br/> |<span data-ttu-id="42585-128">Messages.xsd</span><span class="sxs-lookup"><span data-stu-id="42585-128">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="42585-129">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="42585-129">Can be Empty</span></span>  <br/> |<span data-ttu-id="42585-130">False</span><span class="sxs-lookup"><span data-stu-id="42585-130">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="42585-131">См. также</span><span class="sxs-lookup"><span data-stu-id="42585-131">See also</span></span>



[<span data-ttu-id="42585-132">Операция SetUserOofSettings</span><span class="sxs-lookup"><span data-stu-id="42585-132">SetUserOofSettings operation</span></span>](setuseroofsettings-operation.md)

