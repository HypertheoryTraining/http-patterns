---
title:  HTTP Pattern Index
published: 2017-08-21
categories: REST, HTTP
layout: page
---
When building HTTP based applications we are limited to a small set of HTTP methods in order to achieve the goals of our application. Once our needs go beyond simple CRUD style manipulation of resource representations, we need to be a little more creative in the way we manipulate resources in order to achieve more complex goals.

The following patterns are based on scenarios that I myself have used in production applications, or I have seen others implement. These patterns are language agnostic, domain agnostic and to my knowledge, exist within the limitations of the REST constraints. 

| Name | Description |
|---|---|
| [Alias](/rest/http/2017/08/21/Alias.html) | A resource designed to provide a logical identifier but without being responsible for incurring the costs of transferring the representation bytes.|
|Action | *Coming soon* A processing resource used to convey a client's intent to invoke some kind of unsafe action on a secondary resource.| 
|[Bouncer](/rest/http/2017/08/21/Bouncer.html)| A resource designed to accept a request body containing complex query parameters and redirect to a new location to enable the results of complex and expensive queries to be cached.|
|[Builder](/rest/http/2017/08/21/builder.html) | A builder resource is much like a factory resource in that it is used to create another resource, however, a builder is a transient resource that enables idempotent creation and allows the client to specify values that cannot change over the lifetime of the created resource.|
|[Bucket](/rest/http/2017/08/21/Bucket.html) | A resource used to indicate the status of a "child" resource. |
|[Discovery](/rest/http/2017/08/21/discovery.html) | This type of resource is used to provide a client with the information it needs to be able to access other resources.| 
|[Factory](https://gooroo.io/GoorooTHINK/Article/16651/HTTP-Patterns--Factory/25702) | A factory resource is one that is used to create another resource. |
|[Miniput](/rest/http/2017/08/21/factory.html) | A resource designed to enable doing a partial updates to another resource.|
|[Progress](/rest/http/2017/08/21/progress.html) | A progress resource is usually a temporary resource that is created automatically by the server to provide status on some long running process that has been initiated by a client. 
|Sandbox | *Coming soon*  A processing resource that is paired with a regular resource to enable making "whatif" style updates and seeing what the results would have been if applied against the regular resource. | 
|Toggle | *Coming soon* A resource that has two distinct states and can easily be switched between those states.|
|[Whackamole](/rest/http/2017/08/21/whack-a-mole.html) | A type of resource that when deleted, re-appears as a different resource.Window |
|Window | *Coming soon*  A resource that provides access to a subset of a larger set of information through the use of parameters that filter, project and zoom information from the complete set.|






