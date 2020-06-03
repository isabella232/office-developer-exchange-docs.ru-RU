---
title: Проверка сертификата сервера для управляемого API EWS
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.assetid: 1fe0b215-8340-4bc8-a6ce-4f591ca9e353
description: Узнайте, как создавать и ссылаться на метод обратного вызова проверки сертификата, чтобы можно было выполнять запросы управляемых API EWS на сервер Exchange.
localization_priority: Priority
ms.openlocfilehash: 195c51ca71890d6092e4182d23990bb528d37095
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/31/2020
ms.locfileid: "44456782"
---
# <a name="validate-a-server-certificate-for-the-ews-managed-api"></a>Проверка сертификата сервера для управляемого API EWS

Узнайте, как создавать и ссылаться на метод обратного вызова проверки сертификата, чтобы можно было выполнять запросы управляемых API EWS на сервер Exchange.
  
По умолчанию версии Exchange начиная с Exchange 2007 с пакетом обновления 1 (SP1) используют сертификаты X509 с собственной подписью для проверки подлинности вызовов из EWS. При использовании управляемого API EWS необходимо создать метод обратного вызова проверки сертификата; в противном случае запросы управляемых API EWS завершатся с ошибками. При использовании службы автообнаружения вызов метода автообнаружения управляемого API EWS завершается с ошибкой **аутодисковерлокалексцептион** . При использовании созданного веб-прокси веб-службы может также потребоваться создать метод обратного вызова проверки в зависимости от способа создания прокси-сервера. 
  
## <a name="prerequisites-for-creating-a-validation-callback-method"></a>Необходимые условия для создания метода обратного вызова проверки
<a name="bk_prereq"> </a>

Чтобы настроить проверку сертификата сервера, убедитесь, что выполняются следующие условия: 
  
- Сервер Exchange использует самозаверяющий сертификат для EWS. Если администратор установил действительный сертификат, который отслеживает корневой сертификат, нет необходимости создавать метод обратного вызова проверки. 
    
- Вы создаете управляемое приложение, содержащее ссылку на следующие обязательные пространства имен .NET Framework: 
    
  - **System.Net**
  - **Система .NET. Security**  
  - **System. Security. Cryptography. X509Certificates**
    
## <a name="example-callback-method-to-validate-a-server-certificate-for-the-ews-managed-api"></a>Пример: метод обратного вызова для проверки сертификата сервера для управляемого API EWS
<a name="bk_example"> </a>

В приведенном ниже примере кода показано, как создать метод обратного вызова проверки сертификата X509 для управляемого API EWS. Этот метод проверяет сертификат X509 и возвращает значение true, только если выполнены следующие условия: 
  
- Сертификат действителен и отслеживается обратно в действительный корневой сертификат.    
- Сертификат действителен и является самозаверяющим сервером, который его вернул. 
    
> [!IMPORTANT]
> В этом примере метод обратного вызова проверки сертификата обеспечивает достаточную безопасность для разработки и тестирования приложений управляемого API EWS. Тем не менее, это может не обеспечивать достаточную безопасность для развернутого приложения. Всегда необходимо убедиться, что используемый способ обратного вызова проверки сертификата соответствует требованиям безопасности Организации. 
  
```cs
      private static bool CertificateValidationCallBack(
         object sender,
         System.Security.Cryptography.X509Certificates.X509Certificate certificate,
         System.Security.Cryptography.X509Certificates.X509Chain chain,
         System.Net.Security.SslPolicyErrors sslPolicyErrors)
    {
      // If the certificate is a valid, signed certificate, return true.
      if (sslPolicyErrors == System.Net.Security.SslPolicyErrors.None)
      {
        return true;
      }
      // If there are errors in the certificate chain, look at each error to determine the cause.
      if ((sslPolicyErrors &amp; System.Net.Security.SslPolicyErrors.RemoteCertificateChainErrors) != 0)
      {
        if (chain != null &amp;&amp; chain.ChainStatus != null)
        {
          foreach (System.Security.Cryptography.X509Certificates.X509ChainStatus status in chain.ChainStatus)
          {
            if ((certificate.Subject == certificate.Issuer) &amp;&amp;
               (status.Status == System.Security.Cryptography.X509Certificates.X509ChainStatusFlags.UntrustedRoot))
            {
              // Self-signed certificates with an untrusted root are valid. 
              continue;
            }
            else
            {
              if (status.Status != System.Security.Cryptography.X509Certificates.X509ChainStatusFlags.NoError)
              {
                // If there are any other errors in the certificate chain, the certificate is invalid,
             // so the method returns false.
                return false;
              }
            }
          }
        }
        // When processing reaches this line, the only errors in the certificate chain are 
    // untrusted root errors for self-signed certificates. These certificates are valid
    // for default Exchange server installations, so return true.
        return true;
      }
      else
      {
     // In all other cases, return false.
        return false;
      }
    }

```

Класс **сервицепоинтманажер** в пространстве имен .NET **System.NET** используется для подключения метода обратного вызова проверки путем установки свойства **серверцертификатевалидатионкаллбакк** . Для установки свойства **серверцертификатевалидатионкаллбакк** можно использовать код, похожий на приведенный ниже пример кода. 
  
```cs
ServicePointManager.ServerCertificateValidationCallback = CertificateValidationCallBack;

```

## <a name="next-steps"></a>Дальнейшие действия
<a name="bk_example"> </a>

После создания метода обратного вызова проверки для управляемого API EWS можно использовать службу автообнаружения для получения точек подключения и параметров пользователя и домена с сервера Exchange. Дополнительные сведения см. в следующих статьях:
  
- [Поиск точек соединения с помощью службы автообнаружения](how-to-use-autodiscover-to-find-connection-points.md)
    
- [Получение параметров пользователя из Exchange с помощью службы автообнаружения](how-to-get-user-settings-from-exchange-by-using-autodiscover.md)
    
- [Получение параметров домена с сервера Exchange](how-to-get-domain-settings-from-an-exchange-server.md)
    
## <a name="see-also"></a>См. также

- [Настройка приложения веб-служб Exchange](setting-up-your-ews-application.md)  
- [Начало работы с веб-службами Exchange](start-using-web-services-in-exchange.md)
    

