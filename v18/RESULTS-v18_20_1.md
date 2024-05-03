## Adding property

|name|ops/sec|samples|
|-|-|-|
|Directly in the object|912,194,930|97|
|Using dot notation|909,618,119|96|
|Using define property (writable)|4,597,368|96|
|Using define property initialized (writable)|6,333,403|92|
|Using define property (getter)|2,568,937|95|


<details>
<summary>Environment</summary>

* __Machine:__ linux x64 | 4 vCPUs | 15.2GB Mem
* __Run:__ Fri May 03 2024 20:13:48 GMT+0000 (Coordinated Universal Time)
</details>

<!--
{"environment":{"platform":"linux","arch":"x64","cpus":4,"totalMemory":15.245216369628906},"benchmarks":[{"name":"Directly in the object","opsSec":912194930.0470653,"samples":6},{"name":"Using dot notation","opsSec":909618119.3453944,"samples":6},{"name":"Using define property (writable)","opsSec":4597367.817724662,"samples":6},{"name":"Using define property initialized (writable)","opsSec":6333403.29427827,"samples":5},{"name":"Using define property (getter)","opsSec":2568937.146117732,"samples":6}]}-->

## Array.append (number)

|type|amount|time elapsed|
|-|-|-|
array.push|10|0.011ms
new Array(length)|10|0.002ms
array.push|100|0.087ms
new Array(length)|100|0.007ms
array.push|1,000|0.036ms
new Array(length)|1,000|0.02ms
array.push|10,000|0.277ms
new Array(length)|10,000|0.17ms
array.push|1,000,000|27.374ms
new Array(length)|1,000,000|15.675ms
array.push|100,000,000|2,097.062ms
new Array(length)|100,000,000|4,242.198ms
## Array.append (string)

|type|amount|time elapsed|
|-|-|-|
array.push|10|0.007ms
new Array(length)|10|0.017ms
array.push|100|0.072ms
new Array(length)|100|0.009ms
array.push|1,000|0.035ms
new Array(length)|1,000|0.017ms
array.push|10,000|0.491ms
new Array(length)|10,000|3.087ms
array.push|1,000,000|255.431ms
new Array(length)|1,000,000|4.631ms
array.push|100,000,000|2,612.482ms
new Array(length)|100,000,000|4,647.079ms

## Array Creation

|name|ops/sec|samples|
|-|-|-|
|new Array|213|90|
|Array.from|22|41|


<details>
<summary>Environment</summary>

* __Machine:__ linux x64 | 4 vCPUs | 15.2GB Mem
* __Run:__ Fri May 03 2024 20:30:49 GMT+0000 (Coordinated Universal Time)
</details>

<!--
{"environment":{"platform":"linux","arch":"x64","cpus":4,"totalMemory":15.245216369628906},"benchmarks":[{"name":"new Array","opsSec":213.32984953765558,"samples":2},{"name":"Array.from","opsSec":22.227805136064536,"samples":2}]}-->

## async function vs function

|name|ops/sec|samples|
|-|-|-|
|function|911,584,628|98|
|[async] async function|17,949,683|88|
|[async] function|375,729|38|


<details>
<summary>Environment</summary>

* __Machine:__ linux x64 | 4 vCPUs | 15.2GB Mem
* __Run:__ Fri May 03 2024 20:35:48 GMT+0000 (Coordinated Universal Time)
</details>

<!--
{"environment":{"platform":"linux","arch":"x64","cpus":4,"totalMemory":15.245216369628906},"benchmarks":[{"name":"function","opsSec":911584628.1527041,"samples":6},{"name":"[async] async function","opsSec":17949682.752275303,"samples":6},{"name":"[async] function","opsSec":375729.40531532036,"samples":3}]}-->

## Blob

|name|ops/sec|samples|
|-|-|-|
|new Blob (128)|5,730|92|
|new Blob (1024)|742|79|
|text (128)|38,086|68|
|text (1024)|25,276|78|
|arrayBuffer (128)|42,855|76|
|arrayBuffer (1024)|25,457|80|
|slice (0, 64)|95,881|81|
|slice (0, 512)|46,825|76|


<details>
<summary>Environment</summary>

* __Machine:__ linux x64 | 4 vCPUs | 15.2GB Mem
* __Run:__ Fri May 03 2024 20:44:42 GMT+0000 (Coordinated Universal Time)
</details>

