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
# <a name="validate-a-server-certificate-for-the-ews-managed-api"></a><span data-ttu-id="9ae15-103">Проверка сертификата сервера для управляемого API EWS</span><span class="sxs-lookup"><span data-stu-id="9ae15-103">Validate a server certificate for the EWS Managed API</span></span>

<span data-ttu-id="9ae15-104">Узнайте, как создавать и ссылаться на метод обратного вызова проверки сертификата, чтобы можно было выполнять запросы управляемых API EWS на сервер Exchange.</span><span class="sxs-lookup"><span data-stu-id="9ae15-104">Learn how to create and reference a certificate validation callback method so that you can make EWS Managed API requests to an Exchange server.</span></span>
  
<span data-ttu-id="9ae15-105">По умолчанию версии Exchange начиная с Exchange 2007 с пакетом обновления 1 (SP1) используют сертификаты X509 с собственной подписью для проверки подлинности вызовов из EWS.</span><span class="sxs-lookup"><span data-stu-id="9ae15-105">By default, versions of Exchange starting with Exchange 2007 SP1 use self-signed X509 certificates to authenticate calls from EWS.</span></span> <span data-ttu-id="9ae15-106">При использовании управляемого API EWS необходимо создать метод обратного вызова проверки сертификата; в противном случае запросы управляемых API EWS завершатся с ошибками.</span><span class="sxs-lookup"><span data-stu-id="9ae15-106">When you are using the EWS Managed API, you need to create a certificate validation callback method; otherwise, EWS Managed API requests will fail.</span></span> <span data-ttu-id="9ae15-107">При использовании службы автообнаружения вызов метода автообнаружения управляемого API EWS завершается с ошибкой **аутодисковерлокалексцептион** .</span><span class="sxs-lookup"><span data-stu-id="9ae15-107">If you are using the Autodiscover service, the call to the EWS Managed API Autodiscover method will fail with an **AutodiscoverLocalException** error.</span></span> <span data-ttu-id="9ae15-108">При использовании созданного веб-прокси веб-службы может также потребоваться создать метод обратного вызова проверки в зависимости от способа создания прокси-сервера.</span><span class="sxs-lookup"><span data-stu-id="9ae15-108">If you are using a web-generated web service proxy, you might also have to create a validation callback method, depending on how the proxy is created.</span></span> 
  
## <a name="prerequisites-for-creating-a-validation-callback-method"></a><span data-ttu-id="9ae15-109">Необходимые условия для создания метода обратного вызова проверки</span><span class="sxs-lookup"><span data-stu-id="9ae15-109">Prerequisites for creating a validation callback method</span></span>
<span data-ttu-id="9ae15-110"><a name="bk_prereq"> </a></span><span class="sxs-lookup"><span data-stu-id="9ae15-110"><a name="bk_prereq"> </a></span></span>

<span data-ttu-id="9ae15-111">Чтобы настроить проверку сертификата сервера, убедитесь, что выполняются следующие условия:</span><span class="sxs-lookup"><span data-stu-id="9ae15-111">To set up to validate a server certificate, ensure that the following are true:</span></span> 
  
- <span data-ttu-id="9ae15-112">Сервер Exchange использует самозаверяющий сертификат для EWS.</span><span class="sxs-lookup"><span data-stu-id="9ae15-112">Your Exchange server is using a self-signed certificate for EWS.</span></span> <span data-ttu-id="9ae15-113">Если администратор установил действительный сертификат, который отслеживает корневой сертификат, нет необходимости создавать метод обратного вызова проверки.</span><span class="sxs-lookup"><span data-stu-id="9ae15-113">If the administrator has installed a valid certificate that traces to a root certificate, you do not need to create a validation callback method.</span></span> 
    
- <span data-ttu-id="9ae15-114">Вы создаете управляемое приложение, содержащее ссылку на следующие обязательные пространства имен .NET Framework:</span><span class="sxs-lookup"><span data-stu-id="9ae15-114">You are creating a managed application that includes a reference to the following required .NET Framework namespaces:</span></span> 
    
  - <span data-ttu-id="9ae15-115">**System.Net**</span><span class="sxs-lookup"><span data-stu-id="9ae15-115">**System.Net**</span></span>
  - <span data-ttu-id="9ae15-116">**Система .NET. Security**</span><span class="sxs-lookup"><span data-stu-id="9ae15-116">**System.Net.Security**</span></span>  
  - <span data-ttu-id="9ae15-117">**System. Security. Cryptography. X509Certificates**</span><span class="sxs-lookup"><span data-stu-id="9ae15-117">**System.Security.Cryptography.X509Certificates**</span></span>
    
## <a name="example-callback-method-to-validate-a-server-certificate-for-the-ews-managed-api"></a><span data-ttu-id="9ae15-118">Пример: метод обратного вызова для проверки сертификата сервера для управляемого API EWS</span><span class="sxs-lookup"><span data-stu-id="9ae15-118">Example: Callback method to validate a server certificate for the EWS Managed API</span></span>
<span data-ttu-id="9ae15-119"><a name="bk_example"> </a></span><span class="sxs-lookup"><span data-stu-id="9ae15-119"><a name="bk_example"> </a></span></span>

