
<a name="paths"></a>
## Paths

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


#### Parameters

|Type|Name|Description|Schema|Default|
|---|---|---|---|---|
|**Query**|**coinUnit**  <br>*optional*|币种单位，默认为主币SLU|string|`"SLU"`|


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
|**Path**|**address**  <br>*optional*|地址|string|`"SLUjc1JSj9oqYkq7fdUFZaGeG8uisYVRihbm"`|
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


<a name="coinbaseusingget"></a>
### 查询提币地址余额
```
GET /rpc/coinBase
```


#### Parameters

|Type|Name|Description|Schema|Default|
|---|---|---|---|---|
|**Query**|**coinUnit**  <br>*optional*|币种单位，默认为主币SLU|string|`"SLU"`|


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
|**Query**|**address**  <br>*required*|转出地址(to)|string|`"SLUjc1JSj9oqYkq7fdUFZaGeG8uisYVRihbm"`|
|**Query**|**amount**  <br>*required*|金额|string|`"10"`|
|**Query**|**coinUnit**  <br>*optional*|币种单位，默认为主币SLU|string|`"SLU"`|


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
|**Query**|**address**  <br>*optional*|地址|string|`"SLUjc1JSj9oqYkq7fdUFZaGeG8uisYVRihbm"`|


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



