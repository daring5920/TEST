
<a name="paths"></a>
## Paths

<a name="hiusingpost"></a>
### hi
```
POST /info
```


#### Responses

|HTTP Code|Description|Schema|
|---|---|---|
|**200**|OK|string|
|**201**|Created|No Content|
|**401**|Unauthorized|No Content|
|**403**|Forbidden|No Content|
|**404**|Not Found|No Content|


#### Consumes

* `application/json`


#### Produces

* `\*/*`


#### Tags

* report-controller


<a name="hiusingget"></a>
### hi
```
GET /info
```


#### Responses

|HTTP Code|Description|Schema|
|---|---|---|
|**200**|OK|string|
|**401**|Unauthorized|No Content|
|**403**|Forbidden|No Content|
|**404**|Not Found|No Content|


#### Consumes

* `application/json`


#### Produces

* `\*/*`


#### Tags

* report-controller


<a name="hiusingput"></a>
### hi
```
PUT /info
```


#### Responses

|HTTP Code|Description|Schema|
|---|---|---|
|**200**|OK|string|
|**201**|Created|No Content|
|**401**|Unauthorized|No Content|
|**403**|Forbidden|No Content|
|**404**|Not Found|No Content|


#### Consumes

* `application/json`


#### Produces

* `\*/*`


#### Tags

* report-controller


<a name="hiusingdelete"></a>
### hi
```
DELETE /info
```


#### Responses

|HTTP Code|Description|Schema|
|---|---|---|
|**200**|OK|string|
|**204**|No Content|No Content|
|**401**|Unauthorized|No Content|
|**403**|Forbidden|No Content|


#### Consumes

* `application/json`


#### Produces

* `\*/*`


#### Tags

* report-controller


<a name="hiusingpatch"></a>
### hi
```
PATCH /info
```


#### Responses

|HTTP Code|Description|Schema|
|---|---|---|
|**200**|OK|string|
|**204**|No Content|No Content|
|**401**|Unauthorized|No Content|
|**403**|Forbidden|No Content|


#### Consumes

* `application/json`


#### Produces

* `\*/*`


#### Tags

* report-controller


<a name="hiusinghead"></a>
### hi
```
HEAD /info
```


#### Responses

|HTTP Code|Description|Schema|
|---|---|---|
|**200**|OK|string|
|**204**|No Content|No Content|
|**401**|Unauthorized|No Content|
|**403**|Forbidden|No Content|


#### Consumes

* `application/json`


#### Produces

* `\*/*`


#### Tags

* report-controller


<a name="hiusingoptions"></a>
### hi
```
OPTIONS /info
```


#### Responses

|HTTP Code|Description|Schema|
|---|---|---|
|**200**|OK|string|
|**204**|No Content|No Content|
|**401**|Unauthorized|No Content|
|**403**|Forbidden|No Content|


#### Consumes

* `application/json`


#### Produces

* `\*/*`


#### Tags

* report-controller


<a name="getnewaddressusingget"></a>
### 新增钱包地址
```
GET /rpc/address/{account}
```


#### Parameters

|Type|Name|Description|Schema|Default|
|---|---|---|---|---|
|**Path**|**account**  <br>*required*|地址别名|string|`"test"`|


#### Responses

|HTTP Code|Description|Schema|
|---|---|---|
|**200**|OK|[MessageResult](#messageresult)|
|**401**|Unauthorized|No Content|
|**403**|Forbidden|No Content|
|**404**|Not Found|No Content|


#### Consumes

* `application/json`


#### Produces

* `\*/*`


#### Tags

* 接口操作


<a name="balanceusingget"></a>
### 查询钱包余额
```
GET /rpc/balance
```


#### Responses

|HTTP Code|Description|Schema|
|---|---|---|
|**200**|OK|[MessageResult](#messageresult)|
|**401**|Unauthorized|No Content|
|**403**|Forbidden|No Content|
|**404**|Not Found|No Content|


#### Consumes

* `application/json`


#### Produces

* `\*/*`


#### Tags

* 接口操作


<a name="addressbalanceusingget"></a>
### 查询地址余额
```
GET /rpc/balance/{address}
```


#### Parameters

|Type|Name|Description|Schema|Default|
|---|---|---|---|---|
|**Path**|**address**  <br>*optional*|地址|string|`"12gXC6KDsy8my7xUtCYgNH6oUj1JAJ9LZn"`|
|**Body**|**coinUnit**  <br>*optional*|coinUnit|string||


#### Responses

|HTTP Code|Description|Schema|
|---|---|---|
|**200**|OK|[MessageResult](#messageresult)|
|**401**|Unauthorized|No Content|
|**403**|Forbidden|No Content|
|**404**|Not Found|No Content|


#### Consumes

* `application/json`


#### Produces

* `\*/*`


#### Tags

* 接口操作


<a name="getheightusingget"></a>
### getHeight
```
GET /rpc/height
```


#### Responses

|HTTP Code|Description|Schema|
|---|---|---|
|**200**|OK|[MessageResult](#messageresult)|
|**401**|Unauthorized|No Content|
|**403**|Forbidden|No Content|
|**404**|Not Found|No Content|


#### Consumes

* `application/json`


#### Produces

* `\*/*`


#### Tags

* 接口操作


<a name="gettransationusingget"></a>
### 查询交易详情
```
GET /rpc/transaction
```


#### Parameters

|Type|Name|Description|Schema|Default|
|---|---|---|---|---|
|**Query**|**txid**  <br>*optional*|交易id|string|`"4c9efcac560aea8f6b8fd4d302484d4036514436c01c4435b2b6d9d611478a26"`|


#### Responses

|HTTP Code|Description|Schema|
|---|---|---|
|**200**|OK|[MessageResult](#messageresult)|
|**401**|Unauthorized|No Content|
|**403**|Forbidden|No Content|
|**404**|Not Found|No Content|


#### Consumes

* `application/json`


#### Produces

* `\*/*`


#### Tags

* 接口操作


<a name="withdrawusingget"></a>
### 转账
```
GET /rpc/transfer
```


#### Parameters

|Type|Name|Description|Schema|Default|
|---|---|---|---|---|
|**Query**|**address**  <br>*required*|转出地址|string|`"12gXC6KDsy8my7xUtCYgNH6oUj1JAJ9LZn"`|
|**Query**|**amount**  <br>*required*|金额|string|`"10"`|


#### Responses

|HTTP Code|Description|Schema|
|---|---|---|
|**200**|OK|[MessageResult](#messageresult)|
|**401**|Unauthorized|No Content|
|**403**|Forbidden|No Content|
|**404**|Not Found|No Content|


#### Consumes

* `application/json`


#### Produces

* `\*/*`


#### Tags

* 接口操作


<a name="vailidateusingget"></a>
### 校验地址
```
GET /rpc/validate
```


#### Parameters

|Type|Name|Description|Schema|Default|
|---|---|---|---|---|
|**Query**|**address**  <br>*optional*|地址|string|`"12gXC6KDsy8my7xUtCYgNH6oUj1JAJ9LZn"`|


#### Responses

|HTTP Code|Description|Schema|
|---|---|---|
|**200**|OK|[MessageResult](#messageresult)|
|**401**|Unauthorized|No Content|
|**403**|Forbidden|No Content|
|**404**|Not Found|No Content|


#### Consumes

* `application/json`


#### Produces

* `\*/*`


#### Tags

* 接口操作