<span data-ttu-id="9ae15-120">В приведенном ниже примере кода показано, как создать метод обратного вызова проверки сертификата X509 для управляемого API EWS.</span><span class="sxs-lookup"><span data-stu-id="9ae15-120">The following code example shows how to create an X509 certificate validation callback method for the EWS Managed API.</span></span> <span data-ttu-id="9ae15-121">Этот метод проверяет сертификат X509 и возвращает значение true, только если выполнены следующие условия:</span><span class="sxs-lookup"><span data-stu-id="9ae15-121">This method will validate an X509 certificate and only return true when either of the following criteria are met:</span></span> 
  
- <span data-ttu-id="9ae15-122">Сертификат действителен и отслеживается обратно в действительный корневой сертификат.</span><span class="sxs-lookup"><span data-stu-id="9ae15-122">The certificate is valid and traces back to a valid root certificate.</span></span>    
- <span data-ttu-id="9ae15-123">Сертификат действителен и является самозаверяющим сервером, который его вернул.</span><span class="sxs-lookup"><span data-stu-id="9ae15-123">The certificate is valid and is self-signed by the server that returned it.</span></span> 
    
> [!IMPORTANT]
> <span data-ttu-id="9ae15-124">В этом примере метод обратного вызова проверки сертификата обеспечивает достаточную безопасность для разработки и тестирования приложений управляемого API EWS.</span><span class="sxs-lookup"><span data-stu-id="9ae15-124">The certificate validation callback method in this example provides sufficient security for development and testing of EWS Managed API applications.</span></span> <span data-ttu-id="9ae15-125">Тем не менее, это может не обеспечивать достаточную безопасность для развернутого приложения.</span><span class="sxs-lookup"><span data-stu-id="9ae15-125">However, it might not provide sufficient security for your deployed application.</span></span> <span data-ttu-id="9ae15-126">Всегда необходимо убедиться, что используемый способ обратного вызова проверки сертификата соответствует требованиям безопасности Организации.</span><span class="sxs-lookup"><span data-stu-id="9ae15-126">You should always make sure that the certificate validation callback method that you use meets the security requirements of your organization.</span></span> 
  
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

<span data-ttu-id="9ae15-127">Класс **сервицепоинтманажер** в пространстве имен .NET **System.NET** используется для подключения метода обратного вызова проверки путем установки свойства **серверцертификатевалидатионкаллбакк** .</span><span class="sxs-lookup"><span data-stu-id="9ae15-127">You use the **ServicePointManager** class in the .NET **System.Net** namespace to hook up a validation callback method by setting the **ServerCertificateValidationCallback** property.</span></span> <span data-ttu-id="9ae15-128">Для установки свойства **серверцертификатевалидатионкаллбакк** можно использовать код, похожий на приведенный ниже пример кода.</span><span class="sxs-lookup"><span data-stu-id="9ae15-128">You can use code similar to the following code example to set the **ServerCertificateValidationCallback** property.</span></span> 
  
```cs
ServicePointManager.ServerCertificateValidationCallback = CertificateValidationCallBack;

```

## <a name="next-steps"></a><span data-ttu-id="9ae15-129">Дальнейшие действия</span><span class="sxs-lookup"><span data-stu-id="9ae15-129">Next steps</span></span>
<span data-ttu-id="9ae15-130"><a name="bk_example"> </a></span><span class="sxs-lookup"><span data-stu-id="9ae15-130"><a name="bk_example"> </a></span></span>

<span data-ttu-id="9ae15-131">После создания метода обратного вызова проверки для управляемого API EWS можно использовать службу автообнаружения для получения точек подключения и параметров пользователя и домена с сервера Exchange.</span><span class="sxs-lookup"><span data-stu-id="9ae15-131">After you have created the validation callback method for the EWS Managed API, you can use the Autodiscover service to get connection points and user and domain settings from an Exchange server.</span></span> <span data-ttu-id="9ae15-132">Дополнительные сведения см. в следующих статьях:</span><span class="sxs-lookup"><span data-stu-id="9ae15-132">For more information, see the following articles:</span></span>
  
- [<span data-ttu-id="9ae15-133">Поиск точек соединения с помощью службы автообнаружения</span><span class="sxs-lookup"><span data-stu-id="9ae15-133">Use Autodiscover to find connection points</span></span>](how-to-use-autodiscover-to-find-connection-points.md)
    
- [<span data-ttu-id="9ae15-134">Получение параметров пользователя из Exchange с помощью службы автообнаружения</span><span class="sxs-lookup"><span data-stu-id="9ae15-134">Get user settings from Exchange by using Autodiscover</span></span>](how-to-get-user-settings-from-exchange-by-using-autodiscover.md)
    
- [<span data-ttu-id="9ae15-135">Получение параметров домена с сервера Exchange</span><span class="sxs-lookup"><span data-stu-id="9ae15-135">Get domain settings from an Exchange server</span></span>](how-to-get-domain-settings-from-an-exchange-server.md)
    
## <a name="see-also"></a><span data-ttu-id="9ae15-136">См. также</span><span class="sxs-lookup"><span data-stu-id="9ae15-136">See also</span></span>

- [<span data-ttu-id="9ae15-137">Настройка приложения веб-служб Exchange</span><span class="sxs-lookup"><span data-stu-id="9ae15-137">Setting up your EWS application</span></span>](setting-up-your-ews-application.md)  
- [<span data-ttu-id="9ae15-138">Начало работы с веб-службами Exchange</span><span class="sxs-lookup"><span data-stu-id="9ae15-138">Start using web services in Exchange</span></span>](start-using-web-services-in-exchange.md)
    

