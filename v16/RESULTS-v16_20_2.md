## Adding property

|name|ops/sec|samples|
|-|-|-|
|Directly in the object|715,562,589|99|
|Using dot notation|707,512,682|96|
|Using define property (writable)|3,025,811|90|
|Using define property initialized (writable)|3,799,179|97|
|Using define property (getter)|1,578,554|91|


<details>
<summary>Environment</summary>

* __Machine:__ linux x64 | 2 vCPUs | 6.8GB Mem
* __Run:__ Sat Oct 14 2023 01:29:20 GMT+0000 (Coordinated Universal Time)
</details>

<!--
{"environment":{"platform":"linux","arch":"x64","cpus":2,"totalMemory":6.759757995605469},"benchmarks":[{"name":"Directly in the object","hz":715562589.0655619,"cycles":10,"stats":{"deviation":1.1690405338839232e-11,"mean":1.397501791291072e-9,"moe":2.3028626904833554e-12,"rme":0.16478423890647556,"sem":1.174929944124161e-12,"variance":1.366655769863608e-22}},{"name":"Using dot notation","hz":707512681.7339692,"cycles":9,"stats":{"deviation":1.0840254196873194e-10,"mean":1.4134022270091386e-9,"moe":2.1685024695929272e-11,"rme":1.534242997608427,"sem":1.1063788110167996e-11,"variance":1.1751111105282689e-20}},{"name":"Using define property (writable)","hz":3025810.6279707514,"cycles":7,"stats":{"deviation":4.640149720457776e-8,"mean":3.3048994895977553e-7,"moe":9.58664864321558e-9,"rme":2.9007383351263085,"sem":4.891147266946725e-9,"variance":2.153098942826438e-15}},{"name":"Using define property initialized (writable)","hz":3799178.8338798126,"cycles":5,"stats":{"deviation":3.5817155148783787e-9,"mean":2.6321477448819537e-7,"moe":7.127894980757441e-10,"rme":0.2708014774101183,"sem":3.636681112631348e-10,"variance":1.2828686029520489e-17}},{"name":"Using define property (getter)","hz":1578554.1322443557,"cycles":6,"stats":{"deviation":4.16501305633618e-8,"mean":6.334911040258218e-7,"moe":8.55759526214382e-9,"rme":1.3508627363131849,"sem":4.366120031706031e-9,"variance":1.7347333759450846e-15}}]}-->

## Array.append (number)

|type|amount|time elapsed|
|-|-|-|
array.push|10|0.015ms
new Array(length)|10|0.003ms
array.push|100|0.042ms
new Array(length)|100|0.019ms
array.push|1,000|0.141ms
new Array(length)|1,000|0.029ms
array.push|10,000|0.55ms
new Array(length)|10,000|0.269ms
array.push|1,000,000|56.198ms
new Array(length)|1,000,000|8.447ms
array.push|100,000,000|2,084.983ms
new Array(length)|100,000,000|5,219.92ms
## Array.append (string)

|type|amount|time elapsed|
|-|-|-|
array.push|10|0.009ms
new Array(length)|10|0.021ms
array.push|100|0.08ms
new Array(length)|100|0.013ms
array.push|1,000|0.056ms
new Array(length)|1,000|0.028ms
array.push|10,000|0.671ms
new Array(length)|10,000|4.456ms
array.push|1,000,000|375.576ms
new Array(length)|1,000,000|5.138ms
array.push|100,000,000|2,777.625ms
new Array(length)|100,000,000|5,808.457ms

## Array Creation

|name|ops/sec|samples|
|-|-|-|
|new Array|309|82|
|Array.from|14|39|


<details>
<summary>Environment</summary>

* __Machine:__ linux x64 | 2 vCPUs | 6.8GB Mem
* __Run:__ Sat Oct 14 2023 01:32:18 GMT+0000 (Coordinated Universal Time)
</details>

