---
title: Взаимодействие с веб-служб Exchange с помощью управляемого интерфейса API веб-служб Exchange
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
localization_priority: Normal
ms.assetid: d1b78293-da02-413a-875c-681e99146af3
description: Найдите сведения о том, как использовать управляемый API веб-служб Exchange для взаимодействия с веб-служб Exchange в Exchange.
ms.openlocfilehash: 773fcc3f7e95d25effb5a686d4b79ec22610df8c
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/11/2018
ms.locfileid: "19760995"
---
# <a name="communicate-with-ews-by-using-the-ews-managed-api"></a>Взаимодействие с веб-служб Exchange с помощью управляемого интерфейса API веб-служб Exchange

Найдите сведения о том, как использовать управляемый API веб-служб Exchange для взаимодействия с веб-служб Exchange в Exchange.
  
Класс [ExchangeService](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.exchangeservice%28v=exchg.80%29.aspx) в управляемый API EWS содержит методы и свойства, которые позволяют задать учетные данные пользователя, определение конечной точки веб-служб Exchange, отправлять и получать сообщения SOAP и настроить привязку для связи с веб-служб Exchange. Прежде чем использовать управляемый API веб-служб Exchange для выполнения любой задачи, необходимо создать экземпляр класса **ExchangeService** и связать его с веб-служб Exchange. 
  
