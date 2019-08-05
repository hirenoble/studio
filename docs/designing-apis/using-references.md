---
tags: []
---

# Using References

![]()

## What 

OpenAPI and JSON Schema both let you "reference" other files, which allows for cleaner and more organized API descriptions. Instead of having everything in the same giant file (which is prone to Git conflicts), you can reuse common parts of your description document. Some common use cases are as follows:

* De-duplicating common structures like responses or shared parameters
* Using models alone for contract testing
* Using models alone for client-side and server-side validation

## How 
1. Select an **endpoint** or **model** 
2. Create a **request body** and/or **response body**
3. Within the JSON Schema Viewer, add a new property by clicking the + button or modify an existing property by selecting the property 
4. Select **$ref** in the proceeding window 
5. Select a **$ref target** 
6. Select the file you want to reference 
