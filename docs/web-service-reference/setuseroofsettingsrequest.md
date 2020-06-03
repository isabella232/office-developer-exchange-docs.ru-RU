---
title: сетусеруфсеттингсрекуест
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
description: Элемент Сетусеруфсеттингсрекуест содержит аргументы, используемые для задания параметров отсутствия на работе пользователя в почтовом ящике (отсутствие на работе).
ms.openlocfilehash: 10edc9809fd72f80c316de1c6688eaedec4f93df
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/03/2020
ms.locfileid: "44466152"
---
# <a name="setuseroofsettingsrequest"></a><span data-ttu-id="e9fdb-103">сетусеруфсеттингсрекуест</span><span class="sxs-lookup"><span data-stu-id="e9fdb-103">SetUserOofSettingsRequest</span></span>

<span data-ttu-id="e9fdb-104">Элемент **сетусеруфсеттингсрекуест** содержит аргументы, используемые для задания параметров отсутствия на работе пользователя в почтовом ящике (отсутствие на работе).</span><span class="sxs-lookup"><span data-stu-id="e9fdb-104">The **SetUserOofSettingsRequest** element contains the arguments used to set a mailbox user's Out of Office (OOF) settings.</span></span> 
  
```xml
<SetUserOofSettingsRequest>
   <Mailbox>...</Mailbox>
   <UserOofSettings>...</UserOofSettings>
<SetUserOofSettingsRequest>
```

 <span data-ttu-id="e9fdb-105">**сетусеруфсеттингсрекуест**</span><span class="sxs-lookup"><span data-stu-id="e9fdb-105">**SetUserOofSettingsRequest**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="e9fdb-106">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="e9fdb-106">Attributes and elements</span></span>

<span data-ttu-id="e9fdb-107">В следующих разделах описываются атрибуты, дочерние и родительские элементы.</span><span class="sxs-lookup"><span data-stu-id="e9fdb-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="e9fdb-108">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="e9fdb-108">Attributes</span></span>

<span data-ttu-id="e9fdb-109">Отсутствуют.</span><span class="sxs-lookup"><span data-stu-id="e9fdb-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="e9fdb-110">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="e9fdb-110">Child elements</span></span>

|<span data-ttu-id="e9fdb-111">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="e9fdb-111">**Element**</span></span>|<span data-ttu-id="e9fdb-112">**Описание**</span><span class="sxs-lookup"><span data-stu-id="e9fdb-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="e9fdb-113">Mailbox (доступность)</span><span class="sxs-lookup"><span data-stu-id="e9fdb-113">Mailbox (Availability)</span></span>](mailbox-availability.md) <br/> |<span data-ttu-id="e9fdb-114">Определяет пользователя почтового ящика для запроса SetUserOofSettings или GetUserOofSettings.</span><span class="sxs-lookup"><span data-stu-id="e9fdb-114">Identifies the mailbox user for a SetUserOofSettings or GetUserOofSettings request.</span></span>  <br/> |
|[<span data-ttu-id="e9fdb-115">усеруфсеттингс</span><span class="sxs-lookup"><span data-stu-id="e9fdb-115">UserOofSettings</span></span>](useroofsettings.md) <br/> |<span data-ttu-id="e9fdb-116">Задает параметры отсутствия на работе.</span><span class="sxs-lookup"><span data-stu-id="e9fdb-116">Specifies the OOF settings.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="e9fdb-117">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="e9fdb-117">Parent elements</span></span>

<span data-ttu-id="e9fdb-118">Нет.</span><span class="sxs-lookup"><span data-stu-id="e9fdb-118">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="e9fdb-119">Примечания</span><span class="sxs-lookup"><span data-stu-id="e9fdb-119">Remarks</span></span>

<span data-ttu-id="e9fdb-120">Схема, описывающая этот элемент, расположена в виртуальном каталоге EWS на компьютере с MicrosoftExchange Server 2007 и установленной ролью сервера клиентского доступа.</span><span class="sxs-lookup"><span data-stu-id="e9fdb-120">The schema that describes this element is located in the EWS virtual directory of the computer that is running MicrosoftExchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="example"></a><span data-ttu-id="e9fdb-121">Пример</span><span class="sxs-lookup"><span data-stu-id="e9fdb-121">Example</span></span>

<span data-ttu-id="e9fdb-122">В следующем примере запроса SetUserOofSettings задается значение параметра "отсутствие на работе" в десять дней.</span><span class="sxs-lookup"><span data-stu-id="e9fdb-122">The following example of a SetUserOofSettings request sets an OOF setting for ten days.</span></span>
  
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

## <a name="element-information"></a><span data-ttu-id="e9fdb-123">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="e9fdb-123">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="e9fdb-124">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="e9fdb-124">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="e9fdb-125">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="e9fdb-125">Schema Name</span></span>  <br/> |<span data-ttu-id="e9fdb-126">Схема Messages</span><span class="sxs-lookup"><span data-stu-id="e9fdb-126">Messages schema</span></span>  <br/> |
|<span data-ttu-id="e9fdb-127">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="e9fdb-127">Validation File</span></span>  <br/> |<span data-ttu-id="e9fdb-128">Messages. xsd</span><span class="sxs-lookup"><span data-stu-id="e9fdb-128">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="e9fdb-129">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="e9fdb-129">Can be Empty</span></span>  <br/> |<span data-ttu-id="e9fdb-130">False</span><span class="sxs-lookup"><span data-stu-id="e9fdb-130">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="e9fdb-131">См. также</span><span class="sxs-lookup"><span data-stu-id="e9fdb-131">See also</span></span>



[<span data-ttu-id="e9fdb-132">Операция SetUserOofSettings</span><span class="sxs-lookup"><span data-stu-id="e9fdb-132">SetUserOofSettings operation</span></span>](setuseroofsettings-operation.md)

