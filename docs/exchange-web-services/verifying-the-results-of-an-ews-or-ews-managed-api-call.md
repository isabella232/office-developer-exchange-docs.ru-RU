---
title: Проверка результатов вызова EWS или управляемого API EWS
manager: sethgros
ms.date: 11/16/2014
ms.audience: Developer
ms.assetid: 78a1741c-1bbe-4cb4-9331-9d6d3171fc11
description: Узнайте, как проверить результаты вызовов управляемого API EWS или EWS.
localization_priority: Priority
ms.openlocfilehash: be8e76898dd111a6dec33d4a57d9d50a2a935390
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/31/2020
ms.locfileid: "44457398"
---
# <a name="verifying-the-results-of-an-ews-or-ews-managed-api-call"></a>Проверка результатов вызова EWS или управляемого API EWS

Узнайте, как проверить результаты вызовов управляемого API EWS или EWS.
  
Если что-то не работает должным образом, вы можете узнать, что происходит с помощью проверки SOAP-запросов, отправляемых приложением по сети, и ответов, отправляемых сервером обратно. В статье [Tools and Resources for устранение неполадок приложений EWS](tools-and-resources-for-troubleshooting-ews-applications-for-exchange.md) содержатся ссылки на средства, помогающие записывать и просматривать эти SOAP запросы. После того как вы получите запросы и ответы, как убедиться, что отправленный на сервер запрос был обработан правильно? Прочтите статью, чтобы узнать. 
  
Если вы отправляете запросы EWS, вы собираетесь начать проверку, проверив атрибут **респонсекласс** для каждого ответного сообщения в ответе. С помощью которого вы узнаете, успешно ли завершена операция для каждого элемента. 
  
В зависимости от объекта, который вызывается методом, если вы используете управляемый API EWS для отправки запросов, можно выполнить некоторую проверку с помощью объектов Response. Но так как ответ SOAP содержит надмножество элементов, включенных в объекты ответа управляемых API EWS, может также потребоваться взглянуть на SOAP-ответ. Так как ответ SOAP часто содержит больше сведений, чем объекты ответа управляемого API EWS, запустите проверку с ответом SOAP.
  
## <a name="verifying-the-results-of-a-soap-response"></a>Проверка результатов ответа SOAP
<a name="bk_verifysoap"> </a>

