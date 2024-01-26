# HTTP / HTTPS CheatSheet

---
## **UNDER CONSTRUCTION**
---

## Table of Contents
- [Introduction](#introduction)
- [HTTP Methods](#http-methods)
- [HTTP Status Codes](#http-status-codes)
- [HTTP Headers](#http-headers)
- [HTTP Cookies](#http-cookies)
- [HTTP Caching](#http-caching)
- [HTTP Security](#http-security)
    - [HTTPS](#https)
    - [Cross-Site Scripting (XSS) prevention](#cross-site-scripting-xss-prevention)
    - [Cross-Origin Resource Sharing (CORS) restrictions](#cross-origin-resource-sharing-cors-restrictions)
    - [Content Security Policy (CSP) to mitigate code injection attacks](#content-security-policy-csp-to-mitigate-code-injection-attacks)
    - [HTTP Strict Transport Security (HSTS) to enforce secure connections](#http-strict-transport-security-hsts-to-enforce-secure-connections)
    - [Public Key Pinning (HPKP) to prevent man-in-the-middle attacks](#public-key-pinning-hpkp-to-prevent-man-in-the-middle-attacks)

## Introduction
HTTP (Hypertext Transfer Protocol) is an application protocol for distributed, collaborative, hypermedia information systems. It is the foundation of data communication on the World Wide Web.

## HTTP Methods
HTTP defines several methods, also known as verbs, to indicate the desired action to be performed on a resource. Some commonly used methods include:
- GET: Retrieve a resource
- POST: Submit data to be processed
- PUT: Update a resource
- DELETE: Remove a resource
- HEAD: Retrieve the headers of a resource
- OPTIONS: Retrieve the available methods and headers for a resource

## HTTP Status Codes
HTTP status codes are three-digit numbers that indicate the outcome of an HTTP request. Some common status codes include:
- 100 Continue: The server has received the initial part of the request and expects the client to continue with the rest of the request
- 101 Switching Protocols: The server is switching protocols according to the Upgrade header field sent by the client
- 200 OK: The request was successful
- 201 Created: The request has been fulfilled and a new resource has been created
- 204 No Content: The server has successfully fulfilled the request, but there is no additional content to send in the response
- 300 Multiple Choices: The requested resource has multiple representations, each with its own specific location
- 301 Moved Permanently: The requested resource has been permanently moved to a new location
- 302 Found: The requested resource has been temporarily moved to a different location
- 400 Bad Request: The server cannot process the request due to a client error
- 401 Unauthorized: The request requires user authentication
- 403 Forbidden: The server understood the request, but refuses to authorize it
- 404 Not Found: The requested resource could not be found
- 500 Internal Server Error: An unexpected error occurred on the server

## HTTP Headers
HTTP headers provide additional information about the request or response. Some commonly used headers include:
- Accept: Specifies the media types that are acceptable for the response
- Accept-Encoding: Specifies the content encoding that the client can understand
- Authorization: Provides authentication credentials
- Cache-Control: Specifies directives for caching mechanisms in both requests and responses
- Content-Type: Specifies the media type of the resource
- User-Agent: Identifies the client making the request
- Content-Length: Specifies the length of the request or response body
- Location: Specifies the URL of a resource that has been moved or created
- Set-Cookie: Sets a cookie on the client-side

## HTTP Cookies
HTTP cookies are small pieces of data stored on the client-side by the web browser. They are commonly used for session management and tracking user preferences.

## HTTP Caching
HTTP caching allows the client to store a copy of a resource for future use. This can improve performance and reduce server load.

## HTTP Security
HTTP can be secured using various mechanisms, such as:

### HTTPS
HTTPS (HTTP over SSL/TLS) is a secure version of HTTP that encrypts the communication between the client and the server.

### Cross-Site Scripting (XSS) prevention
Cross-Site Scripting (XSS) is a security vulnerability that allows attackers to inject malicious scripts into web pages viewed by other users. Preventing XSS attacks is important to protect user data and prevent unauthorized actions.

### Cross-Origin Resource Sharing (CORS) restrictions
Cross-Origin Resource Sharing (CORS) is a mechanism that allows restricted resources on a web page to be requested from another domain outside the domain from which the resource originated. CORS restrictions help prevent unauthorized access to sensitive data.

### Content Security Policy (CSP) to mitigate code injection attacks
Content Security Policy (CSP) is a security mechanism that allows web developers to control the types of content that can be loaded on their web pages. It helps mitigate code injection attacks, such as cross-site scripting (XSS) and clickjacking.

### HTTP Strict Transport Security (HSTS) to enforce secure connections
HTTP Strict Transport Security (HSTS) is a security mechanism that allows a website to specify that it should only be accessed over a secure connection (HTTPS). It helps protect against downgrade attacks and ensures that users always connect securely to the website.

### Public Key Pinning (HPKP) to prevent man-in-the-middle attacks
Public Key Pinning (HPKP) is a security mechanism that allows a website to specify which public keys should be used to authenticate the server's SSL/TLS certificate. It helps prevent man-in-the-middle attacks by ensuring that the client only accepts valid certificates from trusted sources.
