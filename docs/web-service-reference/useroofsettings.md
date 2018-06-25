---
title: UserOofSettings
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- UserOofSettings
api_type:
- schema
ms.assetid: 0a95ca63-660e-4cc0-82e4-3f74fb4ae21c
description: Элемент UserOofSettings указывает параметры об отсутствии на работе Office (отсутствие на работе).
ms.openlocfilehash: a035fd89387ece632d83f5f72a564e4896bc6753
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/25/2018
ms.locfileid: "19840433"
---
# <a name="useroofsettings"></a><span data-ttu-id="735a5-103">UserOofSettings</span><span class="sxs-lookup"><span data-stu-id="735a5-103">UserOofSettings</span></span>

<span data-ttu-id="735a5-104">Элемент **UserOofSettings** указывает параметры об отсутствии на работе Office (отсутствие на работе).</span><span class="sxs-lookup"><span data-stu-id="735a5-104">The **UserOofSettings** element specifies the Out of Office (OOF) settings.</span></span> 
  
[<span data-ttu-id="735a5-105">SetUserOofSettingsRequest</span><span class="sxs-lookup"><span data-stu-id="735a5-105">SetUserOofSettingsRequest</span></span>](setuseroofsettingsrequest.md)
  
[<span data-ttu-id="735a5-106">UserOofSettings</span><span class="sxs-lookup"><span data-stu-id="735a5-106">UserOofSettings</span></span>](useroofsettings.md)
  
```xml
<UserOofSettings>
   <OofState>...</OofState>
   <ExternalAudience>...</ExternalAudience>
   <Duration>...</Duration>
   <InternalReply>...</InternalReply>
   <ExternalReply>...</ExternalReply>
</UserOofSettings>
```

 <span data-ttu-id="735a5-107">**UserOofSettings**</span><span class="sxs-lookup"><span data-stu-id="735a5-107">**UserOofSettings**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="735a5-108">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="735a5-108">Attributes and elements</span></span>

<span data-ttu-id="735a5-109">В разделах ниже приводится описание атрибутов, дочерних и родительских элементов.</span><span class="sxs-lookup"><span data-stu-id="735a5-109">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="735a5-110">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="735a5-110">Attributes</span></span>

<span data-ttu-id="735a5-111">Нет.</span><span class="sxs-lookup"><span data-stu-id="735a5-111">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="735a5-112">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="735a5-112">Child elements</span></span>

|<span data-ttu-id="735a5-113">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="735a5-113">**Element**</span></span>|<span data-ttu-id="735a5-114">**Описание**</span><span class="sxs-lookup"><span data-stu-id="735a5-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="735a5-115">OofState</span><span class="sxs-lookup"><span data-stu-id="735a5-115">OofState</span></span>](oofstate.md) <br/> |<span data-ttu-id="735a5-116">Задает состояние пользователя об отсутствии на работе.</span><span class="sxs-lookup"><span data-stu-id="735a5-116">Sets the user's OOF state.</span></span>  <br/> |
|[<span data-ttu-id="735a5-117">ExternalAudience</span><span class="sxs-lookup"><span data-stu-id="735a5-117">ExternalAudience</span></span>](externalaudience.md) <br/> |<span data-ttu-id="735a5-118">Задает или содержит значение, определяющее, которому отправляются внешних сообщений об отсутствии на работе.</span><span class="sxs-lookup"><span data-stu-id="735a5-118">Sets or contains a value that determines to whom external OOF messages are sent.</span></span>  <br/> |
|[<span data-ttu-id="735a5-119">Продолжительность (UserOofSettings)</span><span class="sxs-lookup"><span data-stu-id="735a5-119">Duration (UserOofSettings)</span></span>](duration-useroofsettings.md) <br/> |<span data-ttu-id="735a5-120">Указывает, во время выполнения, для которого включен состояние об отсутствии на работе, если элемент [OofState](oofstate.md) задано значение **Запланировано**.</span><span class="sxs-lookup"><span data-stu-id="735a5-120">Specifies the duration for which the OOF status is enabled if the [OofState](oofstate.md) element is set to **Scheduled**.</span></span> <span data-ttu-id="735a5-121">Если элемент [OofState](oofstate.md) — это значение **включено** или **отключено**, значение этого элемента игнорируется.</span><span class="sxs-lookup"><span data-stu-id="735a5-121">If the [OofState](oofstate.md) element is set to **Enabled** or **Disabled**, the value of this element is ignored.</span></span>  <br/> |
|[<span data-ttu-id="735a5-122">InternalReply</span><span class="sxs-lookup"><span data-stu-id="735a5-122">InternalReply</span></span>](internalreply.md) <br/> |<span data-ttu-id="735a5-123">Содержит ответа об отсутствии на работе, для других пользователей в домене или доверенных доменов пользователя.</span><span class="sxs-lookup"><span data-stu-id="735a5-123">Contains the OOF response sent to other users in the user's domain or trusted domains.</span></span>  <br/> |
|[<span data-ttu-id="735a5-124">ExternalReply</span><span class="sxs-lookup"><span data-stu-id="735a5-124">ExternalReply</span></span>](externalreply.md) <br/> |<span data-ttu-id="735a5-125">Содержит отправлено адресам за пределами домена или доверенных доменов получателя ответов об отсутствии на работе.</span><span class="sxs-lookup"><span data-stu-id="735a5-125">Contains the OOF response sent to addresses outside the recipient's domain or trusted domains.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="735a5-126">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="735a5-126">Parent elements</span></span>