При получении ответа SOAP первым делом рассмотрим атрибут **респонсекласс** . Этот атрибут включается в каждый экземпляр **респонсемессажетипе** в элементе [респонсемессажес](https://msdn.microsoft.com/library/2071bed8-ea66-4627-aa4f-a1d9a025cf3d%28Office.15%29.aspx) , как показано в следующем примере. 
  
```XML
<s:Body>
      <m:GetItemResponse xmlns:m="https://schemas.microsoft.com/exchange/services/2006/messages"
                         xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types">
        <m:ResponseMessages>
          <m:GetItemResponseMessage ResponseClass="Success">
          …
```

Так как ответ SOAP может содержать несколько ответных сообщений в едином SOAP-ответе, важно проверять каждое ответное сообщение по отдельности.
  
Если вы работаете с операцией, которая включает **респонсекласс** в ответ операции, как показано ниже, возможно, вы можете просмотреть только **респонсекласс** операции. 
  
```XML
<soap:Body>
  <m:AddDelegateResponse xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types"
                         ResponseClass="Success"
                         xmlns:m="https://schemas.microsoft.com/exchange/services/2006/messages">
  …

```

Однако состояние операции отражает только форму отклика верхнего уровня и не отражает состояние всех индивидуальных ответов на сообщения. В следующем примере операция [аддделегатереспонсе](https://msdn.microsoft.com/library/d7e6bebb-5dbf-43c1-aacf-4b3ca6a7c429%28Office.15%29.aspx) имеет **респонсекласс** **успешного**выполнения, но базовый элемент [делегатеусерреспонсемессажетипе](https://msdn.microsoft.com/library/3dc9552c-1e2d-40ac-a137-827883c2bb88%28Office.15%29.aspx) имеет значение **ошибки** **респонсекласс** .
  
```XML
<soap:Body>
  <m:AddDelegateResponse xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types"
                         ResponseClass="Success"
                         xmlns:m="https://schemas.microsoft.com/exchange/services/2006/messages">
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

Таким образом, для ответов SOAP EWS вы не можете полагаться на **респонсекласс** операции, чтобы определить, обнаружила ли операция ошибки при обработке элементов, необходимо взглянуть на **респонсекласс** каждого ответного сообщения. 
  
### <a name="verifying-success"></a>Проверка успешности

Если каждому атрибуту **респонсекласс** для каждого атрибута **респонсемессаже** присвоено значение **Success**, операция успешно завершена для всех элементов, и вы можете перейти к следующей задаче.
  
В следующем примере показан успешный ответ на запрос операции [GetItem](https://msdn.microsoft.com/library/e8492e3b-1c8d-4b14-8070-9530f8306edd%28Office.15%29.aspx) для получения одного элемента. Обратите внимание, что если для **респонсекласс** задано значение **Success**, связанному [респонсекодеу](https://msdn.microsoft.com/library/4b84d670-74c9-4d6d-84e7-f0a9f76f0d93%28Office.15%29.aspx) всегда присваивается значение " **Ошибка**".
  
```XML
<s:Body xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" 
             xmlns:xsd="http://www.w3.org/2001/XMLSchema">
      <m:GetItemResponse xmlns:m="https://schemas.microsoft.com/exchange/services/2006/messages"
                         xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types">
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

Ниже приведен успешный ответ на запрос операции **GetItem** для получения нескольких элементов. Каждый из элементов [жетитемреспонсемессаже](https://msdn.microsoft.com/library/cc583723-54d1-4a17-8c1f-6586f70fdefd%28Office.15%29.aspx) имеет **респонсекласс** **об успехе**.
  
```XML
<s:Body xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance"
             xmlns:xsd="http://www.w3.org/2001/XMLSchema">
  <m:GetItemResponse xmlns:m="https://schemas.microsoft.com/exchange/services/2006/messages"
                     xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types">
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

### <a name="handling-errors-and-warnings"></a>Обработка ошибок и предупреждений

При получении ответа, если для атрибута **респонсекласс** задано значение **Error**, операция не была успешно завершена для одного или нескольких элементов. Устраните ошибку и повторите запрос или часть запроса, в которой произошел сбой. Значение свойства **респонсекласс** , равное значению **warning** , возвращается только операцией [ResolveNames](https://msdn.microsoft.com/library/6b4eb4b3-9ad6-4804-a09f-7e20cfea4dbb%28Office.15%29.aspx) и указывает, что сущность не может быть сопоставлена с уникальным идентификатором. Вы можете игнорировать его для всех других операций. 
  
В следующем ответе атрибут **респонсекласс** имеет значение **Error**.
  
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

В этом примере EWS предоставляет сведения для отладки неполадок. Если для атрибута **респонсекласс** задано значение **Error**, при необходимости в отклике включаются следующие дополнительные элементы:
  
- [Мессажетекст](https://msdn.microsoft.com/library/59a23bdc-0d9a-4942-8b3c-9cdb11db1ab1%28Office.15%29.aspx) — описание ошибки. 
    
- [Респонсекоде](https://msdn.microsoft.com/library/4b84d670-74c9-4d6d-84e7-f0a9f76f0d93%28Office.15%29.aspx) — содержит код ошибки, который можно использовать для поиска дополнительных ресурсов по устранению неполадок. 
    
- [Мессажексмл](https://msdn.microsoft.com/library/bcaf9e35-d351-48f3-baad-f90c633cba8a%28Office.15%29.aspx) — определяет элементы, которые привели к ошибке. 
    
- [Дескриптивелинккэй](https://msdn.microsoft.com/library/f7f36749-00f3-4915-b17c-e3caa0af6e67%28Office.15%29.aspx) — не используется. 
    
Сведения, приведенные в этих элементах, можно использовать для изучения возникшей проблемы. В предыдущем примере **мессажетекст** указывает, что свойство не является допустимым для типа объекта. В запросе было получено сообщение электронной почты, но в набор свойств включено свойство **ассоЦиатедкалендаритемид**, которое является допустимым только для элементов встречи.
  
В следующем примере показана ошибка, полученная в составе пакетной операции для получения нескольких элементов электронной почты. Первый элемент был успешно получен, а для **респонсекласс** задано значение **Success**. Не удалось найти второй элемент, а для параметра **респонсекласс** задано значение **Error**.
  
```XML
<m:GetItemResponse xmlns:m="https://schemas.microsoft.com/exchange/services/2006/messages"
                        xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types">
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

Если один или несколько элементов в пакетном запросе не могут быть обработаны как запрошенные, возвращается ошибка для каждого элемента, для которого произошел сбой, а остальные элементы пакета обрабатываются должным образом. Ошибки в пакетной обработке могут возникать, если элемент был удален, поэтому его невозможно отправить, извлечь или обновить, или если элемент перемещен в другую папку, и поэтому имеет новый идентификатор элемента. Так как операция будет выполнена для некоторых элементов и не будет возвращать ошибку при невозможности обработать один или несколько элементов, важно проверить каждый атрибут **респонсекласс** , прежде чем переходить к следующей операции. 
  
Если сведения, предоставляемые элементами ответа, не помогают исправить запрос или не разблокируют вас, ознакомьтесь со статьей [дальнейшие действия](#bk_nextsteps).
  
## <a name="verifying-the-results-of-an-ews-managed-api-method-call"></a>Проверка результатов вызова метода управляемого API EWS
<a name="bk_successful"> </a>

Если вы используете управляемый API EWS и вызываете метод для объекта [ExchangeService](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.exchangeservice%28v=exchg.80%29.aspx) , ваш метод скорее всего вернет объект [сервицереспонсеколлектион](https://msdn.microsoft.com/library/dd633715%28v=exchg.80%29.aspx) , который содержит коллекцию объектов [сервицереспонсе](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.serviceresponse%28v=exchg.80%29.aspx) , или коллекцию объектов, производных от объектов **сервицереспонсе** . **Сервицереспонсеколлектион** и включенные объекты **сервицереспонсе** содержат сведения о результатах вызова метода, которые можно использовать для проверки результатов. 
  
Если вы используете управляемый API EWS и вызываете метод для объекта [Item](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.item%28v=exchg.80%29.aspx) или один из производных объектов, метод, скорее всего, не возвращает объект Response для проверки на успешное выполнение, но при этом создает [исключение](https://msdn.microsoft.com/library/c18k6c59) , если метод не завершается успешно. 
  
### <a name="verifying-success"></a>Проверка успешности

Одним из преимуществ использования управляемого API EWS является то, что он предоставляет общий статус при работе с несколькими элементами в одном ответе. Таким образом, если вызываемый метод возвращает **сервицереспонсеколлектион**, вы можете проверить, что свойство [овераллресулт](https://msdn.microsoft.com/library/dd634515%28v=exchg.80%29.aspx) объекта **сервицереспонсеколлектион** равно [сервицересулт. Success](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.serviceresult%28v=exchg.80%29.aspx). В этом случае все элементы пакетного процесса успешно выполнены; Вам не нужно отдельно проверять каждый объект **сервицереспонсе** . Если для свойства **овераллресулт** не задано значение **сервицересулт. Success**, необходимо [обработать сообщение об ошибке или предупреждение](#bk_ewsmaerrors).
  
Если метод, который вы вызываете, не возвращает **сервицереспонсеколлектион**, но возвращает объект **сервицереспонсе** , необходимо проверить значение свойства **result** . Если для **результата** задано значение **Success**, метод успешно выполнен.
  
Если у вызываемого метода нет возвращаемого значения, то нет никакого способа проверить успешность с помощью управляемого API EWS. Если исключение не создается, можно предположить, что метод выполнен успешно. Для дополнительной проверки можно также [проверить ответ SOAP, чтобы проверить результаты](#bk_verifysoap).
  
### <a name="handling-errors-warnings-and-exceptions"></a>Обработка ошибок, предупреждений и исключений
<a name="bk_ewsmaerrors"> </a>

Если код управляемого API EWS создает **исключение**, можно использовать значение [Exception. Message](https://msdn.microsoft.com/library/9btwf6wk) для определения источника ошибки. Свойство **Message** содержит содержимое элемента [мессажетекст](https://msdn.microsoft.com/library/59a23bdc-0d9a-4942-8b3c-9cdb11db1ab1%28Office.15%29.aspx) в базовом SOAP ответе. Кроме того, если исключение относится к типу [сервицереспонсиксцептион](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.serviceresponseexception%28v=exchg.80%29.aspx) Object, одно из наиболее распространенных исключений, можно также получить [код ошибки](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.serviceresponseexception.errorcode%28v=exchg.80%29.aspx) , содержащийся в базовом элементе SOAP [респонсекоде](https://msdn.microsoft.com/library/4b84d670-74c9-4d6d-84e7-f0a9f76f0d93%28Office.15%29.aspx) , и свойство [Response](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.serviceresponseexception.response%28v=exchg.80%29.aspx) , которое определяет связанный объект [сервицереспонсе](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.serviceresponse%28v=exchg.80%29.aspx) . В приведенном ниже коде показано, как перехватывать и отображать содержимое объекта **сервицереспонсиксцептион**. 
  
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

Если вызываемый метод возвращает **сервицереспонсеколлектион**, а значение свойства **овераллресулт** равно **предупреждению** или **ошибке**, необходимо перебрать каждый объект в **сервицереспонсеколлектион** , чтобы найти ошибку. Свойство **овераллресулт** имеет значение **warning** , если по крайней мере один ответ имеет **значение** **warning** , а для всех остальных откликов задано значение **Success**. **Result** Свойство **овераллресулт** имеет значение **Error** , если по крайней мере один ответ имеет **значение** **Error**. Если для параметра **овераллресулт** задано значение **warning** или **Error**, для объектов **сервицереспонсе** задаются следующие свойства: 
  
- [ErrorCode](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.serviceresponse.errorcode%28v=exchg.80%29.aspx) — содержит код ошибки, который можно использовать для поиска дополнительных ресурсов по устранению неполадок. 
    
- [Еррордетаилс](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.serviceresponse.errordetails%28v=exchg.80%29.aspx) — содержит сведения об ошибке для некоторых **ErrorCodes**. Например, если код ошибки — **ерроррекурренцехаснуккурренце**, **еррордетаилс** будет содержать ключи для **еффективестартдате** и **еффективинддате**. 
    
- [ErrorMessage](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.serviceresponse.errormessage%28v=exchg.80%29.aspx) — описание ошибки. 
    
- [Еррорпропертиес](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.serviceresponse.errorproperties%28v=exchg.80%29.aspx) — при наличии — определяет свойства, которые привели к ошибке. Например, если код ошибки — **ерроринвалидпропертифороператион**, **еррорпропертиес** содержит определение свойства, которое было недопустимым для запроса. 
    
- [Result](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.serviceresponse.result%28v=exchg.80%29.aspx) — содержит **сообщение об ошибке** или **предупреждение** при обнаружении ошибки. 
    
Если сведения, предоставленные в свойствах **сервицереспонсе** , не предоставляют достаточно сведений для исправления вызова метода или разблокировки пользователя, ознакомьтесь со статьей [Далее](#bk_nextsteps) , чтобы получить дополнительные сведения о значениях **ErrorCode** . 
  
## 
<a name="bk_nextsteps"> </a>

Дополнительные сведения об устранении неполадок можно найти в следующих разделах:
  
- Элемент [респонсекоде](https://msdn.microsoft.com/library/4b84d670-74c9-4d6d-84e7-f0a9f76f0d93%28Office.15%29.aspx) 
    
- Перечисление [сервицееррор](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.serviceerror%28v=exchg.80%29.aspx) 
    
- [Ошибки, связанные со свойством EWS](ews-property-related-errors.md)
    
Кроме того, в зависимости от того, что вы пытаетесь выполнить в запросе, вы можете получить дополнительную полезную информацию о коде ошибки в следующих разделах:
  
- [Обработка сообщений об ошибках службы автообнаружения](handling-autodiscover-error-messages.md)
    
- [Обработка ошибок, связанных с уведомлениями, в EWS в Exchange](handling-notification-related-errors-in-ews-in-exchange.md)
    
- [Обработка ошибок, связанных с синхронизацией, в EWS в Exchange](handling-synchronization-related-errors-in-ews-in-exchange.md)
    
- [Обработка ошибок, связанных с удалением, в EWS в Exchange](handling-deletion-related-errors-in-ews-in-exchange.md)
    
## <a name="see-also"></a>См. также


- [Разработка клиентов веб-служб для Exchange](develop-web-service-clients-for-exchange.md)
    
- [Инструменты и ресурсы для устранения неполадок приложений EWS для Exchange](tools-and-resources-for-troubleshooting-ews-applications-for-exchange.md)
    

