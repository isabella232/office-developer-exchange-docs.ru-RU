---
title: GetInboxRules
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- GetInboxRules
api_type:
- schema
ms.assetid: 7a54992d-03a6-4afc-a2e4-dcdc9ce54194
description: Элемент GetInboxRules определяет запрос на получение правил папкиВходящиепочтового ящика в хранилище сервера.
ms.openlocfilehash: 890592fd3f87fc5592a618a2febf28e4daf0dbe4
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/03/2020
ms.locfileid: "44457930"
---
# <a name="getinboxrules"></a><span data-ttu-id="46847-103">GetInboxRules</span><span class="sxs-lookup"><span data-stu-id="46847-103">GetInboxRules</span></span>

<span data-ttu-id="46847-104">Информация, содержащаяся в этом документе, может относиться к функциям и продуктам предварительной версии и может претерпеть значительные изменения до окончательного коммерческого выпуска. Настоящий документ предоставляется "как есть" и служит только для информационных целей. Корпорация Майкрософт не предоставляет никаких гарантий, явных или подразумеваемых, в связи с этим документом Элемент **GetInboxRules** определяет запрос на получение правил папки "Входящие" почтового ящика в хранилище сервера.</span><span class="sxs-lookup"><span data-stu-id="46847-104">The **GetInboxRules** element defines a request to get the Inbox rules on a mailbox in the server store.</span></span> 
  
```XML
<GetInboxRules>
   <MailboxSmtpAddress/>
</GetInboxRules>
```

 <span data-ttu-id="46847-105">**жетинбоксрулесрекуесттипе**</span><span class="sxs-lookup"><span data-stu-id="46847-105">**GetInboxRulesRequestType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="46847-106">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="46847-106">Attributes and elements</span></span>

<span data-ttu-id="46847-107">В следующих разделах описываются атрибуты, дочерние и родительские элементы.</span><span class="sxs-lookup"><span data-stu-id="46847-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="46847-108">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="46847-108">Attributes</span></span>

<span data-ttu-id="46847-109">Отсутствуют.</span><span class="sxs-lookup"><span data-stu-id="46847-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="46847-110">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="46847-110">Child elements</span></span>

|<span data-ttu-id="46847-111">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="46847-111">**Element**</span></span>|<span data-ttu-id="46847-112">**Описание**</span><span class="sxs-lookup"><span data-stu-id="46847-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="46847-113">маилбокссмтпаддресс</span><span class="sxs-lookup"><span data-stu-id="46847-113">MailboxSmtpAddress</span></span>](mailboxsmtpaddress.md) <br/> |<span data-ttu-id="46847-114">Представляет SMTP-адрес пользователя, чьи правила папки "Входящие", нужно вернуть.</span><span class="sxs-lookup"><span data-stu-id="46847-114">Represents the SMTP address of the user whose Inbox rules are to be retrieved.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="46847-115">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="46847-115">Parent elements</span></span>

<span data-ttu-id="46847-116">Нет.</span><span class="sxs-lookup"><span data-stu-id="46847-116">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="46847-117">Примечания</span><span class="sxs-lookup"><span data-stu-id="46847-117">Remarks</span></span>

<span data-ttu-id="46847-118">Схема, описывающая этот элемент, находится в виртуальном каталоге IIS, в котором размещены веб-службы Exchange.</span><span class="sxs-lookup"><span data-stu-id="46847-118">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="46847-119">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="46847-119">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="46847-120">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="46847-120">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="46847-121">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="46847-121">Schema Name</span></span>  <br/> |<span data-ttu-id="46847-122">Схема Messages</span><span class="sxs-lookup"><span data-stu-id="46847-122">Messages schema</span></span>  <br/> |
|<span data-ttu-id="46847-123">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="46847-123">Validation File</span></span>  <br/> |<span data-ttu-id="46847-124">Messages. xsd</span><span class="sxs-lookup"><span data-stu-id="46847-124">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="46847-125">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="46847-125">Can be Empty</span></span>  <br/> |<span data-ttu-id="46847-126">True</span><span class="sxs-lookup"><span data-stu-id="46847-126">True</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="46847-127">См. также</span><span class="sxs-lookup"><span data-stu-id="46847-127">See also</span></span>



[<span data-ttu-id="46847-128">Операция GetInboxRules</span><span class="sxs-lookup"><span data-stu-id="46847-128">GetInboxRules operation</span></span>](getinboxrules-operation.md)

