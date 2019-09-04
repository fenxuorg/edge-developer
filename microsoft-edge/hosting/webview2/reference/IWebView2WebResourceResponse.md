---
description: Host web content in your Win32 app with the Microsoft Edge WebView2 control
title: Microsoft Edge WebView2 for Win32 apps
author: MSEdgeTeam
ms.author: msedgedevrel
ms.date: 07/29/2019
ms.topic: reference
ms.prod: microsoft-edge
ms.technology: webview
keywords: IWebView2, IWebView2WebView, webview2, webview, win32 apps, win32, edge
---

# interface IWebView2WebResourceResponse 

```
interface IWebView2WebResourceResponse
  : public IUnknown
```

An HTTP response used with the WebResourceRequested event.

## Summary

 Members                        | Descriptions
--------------------------------|---------------------------------------------
[get_Content](#get_content) | HTTP response content as stream.
[put_Content](#put_content) | Set the Content property.
[get_Headers](#get_headers) | Overridden HTTP response headers.
[get_StatusCode](#get_statuscode) | The HTTP response status code.
[put_StatusCode](#put_statuscode) | Set the StatusCode property.
[get_ReasonPhrase](#get_reasonphrase) | The HTTP response reason phrase.
[put_ReasonPhrase](#put_reasonphrase) | Set the ReasonPhrase property.

## Members

#### get_Content 

HTTP response content as stream.

> public HRESULT [get_Content](#interface_i_web_view2_web_resource_response_1a1eefcd262414db70d95ac1508e89782a)(IStream ** content)

Stream must have all the content data available by the time this response's WebResourceRequested event deferral is completed. Stream should be agile or be created from a background thread to prevent performance impact to the UI thread. Null means no content data. IStream semantics apply (return S_OK to Read calls until all data is exhausted)

#### put_Content 

Set the Content property.

> public HRESULT [put_Content](#interface_i_web_view2_web_resource_response_1ad788c7c4f69d90704a648368df7d7ae2)(IStream * content)

#### get_Headers 

Overridden HTTP response headers.

> public HRESULT [get_Headers](#interface_i_web_view2_web_resource_response_1abfb232e76c9174eec6e9322fe4019eac)([IWebView2HttpResponseHeaders](IWebView2HttpResponseHeaders.md#interface_i_web_view2_http_response_headers) ** headers)

#### get_StatusCode 

The HTTP response status code.

> public HRESULT [get_StatusCode](#interface_i_web_view2_web_resource_response_1af7dd8039627a9b499c0ac219abe91593)(int * statusCode)

#### put_StatusCode 

Set the StatusCode property.

> public HRESULT [put_StatusCode](#interface_i_web_view2_web_resource_response_1a70218592959208c7335c7a7894b55d6d)(int statusCode)

#### get_ReasonPhrase 

The HTTP response reason phrase.

> public HRESULT [get_ReasonPhrase](#interface_i_web_view2_web_resource_response_1a423fdaa841ceee7a2f366d1f5c64e825)(LPWSTR * reasonPhrase)

#### put_ReasonPhrase 

Set the ReasonPhrase property.

> public HRESULT [put_ReasonPhrase](#interface_i_web_view2_web_resource_response_1a6a9607f75b9899546adf005b9ef8a9ab)(LPCWSTR reasonPhrase)
