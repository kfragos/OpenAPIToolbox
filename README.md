## YAMl

**#** for **comments**

key: value

x: 100

y: another value

**lists or arrays:**

list1:

- Item1
- Item2

**Nesting items** : 2 spaces minimum

**Multiple lines** : \> or |

key: \>

Your long

string here.

# OpenAPI

Install OpenApi Extension on VsCode

Ctrl + Shift + P OpenAPI show preview with Swagger

## OpenApi Schema :

Specifies what the API expects

## OpenApi Components :

Hold a set of reusable objects/define objects

$ref to add reference to the component (object, parameter)

Object Inheritance:

allOf:

- ref: etc etc

## OpenApi Parameters :

Path or Query

- Add parameters to components in order to be reusable
- When I define a path ex: /v1/beer/{beer\_id} I have to give the same name and to the parameter

## OpenApi Requests:

- **operationId** : This is more for tools that generate code etc. MUST BE UNIQUE

- In a scheme where I designate a property as readonly (such as 'id') within a POST request, this property does not appear.

- I can put multiple response codes to a request

- (OpenAPI callbacks: example with beer and orders)

## OpenAPI security :

Check security schemes I have example with BasicAuth and JwtAuthToken

Anonymous authentication is implemented to grant access to individuals without authentication: Insert under responses security[] (empty array) and it overrides the securities.

## OpenAPI Code gen:

This is also accessible through SwaggerHub. Additionally, the OpenAPI Generator, which can be utilized through Docker and npm, is available. These tools can generate clients, servers, and documentation from OpenAPI.
