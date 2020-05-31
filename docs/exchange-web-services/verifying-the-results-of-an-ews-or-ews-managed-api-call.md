---
title: Проверка результатов вызова EWS или EWS управляемых API
manager: sethgros
ms.date: 11/16/2014
ms.audience: Developer
localization_priority: Normal
ms.assetid: 78a1741c-1bbe-4cb4-9331-9d6d3171fc11
description: Узнайте, как проверить результаты вызовов управляемого API EWS или EWS.
ms.openlocfilehash: 077dd923710a1a7f5cad4c822cbbd58ab3603661
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/25/2018
ms.locfileid: "19761251"
---
# <a name="verifying-the-results-of-an-ews-or-ews-managed-api-call"></a><span data-ttu-id="a6a2e-103">Проверка результатов вызова EWS или EWS управляемых API</span><span class="sxs-lookup"><span data-stu-id="a6a2e-103">Verifying the results of an EWS or EWS Managed API call</span></span>

<span data-ttu-id="a6a2e-104">Узнайте, как проверить результаты вызовов управляемого API EWS или EWS.</span><span class="sxs-lookup"><span data-stu-id="a6a2e-104">Learn how to verify the results of your EWS or EWS Managed API calls.</span></span>
  
<span data-ttu-id="a6a2e-105">Если что-то не работает должным образом, вы можете узнать, что происходит с помощью проверки SOAP-запросов, отправляемых приложением по сети, и ответов, отправляемых сервером обратно.</span><span class="sxs-lookup"><span data-stu-id="a6a2e-105">When things aren't working correctly, it helps to see what's going on by examining the SOAP requests that your application is sending over the network and the responses that the server is sending back.</span></span> <span data-ttu-id="a6a2e-106">В статье [Tools and Resources for устранение неполадок приложений EWS](tools-and-resources-for-troubleshooting-ews-applications-for-exchange.md) содержатся ссылки на средства, помогающие записывать и просматривать эти SOAP запросы.</span><span class="sxs-lookup"><span data-stu-id="a6a2e-106">The [tools and resources for troubleshooting EWS applications](tools-and-resources-for-troubleshooting-ews-applications-for-exchange.md) article includes links to tools to help capture and view those SOAP requests.</span></span> <span data-ttu-id="a6a2e-107">После того как вы получите запросы и ответы, как убедиться, что отправленный на сервер запрос был обработан правильно?</span><span class="sxs-lookup"><span data-stu-id="a6a2e-107">After you've got the requests and the responses, how do you verify that the request you sent to the server was processed correctly?</span></span> <span data-ttu-id="a6a2e-108">Прочтите статью, чтобы узнать.</span><span class="sxs-lookup"><span data-stu-id="a6a2e-108">Read on to find out.</span></span> 
  
<span data-ttu-id="a6a2e-109">Если вы отправляете запросы EWS, вы собираетесь начать проверку, проверив атрибут **респонсекласс** для каждого ответного сообщения в ответе.</span><span class="sxs-lookup"><span data-stu-id="a6a2e-109">If you're sending EWS requests, you're going to start your verification by checking the **ResponseClass** attribute for each response message in the response.</span></span> <span data-ttu-id="a6a2e-110">С помощью которого вы узнаете, успешно ли завершена операция для каждого элемента.</span><span class="sxs-lookup"><span data-stu-id="a6a2e-110">That will tell you whether the operation completed successfully on each item.</span></span> 
  
<span data-ttu-id="a6a2e-111">В зависимости от объекта, который вызывается методом, если вы используете управляемый API EWS для отправки запросов, можно выполнить некоторую проверку с помощью объектов Response.</span><span class="sxs-lookup"><span data-stu-id="a6a2e-111">Depending on the object that your method is calling, if you're using the EWS Managed API to send requests, you can do some verification using the response objects.</span></span> <span data-ttu-id="a6a2e-112">Но так как ответ SOAP содержит надмножество элементов, включенных в объекты ответа управляемых API EWS, может также потребоваться взглянуть на SOAP-ответ.</span><span class="sxs-lookup"><span data-stu-id="a6a2e-112">But because the SOAP response contains a superset of what's included in the EWS Managed API response objects, you might want to look at the SOAP response as well.</span></span> <span data-ttu-id="a6a2e-113">Так как ответ SOAP часто содержит больше сведений, чем объекты ответа управляемого API EWS, запустите проверку с ответом SOAP.</span><span class="sxs-lookup"><span data-stu-id="a6a2e-113">Because the SOAP response can often contain more information than the EWS Managed API response objects, start your verification with the SOAP response.</span></span>
  
## <a name="verifying-the-results-of-a-soap-response"></a><span data-ttu-id="a6a2e-114">Проверка результатов ответа SOAP</span><span class="sxs-lookup"><span data-stu-id="a6a2e-114">Verifying the results of a SOAP response</span></span>
<span data-ttu-id="a6a2e-115"><a name="bk_verifysoap"> </a></span><span class="sxs-lookup"><span data-stu-id="a6a2e-115"><a name="bk_verifysoap"> </a></span></span>

