---
title: усеруфсеттингс
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
description: Элемент Усеруфсеттингс указывает параметры заместителя (отсутствие на работе).
ms.openlocfilehash: 417c3d5061a6229d41eb57f72e89f03213acf460
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/31/2020
ms.locfileid: "44461907"
---
# <a name="useroofsettings"></a><span data-ttu-id="aaca1-103">усеруфсеттингс</span><span class="sxs-lookup"><span data-stu-id="aaca1-103">UserOofSettings</span></span>

<span data-ttu-id="aaca1-104">Элемент **усеруфсеттингс** указывает параметры заместителя (отсутствие на работе).</span><span class="sxs-lookup"><span data-stu-id="aaca1-104">The **UserOofSettings** element specifies the Out of Office (OOF) settings.</span></span> 
  
[<span data-ttu-id="aaca1-105">сетусеруфсеттингсрекуест</span><span class="sxs-lookup"><span data-stu-id="aaca1-105">SetUserOofSettingsRequest</span></span>](setuseroofsettingsrequest.md)
  
[<span data-ttu-id="aaca1-106">усеруфсеттингс</span><span class="sxs-lookup"><span data-stu-id="aaca1-106">UserOofSettings</span></span>](useroofsettings.md)
  
```xml
<UserOofSettings>
   <OofState>...</OofState>
   <ExternalAudience>...</ExternalAudience>
   <Duration>...</Duration>
   <InternalReply>...</InternalReply>
   <ExternalReply>...</ExternalReply>
</UserOofSettings>
```

 <span data-ttu-id="aaca1-107">**усеруфсеттингс**</span><span class="sxs-lookup"><span data-stu-id="aaca1-107">**UserOofSettings**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="aaca1-108">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="aaca1-108">Attributes and elements</span></span>

<span data-ttu-id="aaca1-109">В следующих разделах описываются атрибуты, дочерние и родительские элементы.</span><span class="sxs-lookup"><span data-stu-id="aaca1-109">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="aaca1-110">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="aaca1-110">Attributes</span></span>

<span data-ttu-id="aaca1-111">Отсутствуют.</span><span class="sxs-lookup"><span data-stu-id="aaca1-111">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="aaca1-112">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="aaca1-112">Child elements</span></span>

|<span data-ttu-id="aaca1-113">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="aaca1-113">**Element**</span></span>|<span data-ttu-id="aaca1-114">**Описание**</span><span class="sxs-lookup"><span data-stu-id="aaca1-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="aaca1-115">уфстате</span><span class="sxs-lookup"><span data-stu-id="aaca1-115">OofState</span></span>](oofstate.md) <br/> |<span data-ttu-id="aaca1-116">Задает состояние отсутствия на работе пользователя.</span><span class="sxs-lookup"><span data-stu-id="aaca1-116">Sets the user's OOF state.</span></span>  <br/> |
|[<span data-ttu-id="aaca1-117">екстерналаудиенце</span><span class="sxs-lookup"><span data-stu-id="aaca1-117">ExternalAudience</span></span>](externalaudience.md) <br/> |<span data-ttu-id="aaca1-118">Задает или содержит значение, которое определяет, кому отправляются внешние сообщения об отсутствии на работе.</span><span class="sxs-lookup"><span data-stu-id="aaca1-118">Sets or contains a value that determines to whom external OOF messages are sent.</span></span>  <br/> |
|[<span data-ttu-id="aaca1-119">Продолжительность (Усеруфсеттингс)</span><span class="sxs-lookup"><span data-stu-id="aaca1-119">Duration (UserOofSettings)</span></span>](duration-useroofsettings.md) <br/> |<span data-ttu-id="aaca1-120">Указывает срок, в течение которого состояние отсутствия на работе включено, если для элемента [уфстате](oofstate.md) задано значение " **запланировано**".</span><span class="sxs-lookup"><span data-stu-id="aaca1-120">Specifies the duration for which the OOF status is enabled if the [OofState](oofstate.md) element is set to **Scheduled**.</span></span> <span data-ttu-id="aaca1-121">Если для элемента [уфстате](oofstate.md) задано значение **Enabled** или **disabled**, значение этого элемента игнорируется.</span><span class="sxs-lookup"><span data-stu-id="aaca1-121">If the [OofState](oofstate.md) element is set to **Enabled** or **Disabled**, the value of this element is ignored.</span></span>  <br/> |
|[<span data-ttu-id="aaca1-122">интерналрепли</span><span class="sxs-lookup"><span data-stu-id="aaca1-122">InternalReply</span></span>](internalreply.md) <br/> |<span data-ttu-id="aaca1-123">Содержит ответ о нерабочем месте, отправленный другим пользователям в домене пользователя или доверенных доменах.</span><span class="sxs-lookup"><span data-stu-id="aaca1-123">Contains the OOF response sent to other users in the user's domain or trusted domains.</span></span>  <br/> |
|[<span data-ttu-id="aaca1-124">екстерналрепли</span><span class="sxs-lookup"><span data-stu-id="aaca1-124">ExternalReply</span></span>](externalreply.md) <br/> |<span data-ttu-id="aaca1-125">Содержит ответ о нерабочем месте, отправленный на адреса, не входящие в домен получателя или доверенные домены.</span><span class="sxs-lookup"><span data-stu-id="aaca1-125">Contains the OOF response sent to addresses outside the recipient's domain or trusted domains.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="aaca1-126">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="aaca1-126">Parent elements</span></span>