<!--
{"environment":{"platform":"linux","arch":"x64","cpus":2,"totalMemory":6.759754180908203},"benchmarks":[{"name":"new Array","hz":309.10688900703707,"cycles":2,"stats":{"deviation":0.00013984556761597103,"mean":0.003235126862466123,"moe":0.00003026898451540424,"rme":0.9356351636958783,"sem":0.000015443359446634818,"variance":1.9556782781833126e-8}},{"name":"Array.from","hz":14.201565360331818,"cycles":1,"stats":{"deviation":0.0004283131679299982,"mean":0.07041477292307692,"moe":0.00013442659378883618,"rme":0.19090680578589322,"sem":0.00006858499683103886,"variance":1.8345216982223081e-7}}]}-->

## Blob

|name|ops/sec|samples|
|-|-|-|
|new Blob (128)|3,127|86|
|new Blob (1024)|404|68|
|text (128)|25,481|73|
|text (1024)|13,868|81|
|arrayBuffer (128)|31,614|84|
|arrayBuffer (1024)|16,723|81|
|slice (0, 64)|66,234|77|
|slice (0, 512)|34,679|77|


<details>
<summary>Environment</summary>

* __Machine:__ linux x64 | 2 vCPUs | 6.8GB Mem
* __Run:__ Sat Oct 14 2023 01:34:20 GMT+0000 (Coordinated Universal Time)
</details>

<!--
{"environment":{"platform":"linux","arch":"x64","cpus":2,"totalMemory":6.759757995605469},"benchmarks":[{"name":"new Blob (128)","hz":3126.744005575866,"cycles":6,"stats":{"deviation":0.000031439340876798124,"mean":0.00031982151343912967,"moe":0.000006644774976289391,"rme":2.077651032551337,"sem":0.0000033901913144333626,"variance":9.884321547675094e-10}},{"name":"new Blob (1024)","hz":404.4911250885476,"cycles":2,"stats":{"deviation":0.00033366094034616357,"mean":0.0024722421283806632,"moe":0.00007930617142272603,"rme":3.2078642505243677,"sem":0.00004046233235853369,"variance":1.1132962311268611e-7}},{"name":"text (128)","hz":25480.94111149901,"cycles":4,"stats":{"deviation":0.0000033997972227330294,"mean":0.00003924501829128757,"moe":7.799156876784691e-7,"rme":1.9872985709669326,"sem":3.9791616718289244e-7,"variance":1.155862115570322e-11}},{"name":"text (1024)","hz":13868.415567497503,"cycles":3,"stats":{"deviation":0.000007862684691496671,"mean":0.00007210629037852273,"moe":0.0000017123179994814972,"rme":2.3747137600515376,"sem":8.73631632388519e-7,"variance":6.18218105578961e-11}},{"name":"arrayBuffer (128)","hz":31614.166932118387,"cycles":3,"stats":{"deviation":0.0000012615111281307256,"mean":0.00003163138861597048,"moe":2.6977861095211534e-7,"rme":0.8528826041355196,"sem":1.376421484449568e-7,"variance":1.5914103263976561e-12}},{"name":"arrayBuffer (1024)","hz":16722.745295536573,"cycles":4,"stats":{"deviation":0.000004248449429598712,"mean":0.000059798793937674067,"moe":9.252178757792751e-7,"rme":1.5472182879534213,"sem":4.7204993662207913e-7,"variance":1.8049322555857625e-11}},{"name":"slice (0, 64)","hz":66234.18901099933,"cycles":3,"stats":{"deviation":0.000003425843950078477,"mean":0.000015097942843897926,"moe":7.652058567669445e-7,"rme":5.068278934942548,"sem":3.9041115141170635e-7,"variance":1.1736406770289304e-11}},{"name":"slice (0, 512)","hz":34678.88512550235,"cycles":3,"stats":{"deviation":0.000012298072114252925,"mean":0.00002883599044147514,"moe":0.0000027469309594656247,"rme":9.526050319099433,"sem":0.0000014014953874824616,"variance":1.5124257772736542e-10}}]}-->

## Comparison using `instanceof`

