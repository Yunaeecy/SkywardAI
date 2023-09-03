# 🎼 BFF

Credit:

{% embed url="https://blog.bitsrc.io/bff-pattern-backend-for-frontend-an-introduction-e4fa965128bf" %}

You self-contained APIs should be in the microservices layer.

BFF is a translation layer between the client and the services.

When data is returned from a service API, the purpose of it is to transform it into the data type specified by the client application.

The BFF will do the following.

* Call the relevant microservices APIs and obtain the needed data
* Format the data based on the frontend representation
* Send the formatted data to the frontend

If your application depends on microservices and consumes many external APIs and other services, it is better to use a BFF to streamline the data flow and introduce a lot of efficiency to your application.

Purpose of having a BFF is to provide your client a focused interface to connect with. For example, data consumption by a mobile UI could be different from data consumption by a browser. In that case, for better data representation, two BFFs can be used.

<figure><img src="../.gitbook/assets/image (11).png" alt=""><figcaption></figcaption></figure>