<!--
{"environment":{"platform":"linux","arch":"x64","cpus":4,"totalMemory":15.245216369628906},"benchmarks":[{"name":"new Blob (128)","opsSec":5729.898676544437,"samples":5},{"name":"new Blob (1024)","opsSec":742.4077273862412,"samples":2},{"name":"text (128)","opsSec":38085.552240823345,"samples":5},{"name":"text (1024)","opsSec":25276.10925766244,"samples":5},{"name":"arrayBuffer (128)","opsSec":42855.069853772584,"samples":5},{"name":"arrayBuffer (1024)","opsSec":25457.269957829416,"samples":3},{"name":"slice (0, 64)","opsSec":95881.17814201184,"samples":4},{"name":"slice (0, 512)","opsSec":46825.3703275163,"samples":3}]}-->

## Comparison using `instanceof`

|name|ops/sec|samples|
|-|-|-|
|[True conditional] Using instanceof only|290,693|54|
|[True conditional] Using constructor name|228,188|94|
|[True conditional] Check if property is valid then instanceof |230,936|93|
|[False conditional] Using instanceof only|910,712,844|94|
|[False conditional] Using constructor name|910,964,236|97|
|[False conditional] Check if property is valid then instanceof |912,078,083|100|


<details>
<summary>Environment</summary>

* __Machine:__ linux x64 | 4 vCPUs | 15.2GB Mem
* __Run:__ Fri May 03 2024 20:56:53 GMT+0000 (Coordinated Universal Time)
</details>

<!--
{"environment":{"platform":"linux","arch":"x64","cpus":4,"totalMemory":15.245216369628906},"benchmarks":[{"name":"[True conditional] Using instanceof only","opsSec":290692.7411382375,"samples":3},{"name":"[True conditional] Using constructor name","opsSec":228188.32469293973,"samples":3},{"name":"[True conditional] Check if property is valid then instanceof ","opsSec":230936.40175932803,"samples":3},{"name":"[False conditional] Using instanceof only","opsSec":910712843.8050499,"samples":7},{"name":"[False conditional] Using constructor name","opsSec":910964236.0701406,"samples":6},{"name":"[False conditional] Check if property is valid then instanceof ","opsSec":912078082.58517,"samples":7}]}-->

## Crypto Verify

|name|ops/sec|samples|
|-|-|-|
|crypto.createVerify('RSA-SHA256')|7,246|91|
|crypto.verify('RSA-SHA256')|7,288|97|


<details>
<summary>Environment</summary>

* __Machine:__ linux x64 | 4 vCPUs | 15.2GB Mem
* __Run:__ Fri May 03 2024 21:07:00 GMT+0000 (Coordinated Universal Time)
</details>

<!--
{"environment":{"platform":"linux","arch":"x64","cpus":4,"totalMemory":15.245216369628906},"benchmarks":[{"name":"crypto.createVerify('RSA-SHA256')","opsSec":7245.855510486057,"samples":3},{"name":"crypto.verify('RSA-SHA256')","opsSec":7288.302139348693,"samples":3}]}-->

## Date format MM/DD/YYYY

|name|ops/sec|samples|
|-|-|-|
|Intl.DateTimeFormat().format(Date.now())|15,962|83|
|Intl.DateTimeFormat().format(new Date())|15,022|79|
|Intl.DateTimeFormat(undefined, twoDigitsLocaleOptions).format(Date.now())|16,990|76|
|Intl.DateTimeFormat(undefined, twoDigitsLocaleOptions).format(new Date())|17,338|77|
|Reusing Intl.DateTimeFormat()|797,134|98|
|Date.toLocaleDateString()|820,734|99|
|Date.toLocaleDateString(undefined, twoDigitsLocaleOptions)|17,420|79|
|Format using date.get*|0|0|


<details>
<summary>Environment</summary>

* __Machine:__ linux x64 | 4 vCPUs | 15.2GB Mem
* __Run:__ Fri May 03 2024 21:25:17 GMT+0000 (Coordinated Universal Time)
</details>

<!--
{"environment":{"platform":"linux","arch":"x64","cpus":4,"totalMemory":15.245216369628906},"benchmarks":[{"name":"Intl.DateTimeFormat().format(Date.now())","opsSec":15962.314598180494,"samples":3},{"name":"Intl.DateTimeFormat().format(new Date())","opsSec":15021.790156912846,"samples":3},{"name":"Intl.DateTimeFormat(undefined, twoDigitsLocaleOptions).format(Date.now())","opsSec":16989.986566069107,"samples":4},{"name":"Intl.DateTimeFormat(undefined, twoDigitsLocaleOptions).format(new Date())","opsSec":17337.743287350593,"samples":3},{"name":"Reusing Intl.DateTimeFormat()","opsSec":797133.5746031706,"samples":5},{"name":"Date.toLocaleDateString()","opsSec":820734.2853009058,"samples":5},{"name":"Date.toLocaleDateString(undefined, twoDigitsLocaleOptions)","opsSec":17420.206371605826,"samples":4},{"name":"Format using date.get*","opsSec":0,"samples":0}]}-->