После настройки конечной точки веб-служб Exchange и объекта [ExchangeService](https://msdn.microsoft.com/library/Microsoft.Exchange.WebServices.Data.ExchangeService.aspx) с использованием учетных данных пользователей, любой объект почтового ящика, который ссылается на объект [ExchangeService](https://msdn.microsoft.com/library/Microsoft.Exchange.WebServices.Data.ExchangeService.aspx) можно использовать следующие типы метод для взаимодействия с веб-служб Exchange: 
  
- Методы объекта ExchangeService — все методы объекта **ExchangeService** , не наследуется из базового типа **объекта** выполнять вызовы веб-служб Exchange. 
    
- Элемент почтовых ящиков Exchange и папки введите методы.
    
**В таблице 1. Элемент почтового ящика и папок введите методы, которые взаимодействуют с веб-служб Exchange**

|Метод|Назначение|Операции, которые он вызывает|
|:-----|:-----|:-----|
|[Нагрузки](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.item.load%28v=exchg.80%29.aspx) <br/> |Получение свойств объекта конфигурации элемента, вложения или пользователя.  <br/> |[GetItem Operation](http://msdn.microsoft.com/library/e3590b8b-c2a7-4dad-a014-6360197b68e4%28Office.15%29.aspx) <br/><br/> [Операция GetAttachment](http://msdn.microsoft.com/library/24d10a15-b942-415e-9024-a6375708f326%28Office.15%29.aspx) <br/><br/> [Операция GetUserConfiguration](http://msdn.microsoft.com/library/71d50e3c-92bd-435f-8118-b28bb85f8138%28Office.15%29.aspx) <br/> |
|[Привязка](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.item.bind%28v=exchg.80%29.aspx) <br/> |Заполняет элемент на стороне клиента с помощью сведений из существующего элемента на сервере.  <br/> |[GetItem Operation](http://msdn.microsoft.com/library/e3590b8b-c2a7-4dad-a014-6360197b68e4%28Office.15%29.aspx) <br/> |
|[Сохранение](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.item.save%28v=exchg.80%29.aspx) <br/> |Сохранение копии элемента клиента на сервере.  <br/> |[UpdateItem Operation](http://msdn.microsoft.com/library/5d027523-e0bc-4da2-b60b-0cb9fc1fdfe4%28Office.15%29.aspx) <br/><br/> [Операцию UpdateFolder](http://msdn.microsoft.com/library/3494c996-b834-4813-b1ca-d99642d8b4e7%28Office.15%29.aspx) <br/><br/>[CreateItem Operation](http://msdn.microsoft.com/library/78a52120-f1d0-4ed7-8748-436e554f75b6%28Office.15%29.aspx) <br/><br/>[CreateFolder Operation](http://msdn.microsoft.com/library/6f6c334c-b190-4e55-8f0a-38f2a018d1b3%28Office.15%29.aspx) <br/> |
|[обновление](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.item.update%28v=exchg.80%29.aspx). <br/> |Обновляет данные на сервере с помощью изменения, внесенные в клиенте.<br/><br/>Для элементов и папок метод **Update** использует [UpdateItem операции](http://msdn.microsoft.com/library/5d027523-e0bc-4da2-b60b-0cb9fc1fdfe4%28Office.15%29.aspx) и [операции UpdateFolder](http://msdn.microsoft.com/library/3494c996-b834-4813-b1ca-d99642d8b4e7%28Office.15%29.aspx).  <br/> |[UpdateItem Operation](http://msdn.microsoft.com/library/5d027523-e0bc-4da2-b60b-0cb9fc1fdfe4%28Office.15%29.aspx) <br/><br/>[Операцию UpdateFolder](http://msdn.microsoft.com/library/3494c996-b834-4813-b1ca-d99642d8b4e7%28Office.15%29.aspx) <br/> |
|[удаление](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.item.delete%28v=exchg.80%29.aspx); <br/> |Удаляет элемент на сервере.<br/><br/>Для элементов и папок метод **Delete** использует и [DeleteFolder операции](http://msdn.microsoft.com/library/b0f92682-4895-4bcf-a4a1-e4c2e8403979%28Office.15%29.aspx).  <br/> |[Операция DeleteItem](http://msdn.microsoft.com/library/3e26c416-fa12-476e-bfd2-5c1f4bb7b348%28Office.15%29.aspx) <br/><br/> [Операция DeleteFolder](http://msdn.microsoft.com/library/b0f92682-4895-4bcf-a4a1-e4c2e8403979%28Office.15%29.aspx) <br/> |
|[Copy](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.item.copy%28v=exchg.80%29.aspx) <br/> |Создает копию элемента или папки на сервере.  <br/> |[CopyItem Operation](http://msdn.microsoft.com/library/bcc68f9e-d511-4c29-bba6-ed535524624a%28Office.15%29.aspx) <br/><br/> [Операция CopyFolder](http://msdn.microsoft.com/library/c7ea0d68-9793-4144-b378-d99536776db9%28Office.15%29.aspx) <br/> |
|[Перемещение](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.item.move%28v=exchg.80%29.aspx) <br/> |Перемещает элементы или папки на сервере.  <br/> |[MoveItem Operation](http://msdn.microsoft.com/library/dcf40fa7-7796-4a5c-bf5b-7a509a18d208%28Office.15%29.aspx) <br/><br/> [Операция MoveFolder](http://msdn.microsoft.com/library/c7233966-6c87-4a14-8156-b1610760176d%28Office.15%29.aspx) <br/> |
   
## <a name="to-use-the-ews-managed-api-to-communicate-with-ews"></a>Чтобы использовать управляемый API веб-служб Exchange для взаимодействия с веб-служб Exchange

1. Создайте экземпляр класса **ExchangeService** . 
    
   ```csharp
    ExchangeService service = new ExchangeService();
   ```

   > [!NOTE]
   > Создание экземпляра **ExchangeService** с пустой конструктор будет создать экземпляр, который привязан к последней известной версии Exchange. Кроме того можно распределять определенной версии Exchange с указанием версии как параметр. `ExchangeService service = new ExchangeService(ExchangeVersion.Exchange2007_SP1);`
  
2. Задание учетных данных пользователя, который отправляет запросы на сервере Exchange. Если вы хотите подключиться к веб-служб Exchange с компьютера, который вошел в систему к домену, с использованием учетных данных пользователя, прошедшего проверку подлинности, задайте свойству **UseDefaultCredentials** объекта **ExchangeService** в **значение true**.
    
   ```cs
    // Connect by using the default credentials of the authenticated user.
    service.UseDefaultCredentials = true;
   ```

   Если вы не хотите подключиться, используя учетные данные пользователя по умолчанию, необходимо задайте свойство **учетные данные** для объекта **ExchangeService** , чтобы явным образом укажите учетные данные другого пользователя. При использовании Exchange Online или Exchange Online в составе Office 365 используется обычная проверка подлинности с помощью только что имя пользователя и пароль. Имя домена является обязательным для проверки подлинности NTLM. 
    
   ```cs
    // Connect by using the credentials of user1 at contoso.com.
    service.Credentials = new WebCredentials("user1@contoso.com", "password");
   ```

   Также можно указать учетные данные пользователя, с помощью доменное имя пользователя и пароль.
    
   ```cs
    // Connect by using the credentials of contoso/user1.
    service.Credentials = new WebCredentials("user1", "password", "contoso");
   ```

   > [!NOTE]
   > Если свойство **UseDefaultCredentials** имеет значение **true**, значение свойства **учетных данных** игнорируется. 
  
3. Задайте URL-адрес конечной точки веб-служб Exchange. Этот URL-адрес определяет местонахождение файла exchange.asmx на сервере клиентского доступа.
    
   ```cs
    // Use Autodiscover to set the URL endpoint.
    service.AutodiscoverUrl("user1@contoso.com");
   ```

   > [!NOTE]
   >  Несмотря на то, что свойство **URL-адрес** **ExchangeService** можно задать значение жестко, мы рекомендуем использовать вместо этого службы автообнаружения по следующим причинам: > автообнаружения определяет наиболее конечной точки для определенного пользователя (конечная точка, который является ближайшим на сервер почтовых ящиков пользователя). > Веб-служб Exchange URL-адрес может изменяться, если развернуть новые серверы клиентского доступа. В этом сценарии с помощью [службы автообнаружения](autodiscover-for-exchange.md) означает, что изменения кода не требуются. > Вам необходимо явно задать URL-адрес или вызова **AutodiscoverUrl**, но не следует оба. 
  
## <a name="see-also"></a>См. также

- [Начало работы с клиентскими приложениями, использующими управляемый API EWS](get-started-with-ews-managed-api-client-applications.md) 
- [Использование службы автообнаружения для поиска точек подключения](how-to-use-autodiscover-to-find-connection-points.md)   
- [Разработка клиентов веб-служб для Exchange](develop-web-service-clients-for-exchange.md)
    