|name|ops/sec|samples|
|-|-|-|
|[True conditional] Using instanceof only|152,276|53|
|[True conditional] Using constructor name|121,115|87|
|[True conditional] Check if property is valid then instanceof |119,631|88|
|[False conditional] Using instanceof only|765,612,200|88|
|[False conditional] Using constructor name|769,955,036|91|
|[False conditional] Check if property is valid then instanceof |767,503,512|91|


<details>
<summary>Environment</summary>

* __Machine:__ linux x64 | 2 vCPUs | 6.8GB Mem
* __Run:__ Sat Oct 14 2023 01:38:42 GMT+0000 (Coordinated Universal Time)
</details>

<!--
{"environment":{"platform":"linux","arch":"x64","cpus":2,"totalMemory":6.7597503662109375},"benchmarks":[{"name":"[True conditional] Using instanceof only","hz":152275.96789878982,"cycles":4,"stats":{"deviation":0.0000013076778562672077,"mean":0.000006567024421507205,"moe":3.5206180088814963e-7,"rme":5.3610551490434,"sem":1.7962336780007635e-7,"variance":1.7100213757715998e-12}},{"name":"[True conditional] Using constructor name","hz":121114.83506010505,"cycles":3,"stats":{"deviation":4.3137333094554874e-7,"mean":0.000008256626857508703,"moe":9.064622803908522e-8,"rme":1.0978602957774477,"sem":4.624807553014552e-8,"variance":1.8608295065105792e-13}},{"name":"[True conditional] Check if property is valid then instanceof ","hz":119631.42934044593,"cycles":3,"stats":{"deviation":4.5244565413389634e-7,"mean":0.000008359007373841618,"moe":9.453250282186286e-8,"rme":1.1309058431709191,"sem":4.8230868786664725e-8,"variance":2.0470706994464936e-13}},{"name":"[False conditional] Using instanceof only","hz":765612199.5795503,"cycles":6,"stats":{"deviation":5.289607340226677e-11,"mean":1.3061442862968589e-9,"moe":1.1051931126926981e-11,"rme":0.8461493299688264,"sem":5.638740370881113e-12,"variance":2.7979945813779935e-21}},{"name":"[False conditional] Using constructor name","hz":769955035.8582311,"cycles":6,"stats":{"deviation":4.348120671110329e-11,"mean":1.2987771407785509e-9,"moe":8.933815176813693e-12,"rme":0.6878635984814396,"sem":4.558068967762089e-12,"variance":1.8906153370536933e-21}},{"name":"[False conditional] Check if property is valid then instanceof ","hz":767503511.8090057,"cycles":6,"stats":{"deviation":5.3418335942421745e-11,"mean":1.3029256343635485e-9,"moe":1.0975535787986199e-11,"rme":0.8423762261264831,"sem":5.599763157135816e-12,"variance":2.8535186148574267e-21}}]}-->

## Crypto Verify

|name|ops/sec|samples|
|-|-|-|
|crypto.createVerify('RSA-SHA256')|21,085|93|
|crypto.verify('RSA-SHA256')|20,619|94|


<details>
<summary>Environment</summary>

* __Machine:__ linux x64 | 2 vCPUs | 6.8GB Mem
* __Run:__ Sat Oct 14 2023 01:40:19 GMT+0000 (Coordinated Universal Time)
</details>

<!--
{"environment":{"platform":"linux","arch":"x64","cpus":2,"totalMemory":6.759754180908203},"benchmarks":[{"name":"crypto.createVerify('RSA-SHA256')","hz":21085.356952870647,"cycles":5,"stats":{"deviation":0.000002095209486609373,"mean":0.00004742627797267885,"moe":4.258356814791513e-7,"rme":0.8978897347256833,"sem":2.1726310279548536e-7,"variance":4.389902792777913e-12}},{"name":"crypto.verify('RSA-SHA256')","hz":20619.210347696706,"cycles":4,"stats":{"deviation":0.0000040226345233803595,"mean":0.00004849846250837177,"moe":8.132100198163291e-7,"rme":1.6767748455447495,"sem":4.149030713348618e-7,"variance":1.618158850869153e-11}}]}-->