|<span data-ttu-id="735a5-127">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="735a5-127">**Element**</span></span>|<span data-ttu-id="735a5-128">**Описание**</span><span class="sxs-lookup"><span data-stu-id="735a5-128">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="735a5-129">SetUserOofSettingsRequest</span><span class="sxs-lookup"><span data-stu-id="735a5-129">SetUserOofSettingsRequest</span></span>](setuseroofsettingsrequest.md) <br/> |<span data-ttu-id="735a5-130">Содержит аргументы, используется для задания параметров об отсутствии на работе и сообщения пользователя почтового ящика.</span><span class="sxs-lookup"><span data-stu-id="735a5-130">Contains the arguments used to set a mailbox user's OOF settings and messages.</span></span>  <br/> <span data-ttu-id="735a5-131">Ниже приведен выражение XPath для этого элемента.</span><span class="sxs-lookup"><span data-stu-id="735a5-131">The following is the XPath expression to this element:</span></span>  <br/>  `/SetUserOofSettingsRequest` <br/> |
   
## <a name="remarks"></a><span data-ttu-id="735a5-132">Замечания</span><span class="sxs-lookup"><span data-stu-id="735a5-132">Remarks</span></span>

<span data-ttu-id="735a5-133">Схема, описывающая этот элемент, расположена в виртуальном каталоге EWS на компьютере с MicrosoftExchange Server 2007 и установленной ролью сервера клиентского доступа.</span><span class="sxs-lookup"><span data-stu-id="735a5-133">The schema that describes this element is located in the EWS virtual directory of the computer that is running MicrosoftExchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="example"></a><span data-ttu-id="735a5-134">Пример</span><span class="sxs-lookup"><span data-stu-id="735a5-134">Example</span></span>

<span data-ttu-id="735a5-135">В следующем примере запроса SetUserOofSettings задает OoFState **включена**, задает длительность об отсутствии на работе для 10 дней и задает внешних и внутренних сообщений об отсутствии на работе.</span><span class="sxs-lookup"><span data-stu-id="735a5-135">The following example of a SetUserOofSettings request sets the OoFState to **Enabled**, sets the duration of OOF for 10 days, and sets the internal and external OOF messages.</span></span>
  
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

## <a name="element-information"></a><span data-ttu-id="735a5-136">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="735a5-136">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="735a5-137">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="735a5-137">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="735a5-138">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="735a5-138">Schema Name</span></span>  <br/> |<span data-ttu-id="735a5-139">Схема сообщения</span><span class="sxs-lookup"><span data-stu-id="735a5-139">messages schema</span></span>  <br/> |
|<span data-ttu-id="735a5-140">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="735a5-140">Validation File</span></span>  <br/> |<span data-ttu-id="735a5-141">Messages.xsd</span><span class="sxs-lookup"><span data-stu-id="735a5-141">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="735a5-142">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="735a5-142">Can be Empty</span></span>  <br/> |<span data-ttu-id="735a5-143">False</span><span class="sxs-lookup"><span data-stu-id="735a5-143">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="735a5-144">См. также</span><span class="sxs-lookup"><span data-stu-id="735a5-144">See also</span></span>

- [<span data-ttu-id="735a5-145">Операция SetUserOofSettings</span><span class="sxs-lookup"><span data-stu-id="735a5-145">SetUserOofSettings operation</span></span>](setuseroofsettings-operation.md)