<span data-ttu-id="a6a2e-116">При получении ответа SOAP первым делом рассмотрим атрибут **респонсекласс** .</span><span class="sxs-lookup"><span data-stu-id="a6a2e-116">When you receive a SOAP response, the first thing to look at is the **ResponseClass** attribute.</span></span> <span data-ttu-id="a6a2e-117">Этот атрибут включается в каждый экземпляр **респонсемессажетипе** в элементе [респонсемессажес](http://msdn.microsoft.com/library/2071bed8-ea66-4627-aa4f-a1d9a025cf3d%28Office.15%29.aspx) , как показано в следующем примере.</span><span class="sxs-lookup"><span data-stu-id="a6a2e-117">This attribute is included in each **ResponseMessageType** instance in the [ResponseMessages](http://msdn.microsoft.com/library/2071bed8-ea66-4627-aa4f-a1d9a025cf3d%28Office.15%29.aspx) element, as shown in the following example.</span></span> 
  
```XML
<s:Body>
      <m:GetItemResponse xmlns:m="http://schemas.microsoft.com/exchange/services/2006/messages"
                         xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types">
        <m:ResponseMessages>
          <m:GetItemResponseMessage ResponseClass="Success">
          …
```

<span data-ttu-id="a6a2e-118">Так как ответ SOAP может содержать несколько ответных сообщений в едином SOAP-ответе, важно проверять каждое ответное сообщение по отдельности.</span><span class="sxs-lookup"><span data-stu-id="a6a2e-118">Because a SOAP response might contain multiple response messages in a single SOAP response, it's important to check each response message individually.</span></span>
  
<span data-ttu-id="a6a2e-119">Если вы работаете с операцией, которая включает **респонсекласс** в ответ операции, как показано ниже, возможно, вы можете просмотреть только **респонсекласс** операции.</span><span class="sxs-lookup"><span data-stu-id="a6a2e-119">If you're working with an operation that includes a **ResponseClass** as part of the operation response, like the following, you might be tempted to only check the **ResponseClass** of the operation.</span></span> 
  
```XML
<soap:Body>
  <m:AddDelegateResponse xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types"
                         ResponseClass="Success"
                         xmlns:m="http://schemas.microsoft.com/exchange/services/2006/messages">
  …

```

<span data-ttu-id="a6a2e-120">Однако состояние операции отражает только форму отклика верхнего уровня и не отражает состояние всех индивидуальных ответов на сообщения.</span><span class="sxs-lookup"><span data-stu-id="a6a2e-120">However, the operation status only reflects the shape of the top-level response and does not reflect the status of all the individual message responses.</span></span> <span data-ttu-id="a6a2e-121">В следующем примере операция [аддделегатереспонсе](http://msdn.microsoft.com/library/d7e6bebb-5dbf-43c1-aacf-4b3ca6a7c429%28Office.15%29.aspx) имеет **респонсекласс** **успешного**выполнения, но базовый элемент [делегатеусерреспонсемессажетипе](http://msdn.microsoft.com/library/3dc9552c-1e2d-40ac-a137-827883c2bb88%28Office.15%29.aspx) имеет значение **ошибки** **респонсекласс** .</span><span class="sxs-lookup"><span data-stu-id="a6a2e-121">In the following example, the [AddDelegateResponse](http://msdn.microsoft.com/library/d7e6bebb-5dbf-43c1-aacf-4b3ca6a7c429%28Office.15%29.aspx) operation has a **ResponseClass** of **Success**, but the underlying [DelegateUserResponseMessageType](http://msdn.microsoft.com/library/3dc9552c-1e2d-40ac-a137-827883c2bb88%28Office.15%29.aspx) element has a **ResponseClass** value of **Error**.</span></span>
  
```XML
<soap:Body>
  <m:AddDelegateResponse xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types"
                         ResponseClass="Success"
                         xmlns:m="http://schemas.microsoft.com/exchange/services/2006/messages">
    <m:ResponseCode>NoError</m:ResponseCode>
    <m:ResponseMessages>
      <m:DelegateUserResponseMessageType ResponseClass="Error">
        <m:MessageText>The user is already a delegate for the mailbox.</m:MessageText>
        <m:ResponseCode>ErrorDelegateAlreadyExists</m:ResponseCode>
        <m:DescriptiveLinkKey>0</m:DescriptiveLinkKey>
      </m:DelegateUserResponseMessageType>
    </m:ResponseMessages>
  </m:AddDelegateResponse>
</soap:Body>
```

<span data-ttu-id="a6a2e-122">Таким образом, для ответов SOAP EWS вы не можете полагаться на **респонсекласс** операции, чтобы определить, обнаружила ли операция ошибки при обработке элементов, необходимо взглянуть на **респонсекласс** каждого ответного сообщения.</span><span class="sxs-lookup"><span data-stu-id="a6a2e-122">So for SOAP EWS responses, you can't rely on the **ResponseClass** of the operation - you have to look at the **ResponseClass** of each response message to determine whether the operation encountered any errors processing the items.</span></span> 
  
### <a name="verifying-success"></a><span data-ttu-id="a6a2e-123">Проверка успешности</span><span class="sxs-lookup"><span data-stu-id="a6a2e-123">Verifying success</span></span>

<span data-ttu-id="a6a2e-124">Если каждому атрибуту **респонсекласс** для каждого атрибута **респонсемессаже** присвоено значение **Success**, операция успешно завершена для всех элементов, и вы можете перейти к следующей задаче.</span><span class="sxs-lookup"><span data-stu-id="a6a2e-124">If each **ResponseClass** attribute for each **ResponseMessage** attribute is set to **Success**, the operation completed successfully on all the items, and you can move on to your next task.</span></span>
  
<span data-ttu-id="a6a2e-125">В следующем примере показан успешный ответ на запрос операции [GetItem](http://msdn.microsoft.com/library/e8492e3b-1c8d-4b14-8070-9530f8306edd%28Office.15%29.aspx) для получения одного элемента.</span><span class="sxs-lookup"><span data-stu-id="a6a2e-125">The following example shows a successful response to a [GetItem](http://msdn.microsoft.com/library/e8492e3b-1c8d-4b14-8070-9530f8306edd%28Office.15%29.aspx) operation request to retrieve a single item.</span></span> <span data-ttu-id="a6a2e-126">Обратите внимание, что если для **респонсекласс** задано значение **Success**, связанному [респонсекодеу](http://msdn.microsoft.com/library/4b84d670-74c9-4d6d-84e7-f0a9f76f0d93%28Office.15%29.aspx) всегда присваивается значение " **Ошибка**".</span><span class="sxs-lookup"><span data-stu-id="a6a2e-126">Note that when the **ResponseClass** is set to **Success**, the associated [ResponseCode](http://msdn.microsoft.com/library/4b84d670-74c9-4d6d-84e7-f0a9f76f0d93%28Office.15%29.aspx) is always set to **NoError**.</span></span>
  
```XML
<s:Body xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" 
             xmlns:xsd="http://www.w3.org/2001/XMLSchema">
      <m:GetItemResponse xmlns:m="http://schemas.microsoft.com/exchange/services/2006/messages"
                         xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types">
        <m:ResponseMessages>
          <m:GetItemResponseMessage ResponseClass="Success">
            <m:ResponseCode>NoError</m:ResponseCode>
            <m:Items>
              <t:Message>
                <t:ItemId Id="Er5bAAA=" 
                          ChangeKey="CQAAABYAAAD32nSTjepyT63rYH17n9THAAAhE0/M" />
                <t:Subject>Dinner Party</t:Subject>
              </t:Message>
            </m:Items>
          </m:GetItemResponseMessage>
        </m:ResponseMessages>
      </m:GetItemResponse>
    </s:Body>
```

<span data-ttu-id="a6a2e-127">Ниже приведен успешный ответ на запрос операции **GetItem** для получения нескольких элементов.</span><span class="sxs-lookup"><span data-stu-id="a6a2e-127">The following is a successful response to a **GetItem** operation request to retrieve multiple items.</span></span> <span data-ttu-id="a6a2e-128">Каждый из элементов [жетитемреспонсемессаже](http://msdn.microsoft.com/library/cc583723-54d1-4a17-8c1f-6586f70fdefd%28Office.15%29.aspx) имеет **респонсекласс** **об успехе**.</span><span class="sxs-lookup"><span data-stu-id="a6a2e-128">Each of the [GetItemResponseMessage](http://msdn.microsoft.com/library/cc583723-54d1-4a17-8c1f-6586f70fdefd%28Office.15%29.aspx) elements has a **ResponseClass** of **Success**.</span></span>
  
```XML
<s:Body xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance"
             xmlns:xsd="http://www.w3.org/2001/XMLSchema">
  <m:GetItemResponse xmlns:m="http://schemas.microsoft.com/exchange/services/2006/messages"
                     xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types">
    <m:ResponseMessages>
      <m:GetItemResponseMessage ResponseClass="Success">
        <m:ResponseCode>NoError</m:ResponseCode>
        <m:Items>
          <t:Message>
            <t:ItemId Id="Er5bAAA=" 
                      ChangeKey="CQAAABYAAAD32nSTjepyT63rYH17n9THAAAhE0/M" /
            <t:Subject>Dinner Party</t:Subject>
          </t:Message>
        </m:Items>
      </m:GetItemResponseMessage>
      <m:GetItemResponseMessage ResponseClass="Success">
        <m:ResponseCode>NoError</m:ResponseCode>
        <m:Items>
          <t:Message>
            <t:ItemId Id="3c66AAA="
                      ChangeKey="CQAAABYAAAD32nSTjepyT63rYH17n9THAAAc3kqm" />
            <t:Subject>Company Soccer Team</t:Subject>
          </t:Message>
        </m:Items>
      </m:GetItemResponseMessage>
    </m:ResponseMessages>
  </m:GetItemResponse>
</s:Body>
```

### <a name="handling-errors-and-warnings"></a><span data-ttu-id="a6a2e-129">Обработка ошибок и предупреждений</span><span class="sxs-lookup"><span data-stu-id="a6a2e-129">Handling errors and warnings</span></span>

<span data-ttu-id="a6a2e-130">При получении ответа, если для атрибута **респонсекласс** задано значение **Error**, операция не была успешно завершена для одного или нескольких элементов.</span><span class="sxs-lookup"><span data-stu-id="a6a2e-130">When you receive a response and the **ResponseClass** attribute is set to **Error**, the operation did not complete successfully on one or more items.</span></span> <span data-ttu-id="a6a2e-131">Устраните ошибку и повторите запрос или часть запроса, в которой произошел сбой.</span><span class="sxs-lookup"><span data-stu-id="a6a2e-131">Correct the issue and retry your request, or the part of your request that failed.</span></span> <span data-ttu-id="a6a2e-132">Значение свойства **респонсекласс** , равное значению **warning** , возвращается только операцией [ResolveNames](http://msdn.microsoft.com/library/6b4eb4b3-9ad6-4804-a09f-7e20cfea4dbb%28Office.15%29.aspx) и указывает, что сущность не может быть сопоставлена с уникальным идентификатором.</span><span class="sxs-lookup"><span data-stu-id="a6a2e-132">A **ResponseClass** attribute value of **Warning** value is only returned by the [ResolveNames](http://msdn.microsoft.com/library/6b4eb4b3-9ad6-4804-a09f-7e20cfea4dbb%28Office.15%29.aspx) operation, and indicates that the entity could not be resolved to a unique identity.</span></span> <span data-ttu-id="a6a2e-133">Вы можете игнорировать его для всех других операций.</span><span class="sxs-lookup"><span data-stu-id="a6a2e-133">You can ignore it for all other operations.</span></span> 
  
<span data-ttu-id="a6a2e-134">В следующем ответе атрибут **респонсекласс** имеет значение **Error**.</span><span class="sxs-lookup"><span data-stu-id="a6a2e-134">In the following response, the **ResponseClass** attribute has a value of **Error**.</span></span>
  
```XML
<m:GetItemResponseMessage ResponseClass="Error">
  <m:MessageText>Property is not valid for this object type.</m:MessageText>
  <m:ResponseCode>ErrorInvalidPropertyRequest</m:ResponseCode>
  <m:DescriptiveLinkKey>0</m:DescriptiveLinkKey>
  <m:MessageXml>
    <t:FieldURI FieldURI="meeting:AssociatedCalendarItemId" />
  </m:MessageXml>
  <m:Items />
</m:GetItemResponseMessage>
```

<span data-ttu-id="a6a2e-135">В этом примере EWS предоставляет сведения для отладки неполадок.</span><span class="sxs-lookup"><span data-stu-id="a6a2e-135">In this example, EWS provides clues to debug the issue.</span></span> <span data-ttu-id="a6a2e-136">Если для атрибута **респонсекласс** задано значение **Error**, при необходимости в отклике включаются следующие дополнительные элементы:</span><span class="sxs-lookup"><span data-stu-id="a6a2e-136">When the **ResponseClass** attribute has a value of **Error**, the following additional elements are included in the response when applicable:</span></span>
  
- <span data-ttu-id="a6a2e-137">[Мессажетекст](http://msdn.microsoft.com/library/59a23bdc-0d9a-4942-8b3c-9cdb11db1ab1%28Office.15%29.aspx) — описание ошибки.</span><span class="sxs-lookup"><span data-stu-id="a6a2e-137">[MessageText](http://msdn.microsoft.com/library/59a23bdc-0d9a-4942-8b3c-9cdb11db1ab1%28Office.15%29.aspx) — Describes the error.</span></span> 
    
- <span data-ttu-id="a6a2e-138">[Респонсекоде](http://msdn.microsoft.com/library/4b84d670-74c9-4d6d-84e7-f0a9f76f0d93%28Office.15%29.aspx) — содержит код ошибки, который можно использовать для поиска дополнительных ресурсов по устранению неполадок.</span><span class="sxs-lookup"><span data-stu-id="a6a2e-138">[ResponseCode](http://msdn.microsoft.com/library/4b84d670-74c9-4d6d-84e7-f0a9f76f0d93%28Office.15%29.aspx) — Contains the error code, which can be used to find additional troubleshooting resources.</span></span> 
    
- <span data-ttu-id="a6a2e-139">[Мессажексмл](http://msdn.microsoft.com/library/bcaf9e35-d351-48f3-baad-f90c633cba8a%28Office.15%29.aspx) — определяет элементы, которые привели к ошибке.</span><span class="sxs-lookup"><span data-stu-id="a6a2e-139">[MessageXml](http://msdn.microsoft.com/library/bcaf9e35-d351-48f3-baad-f90c633cba8a%28Office.15%29.aspx) — Identifies the elements that caused the error.</span></span> 
    
- <span data-ttu-id="a6a2e-140">[Дескриптивелинккэй](http://msdn.microsoft.com/library/f7f36749-00f3-4915-b17c-e3caa0af6e67%28Office.15%29.aspx) — не используется.</span><span class="sxs-lookup"><span data-stu-id="a6a2e-140">[DescriptiveLinkKey](http://msdn.microsoft.com/library/f7f36749-00f3-4915-b17c-e3caa0af6e67%28Office.15%29.aspx) — Unused.</span></span> 
    
<span data-ttu-id="a6a2e-141">Сведения, приведенные в этих элементах, можно использовать для изучения возникшей проблемы.</span><span class="sxs-lookup"><span data-stu-id="a6a2e-141">You can use the information provided in these elements to investigate your issue.</span></span> <span data-ttu-id="a6a2e-142">В предыдущем примере **мессажетекст** указывает, что свойство не является допустимым для типа объекта.</span><span class="sxs-lookup"><span data-stu-id="a6a2e-142">In the previous example, the **MessageText** indicates that the property isn't valid for the object type.</span></span> <span data-ttu-id="a6a2e-143">В запросе было получено сообщение электронной почты, но в набор свойств включено свойство **ассоЦиатедкалендаритемид**, которое является допустимым только для элементов встречи.</span><span class="sxs-lookup"><span data-stu-id="a6a2e-143">The request was to get an email message, but the property set included the **AssociatedCalendarItemId**, which is only valid for appointment items.</span></span>
  
<span data-ttu-id="a6a2e-144">В следующем примере показана ошибка, полученная в составе пакетной операции для получения нескольких элементов электронной почты.</span><span class="sxs-lookup"><span data-stu-id="a6a2e-144">The following example shows an error that was received as part of a batched operation to get multiple email items.</span></span> <span data-ttu-id="a6a2e-145">Первый элемент был успешно получен, а для **респонсекласс** задано значение **Success**.</span><span class="sxs-lookup"><span data-stu-id="a6a2e-145">The first item was retrieved successfully and the **ResponseClass** is set to **Success**.</span></span> <span data-ttu-id="a6a2e-146">Не удалось найти второй элемент, а для параметра **респонсекласс** задано значение **Error**.</span><span class="sxs-lookup"><span data-stu-id="a6a2e-146">The second item could not be found, and the **ResponseClass** is set to **Error**.</span></span>
  
```XML
<m:GetItemResponse xmlns:m="http://schemas.microsoft.com/exchange/services/2006/messages"
                        xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types">
  <m:ResponseMessages>
    <m:GetItemResponseMessage ResponseClass="Success">
      <m:ResponseCode>NoError</m:ResponseCode>
      <m:Items>
        <t:Message>
          <t:ItemId Id="Er5cAAA="
                    ChangeKey="CQAAABYAAAD32nSTjepyT63rYH17n9THAAAhE0/O" />
          <t:Subject>Business plans</t:Subject>
        </t:Message>
      </m:Items>
    </m:GetItemResponseMessage>
    <m:GetItemResponseMessage ResponseClass="Error">
      <m:MessageText>The specified object was not found in the store.</m:MessageText>
      <m:ResponseCode>ErrorItemNotFound</m:ResponseCode>
      <m:DescriptiveLinkKey>0</m:DescriptiveLinkKey>
      <m:Items />
    </m:GetItemResponseMessage>
  </m:ResponseMessages>
</m:GetItemResponse>
```

<span data-ttu-id="a6a2e-147">Если один или несколько элементов в пакетном запросе не могут быть обработаны как запрошенные, возвращается ошибка для каждого элемента, для которого произошел сбой, а остальные элементы пакета обрабатываются должным образом.</span><span class="sxs-lookup"><span data-stu-id="a6a2e-147">When one or more items in a batched request can't be processed as requested, an error is returned for each item that failed, and the rest of the items in the batch are processed as expected.</span></span> <span data-ttu-id="a6a2e-148">Ошибки в пакетной обработке могут возникать, если элемент был удален, поэтому его невозможно отправить, извлечь или обновить, или если элемент перемещен в другую папку, и поэтому имеет новый идентификатор элемента.</span><span class="sxs-lookup"><span data-stu-id="a6a2e-148">Failures in batch processing can occur if the item was deleted, and therefore can't be sent, retrieved, or updated, or if the item moved to a different folder, and therefore has a new item ID.</span></span> <span data-ttu-id="a6a2e-149">Так как операция будет выполнена для некоторых элементов и не будет возвращать ошибку при невозможности обработать один или несколько элементов, важно проверить каждый атрибут **респонсекласс** , прежде чем переходить к следующей операции.</span><span class="sxs-lookup"><span data-stu-id="a6a2e-149">Because the operation will complete for some items and not return an error when one or more items can't be processed, it's important to check each **ResponseClass** attribute before you move on to your next operation.</span></span> 
  
<span data-ttu-id="a6a2e-150">Если сведения, предоставляемые элементами ответа, не помогают исправить запрос или не разблокируют вас, ознакомьтесь со статьей [дальнейшие действия](#bk_nextsteps).</span><span class="sxs-lookup"><span data-stu-id="a6a2e-150">If the information provided by the response elements doesn't help you correct your request or otherwise unblock you, see [Next steps](#bk_nextsteps).</span></span>
  
## <a name="verifying-the-results-of-an-ews-managed-api-method-call"></a><span data-ttu-id="a6a2e-151">Проверка результатов вызова метода управляемого API EWS</span><span class="sxs-lookup"><span data-stu-id="a6a2e-151">Verifying the results of an EWS Managed API method call</span></span>
<span data-ttu-id="a6a2e-152"><a name="bk_successful"> </a></span><span class="sxs-lookup"><span data-stu-id="a6a2e-152"><a name="bk_successful"> </a></span></span>

<span data-ttu-id="a6a2e-153">Если вы используете управляемый API EWS и вызываете метод для объекта [ExchangeService](http://msdn.microsoft.com/EN-US/library/microsoft.exchange.webservices.data.exchangeservice%28v=exchg.80%29.aspx) , ваш метод скорее всего вернет объект [сервицереспонсеколлектион](http://msdn.microsoft.com/EN-US/library/dd633715%28v=exchg.80%29.aspx) , который содержит коллекцию объектов [сервицереспонсе](http://msdn.microsoft.com/EN-US/library/microsoft.exchange.webservices.data.serviceresponse%28v=exchg.80%29.aspx) , или коллекцию объектов, производных от объектов **сервицереспонсе** .</span><span class="sxs-lookup"><span data-stu-id="a6a2e-153">If you're using the EWS Managed API and calling a method on an [ExchangeService](http://msdn.microsoft.com/EN-US/library/microsoft.exchange.webservices.data.exchangeservice%28v=exchg.80%29.aspx) object, your method will likely return a [ServiceResponseCollection](http://msdn.microsoft.com/EN-US/library/dd633715%28v=exchg.80%29.aspx) object, which contains a collection of [ServiceResponse](http://msdn.microsoft.com/EN-US/library/microsoft.exchange.webservices.data.serviceresponse%28v=exchg.80%29.aspx) objects, or a collection of objects derived from the **ServiceResponse** objects.</span></span> <span data-ttu-id="a6a2e-154">**Сервицереспонсеколлектион** и включенные объекты **сервицереспонсе** содержат сведения о результатах вызова метода, которые можно использовать для проверки результатов.</span><span class="sxs-lookup"><span data-stu-id="a6a2e-154">The **ServiceResponseCollection** and included **ServiceResponse** objects contain information about the result of the method call, which you can use to verify your results.</span></span> 
  
<span data-ttu-id="a6a2e-155">Если вы используете управляемый API EWS и вызываете метод для объекта [Item](http://msdn.microsoft.com/EN-US/library/microsoft.exchange.webservices.data.item%28v=exchg.80%29.aspx) или один из производных объектов, метод, скорее всего, не возвращает объект Response для проверки на успешное выполнение, но при этом создает [исключение](http://msdn.microsoft.com/EN-US/library/c18k6c59) , если метод не завершается успешно.</span><span class="sxs-lookup"><span data-stu-id="a6a2e-155">If you're using the EWS Managed API and calling a method on an [Item](http://msdn.microsoft.com/EN-US/library/microsoft.exchange.webservices.data.item%28v=exchg.80%29.aspx) object, or one of the derived objects, the method likely does not return a response object to check for success, but does throw an [Exception](http://msdn.microsoft.com/EN-US/library/c18k6c59) if the method does not complete successfully.</span></span> 
  
### <a name="verifying-success"></a><span data-ttu-id="a6a2e-156">Проверка успешности</span><span class="sxs-lookup"><span data-stu-id="a6a2e-156">Verifying success</span></span>

<span data-ttu-id="a6a2e-157">Одним из преимуществ использования управляемого API EWS является то, что он предоставляет общий статус при работе с несколькими элементами в одном ответе.</span><span class="sxs-lookup"><span data-stu-id="a6a2e-157">One benefit of using the EWS Managed API is that it provides an overall status when dealing with multiple items in one response.</span></span> <span data-ttu-id="a6a2e-158">Таким образом, если вызываемый метод возвращает **сервицереспонсеколлектион**, вы можете проверить, что свойство [овераллресулт](http://msdn.microsoft.com/en-us/library/dd634515%28v=exchg.80%29.aspx) объекта **сервицереспонсеколлектион** равно [сервицересулт. Success](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.serviceresult%28v=exchg.80%29.aspx).</span><span class="sxs-lookup"><span data-stu-id="a6a2e-158">So if the method you called returns a **ServiceResponseCollection**, you can check that the [OverallResult](http://msdn.microsoft.com/en-us/library/dd634515%28v=exchg.80%29.aspx) property of the **ServiceResponseCollection** is equal to [ServiceResult.Success](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.serviceresult%28v=exchg.80%29.aspx).</span></span> <span data-ttu-id="a6a2e-159">В этом случае все элементы пакетного процесса успешно выполнены; Вам не нужно отдельно проверять каждый объект **сервицереспонсе** .</span><span class="sxs-lookup"><span data-stu-id="a6a2e-159">If so, all the items in the batched process were completed successfully; you don't have to check each **ServiceResponse** object individually.</span></span> <span data-ttu-id="a6a2e-160">Если для свойства **овераллресулт** не задано значение **сервицересулт. Success**, необходимо [обработать сообщение об ошибке или предупреждение](#bk_ewsmaerrors).</span><span class="sxs-lookup"><span data-stu-id="a6a2e-160">If the **OverallResult** property is not set to **ServiceResult.Success**, you have to [handle the error or warning](#bk_ewsmaerrors).</span></span>
  
<span data-ttu-id="a6a2e-161">Если метод, который вы вызываете, не возвращает **сервицереспонсеколлектион**, но возвращает объект **сервицереспонсе** , необходимо проверить значение свойства **result** .</span><span class="sxs-lookup"><span data-stu-id="a6a2e-161">If the method you're calling does not return a **ServiceResponseCollection**, but does return a **ServiceResponse** object, you have to check the value of the **Result** property.</span></span> <span data-ttu-id="a6a2e-162">Если для **результата** задано значение **Success**, метод успешно выполнен.</span><span class="sxs-lookup"><span data-stu-id="a6a2e-162">If the **Result** value is set to **Success**, you know the method completed successfully.</span></span>
  
<span data-ttu-id="a6a2e-163">Если у вызываемого метода нет возвращаемого значения, то нет никакого способа проверить успешность с помощью управляемого API EWS.</span><span class="sxs-lookup"><span data-stu-id="a6a2e-163">If the method you're calling has no return value, there's really no way to check for success via the EWS Managed API.</span></span> <span data-ttu-id="a6a2e-164">Если исключение не создается, можно предположить, что метод выполнен успешно.</span><span class="sxs-lookup"><span data-stu-id="a6a2e-164">As long as an exception is not thrown, you can assume the method completed successfully.</span></span> <span data-ttu-id="a6a2e-165">Для дополнительной проверки можно также [проверить ответ SOAP, чтобы проверить результаты](#bk_verifysoap).</span><span class="sxs-lookup"><span data-stu-id="a6a2e-165">For additional validation, you can also [check the SOAP response to verify the results](#bk_verifysoap).</span></span>
  
### <a name="handling-errors-warnings-and-exceptions"></a><span data-ttu-id="a6a2e-166">Обработка ошибок, предупреждений и исключений</span><span class="sxs-lookup"><span data-stu-id="a6a2e-166">Handling errors, warnings, and exceptions</span></span>
<span data-ttu-id="a6a2e-167"><a name="bk_ewsmaerrors"> </a></span><span class="sxs-lookup"><span data-stu-id="a6a2e-167"><a name="bk_ewsmaerrors"> </a></span></span>

<span data-ttu-id="a6a2e-168">Если код управляемого API EWS создает **исключение**, можно использовать значение [Exception. Message](http://msdn.microsoft.com/EN-US/library/9btwf6wk) для определения источника ошибки.</span><span class="sxs-lookup"><span data-stu-id="a6a2e-168">If your EWS Managed API code throws an **Exception**, you can use the [Exception.Message](http://msdn.microsoft.com/EN-US/library/9btwf6wk) value to determine the source of the error.</span></span> <span data-ttu-id="a6a2e-169">Свойство **Message** содержит содержимое элемента [мессажетекст](http://msdn.microsoft.com/library/59a23bdc-0d9a-4942-8b3c-9cdb11db1ab1%28Office.15%29.aspx) в базовом SOAP ответе.</span><span class="sxs-lookup"><span data-stu-id="a6a2e-169">The **Message** property contains the contents of the [MessageText](http://msdn.microsoft.com/library/59a23bdc-0d9a-4942-8b3c-9cdb11db1ab1%28Office.15%29.aspx) element in the underlying SOAP response.</span></span> <span data-ttu-id="a6a2e-170">Кроме того, если исключение относится к типу [сервицереспонсиксцептион](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.serviceresponseexception%28v=exchg.80%29.aspx) Object, одно из наиболее распространенных исключений, можно также получить [код ошибки](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.serviceresponseexception.errorcode%28v=exchg.80%29.aspx) , содержащийся в базовом элементе SOAP [респонсекоде](http://msdn.microsoft.com/library/4b84d670-74c9-4d6d-84e7-f0a9f76f0d93%28Office.15%29.aspx) , и свойство [Response](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.serviceresponseexception.response%28v=exchg.80%29.aspx) , которое определяет связанный объект [сервицереспонсе](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.serviceresponse%28v=exchg.80%29.aspx) .</span><span class="sxs-lookup"><span data-stu-id="a6a2e-170">In addition, if the exception is of type [ServiceResponseException](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.serviceresponseexception%28v=exchg.80%29.aspx) object, one of the most common exceptions, you can also retrieve the [ErrorCode](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.serviceresponseexception.errorcode%28v=exchg.80%29.aspx) contained in the underlying SOAP [ResponseCode](http://msdn.microsoft.com/library/4b84d670-74c9-4d6d-84e7-f0a9f76f0d93%28Office.15%29.aspx) element, and the [Response](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.serviceresponseexception.response%28v=exchg.80%29.aspx) property that identifies the associated [ServiceResponse](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.serviceresponse%28v=exchg.80%29.aspx) object.</span></span> <span data-ttu-id="a6a2e-171">В приведенном ниже коде показано, как перехватывать и отображать содержимое объекта **сервицереспонсиксцептион**.</span><span class="sxs-lookup"><span data-stu-id="a6a2e-171">The following code shows how to catch and display the contents of a **ServiceResponseException**.</span></span> 
  
```cs
try
    {
         …
    }
    catch (ServiceResponseException ex)
    {
        Console.WriteLine("Error code: " + ex.ErrorCode);
        Console.WriteLine("Error message: " + ex.Message);
        Console.WriteLine("Response: " + ex.Response);
    }
```

<span data-ttu-id="a6a2e-172">Если вызываемый метод возвращает **сервицереспонсеколлектион**, а значение свойства **овераллресулт** равно **предупреждению** или **ошибке**, необходимо перебрать каждый объект в **сервицереспонсеколлектион** , чтобы найти ошибку.</span><span class="sxs-lookup"><span data-stu-id="a6a2e-172">If the method you called returns a **ServiceResponseCollection**, and the value of the **OverallResult** property is equal to **Warning** or **Error**, you'll have to loop through each object in the **ServiceResponseCollection** to find the error.</span></span> <span data-ttu-id="a6a2e-173">Свойство **овераллресулт** имеет значение **warning** , если по крайней мере один ответ имеет **значение** **warning** , а для всех остальных откликов задано значение **Success**. **Result**</span><span class="sxs-lookup"><span data-stu-id="a6a2e-173">The **OverallResult** property is set to **Warning** if at least one response has its **Result** value set to **Warning** and all other responses have their **Result** values set to **Success**.</span></span> <span data-ttu-id="a6a2e-174">Свойство **овераллресулт** имеет значение **Error** , если по крайней мере один ответ имеет **значение** **Error**.</span><span class="sxs-lookup"><span data-stu-id="a6a2e-174">The **OverallResult** property is set to **Error** if at least one response has its **Result** value set to **Error**.</span></span> <span data-ttu-id="a6a2e-175">Если для параметра **овераллресулт** задано значение **warning** или **Error**, для объектов **сервицереспонсе** задаются следующие свойства:</span><span class="sxs-lookup"><span data-stu-id="a6a2e-175">When the **OverallResult** is set to **Warning** or **Error**, the following properties are set on the **ServiceResponse** objects as appropriate:</span></span> 
  
- <span data-ttu-id="a6a2e-176">[ErrorCode](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.serviceresponse.errorcode%28v=exchg.80%29.aspx) — содержит код ошибки, который можно использовать для поиска дополнительных ресурсов по устранению неполадок.</span><span class="sxs-lookup"><span data-stu-id="a6a2e-176">[ErrorCode](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.serviceresponse.errorcode%28v=exchg.80%29.aspx) — Contains the error code, which can be used to find additional troubleshooting resources.</span></span> 
    
- <span data-ttu-id="a6a2e-177">[Еррордетаилс](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.serviceresponse.errordetails%28v=exchg.80%29.aspx) — содержит сведения об ошибке для некоторых **ErrorCodes**.</span><span class="sxs-lookup"><span data-stu-id="a6a2e-177">[ErrorDetails](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.serviceresponse.errordetails%28v=exchg.80%29.aspx) — Contains details about the error for some **ErrorCodes**.</span></span> <span data-ttu-id="a6a2e-178">Например, если код ошибки — **ерроррекурренцехаснуккурренце**, **еррордетаилс** будет содержать ключи для **еффективестартдате** и **еффективинддате**.</span><span class="sxs-lookup"><span data-stu-id="a6a2e-178">For example, when the error code is **ErrorRecurrenceHasNoOccurrence**, the **ErrorDetails** will contain keys for **EffectiveStartDate** and **EffectiveEndDate**.</span></span> 
    
- <span data-ttu-id="a6a2e-179">[ErrorMessage](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.serviceresponse.errormessage%28v=exchg.80%29.aspx) — описание ошибки.</span><span class="sxs-lookup"><span data-stu-id="a6a2e-179">[ErrorMessage](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.serviceresponse.errormessage%28v=exchg.80%29.aspx) — Describes the error.</span></span> 
    
- <span data-ttu-id="a6a2e-180">[Еррорпропертиес](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.serviceresponse.errorproperties%28v=exchg.80%29.aspx) — при наличии — определяет свойства, которые привели к ошибке.</span><span class="sxs-lookup"><span data-stu-id="a6a2e-180">[ErrorProperties](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.serviceresponse.errorproperties%28v=exchg.80%29.aspx) — If available, identifies the properties that caused the error.</span></span> <span data-ttu-id="a6a2e-181">Например, если код ошибки — **ерроринвалидпропертифороператион**, **еррорпропертиес** содержит определение свойства, которое было недопустимым для запроса.</span><span class="sxs-lookup"><span data-stu-id="a6a2e-181">For example, when the error code is **ErrorInvalidPropertyForOperation**, **ErrorProperties** contains the definition of the property that was invalid for the request.</span></span> 
    
- <span data-ttu-id="a6a2e-182">[Result](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.serviceresponse.result%28v=exchg.80%29.aspx) — содержит **сообщение об ошибке** или **предупреждение** при обнаружении ошибки.</span><span class="sxs-lookup"><span data-stu-id="a6a2e-182">[Result](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.serviceresponse.result%28v=exchg.80%29.aspx) — Contains **Error** or **Warning** when an issue is encountered.</span></span> 
    
<span data-ttu-id="a6a2e-183">Если сведения, предоставленные в свойствах **сервицереспонсе** , не предоставляют достаточно сведений для исправления вызова метода или разблокировки пользователя, ознакомьтесь со статьей [Далее](#bk_nextsteps) , чтобы получить дополнительные сведения о значениях **ErrorCode** .</span><span class="sxs-lookup"><span data-stu-id="a6a2e-183">If the information provided by the **ServiceResponse** properties doesn't provide enough information to correct your method call or unblock you, see [Next steps](#bk_nextsteps) to dig up more information on **ErrorCode** values.</span></span> 
  
## 
<span data-ttu-id="a6a2e-184"><a name="bk_nextsteps"> </a></span><span class="sxs-lookup"><span data-stu-id="a6a2e-184"><a name="bk_nextsteps"> </a></span></span>

<span data-ttu-id="a6a2e-185">Дополнительные сведения об устранении неполадок можно найти в следующих разделах:</span><span class="sxs-lookup"><span data-stu-id="a6a2e-185">You can look up additional troubleshooting information in the following topics:</span></span>
  
- <span data-ttu-id="a6a2e-186">Элемент [респонсекоде](http://msdn.microsoft.com/library/4b84d670-74c9-4d6d-84e7-f0a9f76f0d93%28Office.15%29.aspx)</span><span class="sxs-lookup"><span data-stu-id="a6a2e-186">[ResponseCode](http://msdn.microsoft.com/library/4b84d670-74c9-4d6d-84e7-f0a9f76f0d93%28Office.15%29.aspx) element</span></span> 
    
- <span data-ttu-id="a6a2e-187">Перечисление [сервицееррор](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.serviceerror%28v=exchg.80%29.aspx)</span><span class="sxs-lookup"><span data-stu-id="a6a2e-187">[ServiceError](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.serviceerror%28v=exchg.80%29.aspx) enumeration</span></span> 
    
- [<span data-ttu-id="a6a2e-188">Ошибки, связанные со свойством EWS</span><span class="sxs-lookup"><span data-stu-id="a6a2e-188">EWS property-related errors</span></span>](ews-property-related-errors.md)
    
<span data-ttu-id="a6a2e-189">Кроме того, в зависимости от того, что вы пытаетесь выполнить в запросе, вы можете получить дополнительную полезную информацию о коде ошибки в следующих разделах:</span><span class="sxs-lookup"><span data-stu-id="a6a2e-189">In addition, depending on what you're trying to accomplish in your request, you might find additional helpful information about the error code in the following topics:</span></span>
  
- [<span data-ttu-id="a6a2e-190">Обработка сообщений об ошибках службы автообнаружения</span><span class="sxs-lookup"><span data-stu-id="a6a2e-190">Handling Autodiscover error messages</span></span>](handling-autodiscover-error-messages.md)
    
- [<span data-ttu-id="a6a2e-191">Обработка ошибок, связанных с уведомлениями, в EWS в Exchange</span><span class="sxs-lookup"><span data-stu-id="a6a2e-191">Handling notification-related errors in EWS in Exchange</span></span>](handling-notification-related-errors-in-ews-in-exchange.md)
    
- [<span data-ttu-id="a6a2e-192">Обработка ошибок, связанных с синхронизацией, в EWS в Exchange</span><span class="sxs-lookup"><span data-stu-id="a6a2e-192">Handling synchronization-related errors in EWS in Exchange</span></span>](handling-synchronization-related-errors-in-ews-in-exchange.md)
    
- [<span data-ttu-id="a6a2e-193">Обработка ошибок, связанных с удалением, в EWS в Exchange</span><span class="sxs-lookup"><span data-stu-id="a6a2e-193">Handling deletion-related errors in EWS in Exchange</span></span>](handling-deletion-related-errors-in-ews-in-exchange.md)
    
## <a name="see-also"></a><span data-ttu-id="a6a2e-194">См. также</span><span class="sxs-lookup"><span data-stu-id="a6a2e-194">See also</span></span>


- [<span data-ttu-id="a6a2e-195">Разработка клиентов веб-служб для Exchange</span><span class="sxs-lookup"><span data-stu-id="a6a2e-195">Develop web service clients for Exchange</span></span>](develop-web-service-clients-for-exchange.md)
    
- [<span data-ttu-id="a6a2e-196">Инструменты и ресурсы для устранения неполадок приложений EWS для Exchange</span><span class="sxs-lookup"><span data-stu-id="a6a2e-196">Tools and resources for troubleshooting EWS applications for Exchange</span></span>](tools-and-resources-for-troubleshooting-ews-applications-for-exchange.md)
    