|<span data-ttu-id="aaca1-127">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="aaca1-127">**Element**</span></span>|<span data-ttu-id="aaca1-128">**Описание**</span><span class="sxs-lookup"><span data-stu-id="aaca1-128">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="aaca1-129">сетусеруфсеттингсрекуест</span><span class="sxs-lookup"><span data-stu-id="aaca1-129">SetUserOofSettingsRequest</span></span>](setuseroofsettingsrequest.md) <br/> |<span data-ttu-id="aaca1-130">Содержит аргументы, используемые для задания параметров и сообщений о нежелательных пользователя почтового ящика.</span><span class="sxs-lookup"><span data-stu-id="aaca1-130">Contains the arguments used to set a mailbox user's OOF settings and messages.</span></span>  <br/> <span data-ttu-id="aaca1-131">Ниже приведено выражение XPath для этого элемента:</span><span class="sxs-lookup"><span data-stu-id="aaca1-131">The following is the XPath expression to this element:</span></span>  <br/>  `/SetUserOofSettingsRequest` <br/> |
   
## <a name="remarks"></a><span data-ttu-id="aaca1-132">Примечания</span><span class="sxs-lookup"><span data-stu-id="aaca1-132">Remarks</span></span>

<span data-ttu-id="aaca1-133">Схема, описывающая этот элемент, расположена в виртуальном каталоге EWS на компьютере с MicrosoftExchange Server 2007 и установленной ролью сервера клиентского доступа.</span><span class="sxs-lookup"><span data-stu-id="aaca1-133">The schema that describes this element is located in the EWS virtual directory of the computer that is running MicrosoftExchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="example"></a><span data-ttu-id="aaca1-134">Пример</span><span class="sxs-lookup"><span data-stu-id="aaca1-134">Example</span></span>

<span data-ttu-id="aaca1-135">В следующем примере запроса SetUserOofSettings задается для Уфстате значение **Enabled**, устанавливается длительность бездействия в течение 10 дней, а также задаются внутренние и внешние сообщения об отсутствии на работе.</span><span class="sxs-lookup"><span data-stu-id="aaca1-135">The following example of a SetUserOofSettings request sets the OoFState to **Enabled**, sets the duration of OOF for 10 days, and sets the internal and external OOF messages.</span></span>
  
```xml
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

## <a name="element-information"></a><span data-ttu-id="aaca1-136">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="aaca1-136">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="aaca1-137">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="aaca1-137">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="aaca1-138">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="aaca1-138">Schema Name</span></span>  <br/> |<span data-ttu-id="aaca1-139">схема сообщений</span><span class="sxs-lookup"><span data-stu-id="aaca1-139">messages schema</span></span>  <br/> |
|<span data-ttu-id="aaca1-140">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="aaca1-140">Validation File</span></span>  <br/> |<span data-ttu-id="aaca1-141">Messages. xsd</span><span class="sxs-lookup"><span data-stu-id="aaca1-141">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="aaca1-142">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="aaca1-142">Can be Empty</span></span>  <br/> |<span data-ttu-id="aaca1-143">False</span><span class="sxs-lookup"><span data-stu-id="aaca1-143">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="aaca1-144">См. также</span><span class="sxs-lookup"><span data-stu-id="aaca1-144">See also</span></span>

- [<span data-ttu-id="aaca1-145">Операция SetUserOofSettings</span><span class="sxs-lookup"><span data-stu-id="aaca1-145">SetUserOofSettings operation</span></span>](setuseroofsettings-operation.md)

