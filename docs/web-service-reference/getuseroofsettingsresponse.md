---
title: жетусеруфсеттингсреспонсе
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- GetUserOofSettingsResponse
api_type:
- schema
ms.assetid: 011cb38b-da3c-4b1b-8836-a6b212b511f6
description: Элемент Жетусеруфсеттингсреспонсе содержит ответное сообщение и параметры отсутствия на работе (отсутствие на работе) для пользователя.
ms.openlocfilehash: f7f28c67fd36630ffb5294ab35c0fef2f467ba22
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/03/2020
ms.locfileid: "44457818"
---
# <a name="getuseroofsettingsresponse"></a><span data-ttu-id="e079f-103">жетусеруфсеттингсреспонсе</span><span class="sxs-lookup"><span data-stu-id="e079f-103">GetUserOofSettingsResponse</span></span>

<span data-ttu-id="e079f-104">Элемент **жетусеруфсеттингсреспонсе** содержит ответное сообщение и параметры отсутствия на работе (отсутствие на работе) для пользователя.</span><span class="sxs-lookup"><span data-stu-id="e079f-104">The **GetUserOofSettingsResponse** element contains the response message and the Out of Office (OOF) settings for a user.</span></span> 
  
```xml
<GetUserOofSettingsResponse>
   <ResponseMessage>...</ResponseMessage>
   <OofSettings>...</OofSettings>
   <AllowExternalOof>...</AllowExternalOof>
</GetUserOofSettingsResponse>
```

 <span data-ttu-id="e079f-105">**жетусеруфсеттингсреспонсе**</span><span class="sxs-lookup"><span data-stu-id="e079f-105">**GetUserOofSettingsResponse**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="e079f-106">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="e079f-106">Attributes and elements</span></span>

<span data-ttu-id="e079f-107">В следующих разделах описываются атрибуты, дочерние и родительские элементы.</span><span class="sxs-lookup"><span data-stu-id="e079f-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="e079f-108">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="e079f-108">Attributes</span></span>

<span data-ttu-id="e079f-109">Отсутствуют.</span><span class="sxs-lookup"><span data-stu-id="e079f-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="e079f-110">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="e079f-110">Child elements</span></span>

|<span data-ttu-id="e079f-111">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="e079f-111">**Element**</span></span>|<span data-ttu-id="e079f-112">**Описание**</span><span class="sxs-lookup"><span data-stu-id="e079f-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="e079f-113">респонсемессаже</span><span class="sxs-lookup"><span data-stu-id="e079f-113">ResponseMessage</span></span>](responsemessage.md) <br/> |<span data-ttu-id="e079f-114">Предоставляет описательные сведения о состоянии отклика.</span><span class="sxs-lookup"><span data-stu-id="e079f-114">Provides descriptive information about the response status.</span></span>  <br/> |
|[<span data-ttu-id="e079f-115">уфсеттингс</span><span class="sxs-lookup"><span data-stu-id="e079f-115">OofSettings</span></span>](oofsettings.md) <br/> |<span data-ttu-id="e079f-116">Содержит параметры отсутствия на работе.</span><span class="sxs-lookup"><span data-stu-id="e079f-116">Contains the OOF settings.</span></span>  <br/> |
|[<span data-ttu-id="e079f-117">алловекстерналуф</span><span class="sxs-lookup"><span data-stu-id="e079f-117">AllowExternalOof</span></span>](allowexternaloof.md) <br/> |<span data-ttu-id="e079f-118">Содержит значение, указывающее, кому отправляются внешние сообщения об отсутствии на работе.</span><span class="sxs-lookup"><span data-stu-id="e079f-118">Contains a value that identifies to whom external OOF messages are sent.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="e079f-119">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="e079f-119">Parent elements</span></span>

<span data-ttu-id="e079f-120">Нет.</span><span class="sxs-lookup"><span data-stu-id="e079f-120">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="e079f-121">Примечания</span><span class="sxs-lookup"><span data-stu-id="e079f-121">Remarks</span></span>

<span data-ttu-id="e079f-122">Схема, описывающая этот элемент, расположена в виртуальном каталоге EWS на компьютере с MicrosoftExchange Server 2007 и установленной ролью сервера клиентского доступа.</span><span class="sxs-lookup"><span data-stu-id="e079f-122">The schema that describes this element is located in the EWS virtual directory of the computer that is running MicrosoftExchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="e079f-123">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="e079f-123">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="e079f-124">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="e079f-124">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="e079f-125">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="e079f-125">Schema Name</span></span>  <br/> |<span data-ttu-id="e079f-126">Схема Messages</span><span class="sxs-lookup"><span data-stu-id="e079f-126">Messages schema</span></span>  <br/> |
|<span data-ttu-id="e079f-127">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="e079f-127">Validation File</span></span>  <br/> |<span data-ttu-id="e079f-128">Messages. xsd</span><span class="sxs-lookup"><span data-stu-id="e079f-128">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="e079f-129">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="e079f-129">Can be Empty</span></span>  <br/> |<span data-ttu-id="e079f-130">False</span><span class="sxs-lookup"><span data-stu-id="e079f-130">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="e079f-131">См. также</span><span class="sxs-lookup"><span data-stu-id="e079f-131">See also</span></span>



[<span data-ttu-id="e079f-132">Операция GetUserOofSettings</span><span class="sxs-lookup"><span data-stu-id="e079f-132">GetUserOofSettings operation</span></span>](getuseroofsettings-operation.md)
  
[<span data-ttu-id="e079f-133">Операция SetUserOofSettings</span><span class="sxs-lookup"><span data-stu-id="e079f-133">SetUserOofSettings operation</span></span>](setuseroofsettings-operation.md)

