---
title: Вложение и EWS в Exchange
manager: sethgros
ms.date: 7/11/2016
ms.audience: Developer
localization_priority: Normal
ms.assetid: 8e4289a4-ec9d-4502-9854-c593c95d5f98
description: Сведения о вложениях, а также о том, как ваши управляемые API EWS и EWS в клиенте Exchange представляют их.
ms.openlocfilehash: e4a97873798b8252e6fc14003519ce8a0eab7ec8
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/25/2018
ms.locfileid: "19760937"
---
# <a name="attachments-and-ews-in-exchange"></a>Вложение и EWS в Exchange

Сведения о вложениях, а также о том, как ваши управляемые API EWS и EWS в клиенте Exchange представляют их.
  
Обычно вложения связываются с элементами электронной почты, но на самом деле все элементы EWS — сообщения электронной почты, элементы календаря, контакты, задачи — могут включать вложения.
  
## <a name="types-of-attachments"></a>Типы вложений

EWS разбивает вложения на две группы: вложенные файлы и вложенные элементы.
  
- **Вложения элементов:** Строго типизированные [элементы EWS](folders-and-items-in-ews-in-exchange.md), такие как сообщения электронной почты и элементы календаря, которые присоединены к другому строго типизированному элементу EWS. Любой строго типизированный элемент, который можно создать с помощью управляемого API EWS или EWS, можно использовать в качестве вложения элемента. Содержимым вложения элемента называется строго типизированный элемент, который обеспечивает легкий доступ ко всем его свойствам. Вложения элементов могут иметь собственные вложенные элементы, поэтому возможна иерархия вложений элементов (или вложенных вложений).
    
- **Вложенные файлы:** Любой файл, например TXT, JPG, ZIP, PDF или даже MSG-файл. Только вложенный файл содержит несколько свойств, один из которых является содержимым файла в кодировке Base-64. 
    
- **Справочные вложения:** Любое вложение, на которое ссылается поставщик файлов, например файл, расположенный в облаке. Вложение может относиться к нескольким поставщикам. 
    
