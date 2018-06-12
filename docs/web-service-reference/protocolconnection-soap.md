---
title: ProtocolConnection (SOAP)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
localization_priority: Normal
api_type:
- schema
ms.assetid: 6eef2188-6194-48f1-ad7e-46104aecdf56
description: Элемент ProtocolConnection представляет подключение к протокола сервера веб-клиент.
ms.openlocfilehash: 8b5396821cd959e41d24fcf7a94c519f9c634a1f
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/11/2018
ms.locfileid: "19834915"
---
# <a name="protocolconnection-soap"></a><span data-ttu-id="b3814-103">ProtocolConnection (SOAP)</span><span class="sxs-lookup"><span data-stu-id="b3814-103">ProtocolConnection (SOAP)</span></span>

<span data-ttu-id="b3814-104">Элемент **ProtocolConnection** представляет подключение к протокола сервера веб-клиент.</span><span class="sxs-lookup"><span data-stu-id="b3814-104">The **ProtocolConnection** element represents the protocol connection of the server Web client.</span></span> 
  
```XML
<ProtocolConnection>
   <Hostname/>
   <Port/>
   <EncryptionMethod/>
</ProtocolConnection>
```

 <span data-ttu-id="b3814-105">**ProtocolConnection**</span><span class="sxs-lookup"><span data-stu-id="b3814-105">**ProtocolConnection**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="b3814-106">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="b3814-106">Attributes and elements</span></span>

<span data-ttu-id="b3814-107">В разделах ниже приводится описание атрибутов, дочерних и родительских элементов.</span><span class="sxs-lookup"><span data-stu-id="b3814-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="b3814-108">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="b3814-108">Attributes</span></span>

<span data-ttu-id="b3814-109">Нет.</span><span class="sxs-lookup"><span data-stu-id="b3814-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="b3814-110">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="b3814-110">Child elements</span></span>

|<span data-ttu-id="b3814-111">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="b3814-111">**Element**</span></span>|<span data-ttu-id="b3814-112">**Описание**</span><span class="sxs-lookup"><span data-stu-id="b3814-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="b3814-113">Имя узла (SOAP)</span><span class="sxs-lookup"><span data-stu-id="b3814-113">Hostname (SOAP)</span></span>](hostname-soap.md) <br/> |<span data-ttu-id="b3814-114">Представляет часть полное имя компьютера, имя узла.</span><span class="sxs-lookup"><span data-stu-id="b3814-114">Represents the host name portion of the full computer name of the computer.</span></span>  <br/> |
|[<span data-ttu-id="b3814-115">Порт (SOAP)</span><span class="sxs-lookup"><span data-stu-id="b3814-115">Port (SOAP)</span></span>](port-soap.md) <br/> |<span data-ttu-id="b3814-116">Представляет номер порта для использования протокола.</span><span class="sxs-lookup"><span data-stu-id="b3814-116">Represents the port number to use for the protocol.</span></span>  <br/> |
|[<span data-ttu-id="b3814-117">EncryptionMethod (SOAP)</span><span class="sxs-lookup"><span data-stu-id="b3814-117">EncryptionMethod (SOAP)</span></span>](encryptionmethod-soap.md) <br/> |<span data-ttu-id="b3814-118">Представляет метод шифрования, который используется для протоколов POP, IMAP и SMTP.</span><span class="sxs-lookup"><span data-stu-id="b3814-118">Represents the cryptographic method that is used for the POP, IMAP, and SMTP protocols.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="b3814-119">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="b3814-119">Parent elements</span></span>

|<span data-ttu-id="b3814-120">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="b3814-120">**Element**</span></span>|<span data-ttu-id="b3814-121">**Описание**</span><span class="sxs-lookup"><span data-stu-id="b3814-121">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="b3814-122">ProtocolConnections (SOAP)</span><span class="sxs-lookup"><span data-stu-id="b3814-122">ProtocolConnections (SOAP)</span></span>](protocolconnections-soap.md) <br/> |<span data-ttu-id="b3814-123">Содержит ноль или больше протокол подключения.</span><span class="sxs-lookup"><span data-stu-id="b3814-123">Contains zero or more protocol connections.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="b3814-124">Текстовое значение</span><span class="sxs-lookup"><span data-stu-id="b3814-124">Text value</span></span>

<span data-ttu-id="b3814-125">Нет.</span><span class="sxs-lookup"><span data-stu-id="b3814-125">None.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="b3814-126">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="b3814-126">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="b3814-127">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="b3814-127">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/2010/Autodiscover  <br/> |
|<span data-ttu-id="b3814-128">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="b3814-128">Schema Name</span></span>  <br/> |<span data-ttu-id="b3814-129">Схема службы автообнаружения</span><span class="sxs-lookup"><span data-stu-id="b3814-129">Autodiscover schema</span></span>  <br/> |
|<span data-ttu-id="b3814-130">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="b3814-130">Validation File</span></span>  <br/> |<span data-ttu-id="b3814-131">Messages.xsd</span><span class="sxs-lookup"><span data-stu-id="b3814-131">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="b3814-132">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="b3814-132">Can be Empty</span></span>  <br/> |<span data-ttu-id="b3814-133">True</span><span class="sxs-lookup"><span data-stu-id="b3814-133">True</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="b3814-134">См. также</span><span class="sxs-lookup"><span data-stu-id="b3814-134">See also</span></span>



[<span data-ttu-id="b3814-135">ProtocolConnectionCollectionSetting (SOAP)</span><span class="sxs-lookup"><span data-stu-id="b3814-135">ProtocolConnectionCollectionSetting (SOAP)</span></span>](protocolconnectioncollectionsetting-soap.md)

