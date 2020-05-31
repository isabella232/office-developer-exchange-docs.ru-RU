---
title: CreateManagedFolder
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- CreateManagedFolder
api_type:
- schema
ms.assetid: cfdf01a9-0191-47c7-a7ad-5254d8bdee4a
description: Элемент CreateManagedFolder определяет запрос на добавление управляемых пользовательских папок в почтовый ящик.
ms.openlocfilehash: 4acc931de2a8665db092c3b309d914f0a3c67558
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/25/2018
ms.locfileid: "19761908"
---
# <a name="createmanagedfolder"></a>CreateManagedFolder

Элемент **CreateManagedFolder** определяет запрос на добавление управляемых пользовательских папок в почтовый ящик. 
  
```xml
<CreateManagedFolder>
   <FolderNames/>
   <Mailbox/>
</CreateManagedFolder>
```

 **креатеманажедфолдеррекуесттипе**
## <a name="attributes-and-elements"></a>Атрибуты и элементы

В следующих разделах описываются атрибуты, дочерние и родительские элементы.
  
### <a name="attributes"></a>Атрибуты

Нет.
  
### <a name="child-elements"></a>Дочерние элементы

|**Элемент**|**Описание**|
|:-----|:-----|
|[фолдернамес](foldernames.md) <br/> |Содержит массив именованных управляемых папок для добавления к почтовому ящику.  <br/> |
|[Mailbox](mailbox.md) <br/> |Определяет объект службы каталогов с включенной поддержкой почты Active Directory.  <br/> |
   
### <a name="parent-elements"></a>Родительские элементы

Нет.
  
## <a name="remarks"></a>Примечания

Учетная запись пользователя, выполняющего запрос, должен иметь разрешения FullAccess для почтового ящика, в котором создаются управляемые папки. Для назначения разрешения FullAccess можно использовать параметр _ – AccessRights _ с командлетом **Add – MailboxPermission** консоли управления Exchange. 
  
Несмотря на то, что вы можете использовать веб-службы Exchange для добавления управляемых папок в почтовый ящик, вы не можете использовать веб-службы Exchange для доступа к списку доступных управляемых папок. Чтобы получить список доступных управляемых папок, используйте командлет **Get – ManagedFolder** Exchange Management Shell. Список, возвращаемый **командлетом Get-ManagedFolder** , будет содержать как управляемые настраиваемые папки, так и управляемые папки по умолчанию. Можно добавлять только папки типа **манажедкустомфолдер** в почтовый ящик с помощью операции CreateManagedFolder. 
  
> [!NOTE]
> Вы также можете получить список управляемых папок с помощью API DirectoryServices платформы Microsoft .NET Framework. 
  
Вы можете использовать [операцию FindFolder](findfolder-operation.md) для поиска управляемых папок в почтовом ящике. Управляемые папки можно отличать, присвоив элементу [басешапе](baseshape.md) значение аллпропертиес в запросе. Ответ будет содержать элемент [манажедфолдеринформатион](managedfolderinformation.md) для различения управляемых папок из папок хранилища Exchange. Вы можете удалять управляемые папки так же, как и другие типы папок. 
  
Схема, описывающая этот элемент, расположена в виртуальном каталоге EWS на компьютере с MicrosoftExchange Server 2007 и установленной ролью сервера клиентского доступа.
  
## <a name="element-information"></a>Сведения об элементе

|||
|:-----|:-----|
|Пространство имен  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|Имя схемы  <br/> |Схема Messages  <br/> |
|Файл проверки  <br/> |Messages. xsd  <br/> |
|Может быть пустым  <br/> |False  <br/> |
   
## <a name="see-also"></a>См. также



[Операция CreateManagedFolder](createmanagedfolder-operation.md)
  
[Операция FindFolder](findfolder-operation.md)


[Поиск папок](http://msdn.microsoft.com/library/9124d868-017a-43f0-b915-5c0082cacec9%28Office.15%29.aspx)
  
[Добавление управляемых папок](http://msdn.microsoft.com/library/846658c6-7043-40fb-8439-19f97c2a967f%28Office.15%29.aspx)