При добавлении или получении вложений из элемента это делается по-разному в зависимости от того, является ли он вложенным файлом или вложением элемента. Например, чтобы добавить вложенный файл в элемент, можно просто передать путь к файлу. Чтобы добавить существующий элемент в качестве вложения элемента, фактически необходимо скопировать свойства или содержимое MIME существующего элемента в новый вложенный элемент; невозможно просто выполнить привязывание к существующему элементу. Поэтому важно различать два типа вложений. Дополнительные сведения о различиях между вложениями элементов и вложениями файлов обсуждаются в статьях, приведенных [в этом разделе](#bk_inthissection).
  
## <a name="how-are-attachments-represented-programmatically"></a>Как программно отображаются вложения?

Вложения хранятся в коллекции элемента EWS. Коллекция вложений состоит из вложенных файлов и/или вложений элементов. Метаданные о коллекции вложений доступны при получении элемента с помощью метода [Item. Bind](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.item.bind%28v=exchg.80%29.aspx) для управляемого API EWS [или операции EWS](http://msdn.microsoft.com/library/e3590b8b-c2a7-4dad-a014-6360197b68e4%28Office.15%29.aspx) , но для фактического получения содержимого вложений требуются дополнительные вызовы. 
  
**Таблица 1. Метаданные элемента о вложениях**

|**Сущность метаданных**|**Свойство управляемого API EWS**|**Элемент EWS**|
|:-----|:-----|:-----|
|Индикатор вложения (не помечает встроенные вложения)  <br/> |[Item. HasAttachments](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.item.hasattachments%28v=exchg.80%29.aspx) <br/> |[HasAttachments](http://msdn.microsoft.com/library/538b7a85-11d7-4daa-8458-09b540760e8b%28Office.15%29.aspx) <br/> |
|Коллекция Attachment  <br/> |[Item. вложения](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.item.attachments%28v=exchg.80%29.aspx) <br/> |[Вложения](http://msdn.microsoft.com/library/b470e614-34bb-44f0-8790-7ddbdcbbd29d%28Office.15%29.aspx) <br/> |
|Идентификатор вложения  <br/> |[Attachment.Id](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.attachment.id%28v=exchg.80%29.aspx) <br/> |[AttachmentId](http://msdn.microsoft.com/library/55a5fd77-60d1-40fa-8144-770600cedc6a%28Office.15%29.aspx) <br/> |
   
**Таблица 2. Сущности вложений**

|**Тип вложения**|**Класс управляемого API EWS**|**Элемент EWS**|
|:-----|:-----|:-----|
|Вложенный файл  <br/> |[FileAttachment](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.fileattachment%28v=exchg.80%29.aspx) <br/> |[FileAttachment](http://msdn.microsoft.com/library/3ecea174-73d1-47fd-8917-6065cef1d565%28Office.15%29.aspx) <br/> |
|Вложение элемента  <br/> |[ItemAttachment](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.itemattachment%28v=exchg.80%29.aspx) <br/> [ItemAttachment\<титем\>](http://msdn.microsoft.com/en-us/library/dd635165%28v=exchg.80%29.aspx) <br/> |[ItemAttachment](http://msdn.microsoft.com/library/089ee599-f45e-46f5-a18a-5cfb3d2851ff%28Office.15%29.aspx) <br/> |
|Вложение в виде ссылки  <br/> |[Референцеаттачменттипе complexType (EWS)](http://msdn.microsoft.com/library/18bfa012-e903-d7f3-528a-31ccceb65463%28Office.15%29.aspx) <br/> |[ReferenceAttachment](http://msdn.microsoft.com/library/b9bde862-6b75-4a81-8033-00a47be4dc2f%28Office.15%29.aspx) <br/> |
   
## <a name="inline-attachments"></a>Встроенные вложения

Встроенные вложения являются особым породом вложения. Вложенные файлы и вложения элементов могут быть встроенными вложениями. Встроенное вложение отображается как часть содержимого тела и сохраняет свое положение относительно остального содержимого элемента. 
  
Вложение — это встроенное вложение, если свойство [IsInline](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.attachment.isinline%28v=exchg.80%29.aspx) для управляемого API EWS или элемент EWS [IsInline](http://msdn.microsoft.com/library/5e7712c8-372a-4a16-be64-360c5ff3961a%28Office.15%29.aspx) имеет значение true. Встроенные вложения используют следующие необязательные свойства и элементы для определения расположения встроенного вложения: 
  
- Управляемый API EWS — свойства [ContentId](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.attachment.contentid%28v=exchg.80%29.aspx) или [ContentLocation](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.attachment.contentlocation%28v=exchg.80%29.aspx) . 
    
- EWS — идентификатор [ContentId](http://msdn.microsoft.com/library/bc59100d-6079-414b-a6e0-7c15feaa3184%28Office.15%29.aspx) или [ContentLocation](http://msdn.microsoft.com/library/d91cf587-24e3-4c13-8784-5ca29787cca7%28Office.15%29.aspx) . 
    
Обратите внимание, что свойство [HasAttachments](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.item.hasattachments%28v=exchg.80%29.aspx) управляемого API EWS и элемент EWS [HasAttachments](http://msdn.microsoft.com/library/538b7a85-11d7-4daa-8458-09b540760e8b%28Office.15%29.aspx) не отражают существование встроенных вложений, поэтому встроенные вложения также называются скрытыми вложениями. Таким образом, если задать для свойства [IsInline](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.attachment.isinline%28v=exchg.80%29.aspx) управляемого API EWS или EWS [IsInline](http://msdn.microsoft.com/library/5e7712c8-372a-4a16-be64-360c5ff3961a%28Office.15%29.aspx) элемент true, а у элемента нет других вложений, **HasAttachments** будет установлено значение false. Если ваш клиент использует **HasAttachments** для заполнения значка вложения или значка в сообщении электронной почты, обратите внимание на то, что значок не будет отображаться для электронных сообщений с вложенными вложениями. 
  
## <a name="in-this-section"></a>В этом разделе:
<a name="bk_inthissection"> </a>

- [Добавление вложений с помощью EWS в Exchange](how-to-add-attachments-by-using-ews-in-exchange.md)
    
- [Получение вложений с помощью EWS в Exchange](how-to-get-attachments-by-using-ews-in-exchange.md)
    
- [Удаление вложений с помощью EWS в Exchange](how-to-delete-attachments-by-using-ews-in-exchange.md)
    
## <a name="see-also"></a>См. также
<a name="bk_additionalresources"> </a>

- [Разработка клиентов веб-служб для Exchange](develop-web-service-clients-for-exchange.md)
    
- [Папки и элементы в веб-службах Exchange](folders-and-items-in-ews-in-exchange.md)
    
- [Электронная почта и веб-службах Exchange](email-and-ews-in-exchange.md)
    

