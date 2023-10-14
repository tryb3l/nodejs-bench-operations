## Adding property

|name|ops/sec|samples|
|-|-|-|
|Directly in the object|660,166,844|87|
|Using dot notation|635,660,830|86|
|Using define property (writable)|2,537,449|91|
|Using define property initialized (writable)|3,346,301|88|
|Using define property (getter)|1,389,947|83|


<details>
<summary>Environment</summary>

* __Machine:__ linux x64 | 2 vCPUs | 6.8GB Mem
* __Run:__ Sat Oct 14 2023 01:29:21 GMT+0000 (Coordinated Universal Time)
</details>

<!--
{"environment":{"platform":"linux","arch":"x64","cpus":2,"totalMemory":6.759757995605469},"benchmarks":[{"name":"Directly in the object","hz":660166843.8399377,"cycles":8,"stats":{"deviation":7.336904156047068e-11,"mean":1.5147685911994353e-9,"moe":1.5417334348699085e-11,"rme":1.0178012957405735,"sem":7.865986912601574e-12,"variance":5.383016259502074e-21}},{"name":"Using dot notation","hz":635660830.2048651,"cycles":6,"stats":{"deviation":9.766837172523297e-11,"mean":1.5731659911744337e-9,"moe":2.0642428699696482e-11,"rme":1.3121583364693798,"sem":1.0531851377396164e-11,"variance":9.539110835458288e-21}},{"name":"Using define property (writable)","hz":2537448.8167411312,"cycles":5,"stats":{"deviation":2.9376520371421074e-8,"mean":3.940966191721294e-7,"moe":6.035812328758596e-9,"rme":1.531556485168003,"sem":3.0794960861013246e-9,"variance":8.629799491325174e-16}},{"name":"Using define property initialized (writable)","hz":3346300.9773303135,"cycles":6,"stats":{"deviation":1.236880943678366e-8,"mean":2.988374347599188e-7,"moe":2.5842982517405445e-9,"rme":0.8647839765512404,"sem":1.3185195161941553e-9,"variance":1.5298744688346853e-16}},{"name":"Using define property (getter)","hz":1389947.2769589713,"cycles":4,"stats":{"deviation":6.097119456482759e-8,"mean":7.194517494130234e-7,"moe":1.3117217782107631e-8,"rme":1.82322411375183,"sem":6.69245805209573e-9,"variance":3.7174865666620615e-15}}]}-->

## Array.append (number)

|type|amount|time elapsed|
|-|-|-|
array.push|10|0.011ms
new Array(length)|10|0.003ms
array.push|100|0.044ms
new Array(length)|100|0.014ms
array.push|1,000|0.069ms
new Array(length)|1,000|0.034ms
array.push|10,000|0.466ms
new Array(length)|10,000|0.245ms
array.push|1,000,000|45.491ms
new Array(length)|1,000,000|7.596ms
array.push|100,000,000|2,151.642ms
new Array(length)|100,000,000|4,947.681ms
## Array.append (string)

|type|amount|time elapsed|
|-|-|-|
array.push|10|0.009ms
new Array(length)|10|0.042ms
array.push|100|0.018ms
new Array(length)|100|0.013ms
array.push|1,000|0.068ms
new Array(length)|1,000|0.037ms
array.push|10,000|0.746ms
new Array(length)|10,000|4.445ms
array.push|1,000,000|377.83ms
new Array(length)|1,000,000|4.587ms
array.push|100,000,000|2,876.191ms
new Array(length)|100,000,000|5,670.299ms

## Array Creation

|name|ops/sec|samples|
|-|-|-|
|new Array|246|80|
|Array.from|12|34|


<details>
<summary>Environment</summary>

* __Machine:__ linux x64 | 2 vCPUs | 6.8GB Mem
* __Run:__ Sat Oct 14 2023 01:32:19 GMT+0000 (Coordinated Universal Time)
</details>

<!--
{"environment":{"platform":"linux","arch":"x64","cpus":2,"totalMemory":6.759757995605469},"benchmarks":[{"name":"new Array","hz":245.9124393738427,"cycles":3,"stats":{"deviation":0.0004803697556465623,"mean":0.004066488066021634,"moe":0.00010526566394014633,"rme":2.5886136201828536,"sem":0.00005370697139803384,"variance":2.3075510213993797e-7}},{"name":"Array.from","hz":11.852383189800479,"cycles":1,"stats":{"deviation":0.0038323257399697237,"mean":0.0843712175,"moe":0.0012881873467316507,"rme":1.5268090053715897,"sem":0.0006572384422100259,"variance":0.00001468672057723449}}]}-->

## Blob

|name|ops/sec|samples|
|-|-|-|
|new Blob (128)|3,234|85|
|new Blob (1024)|412|71|
|text (128)|30,628|84|
|text (1024)|20,449|86|
|arrayBuffer (128)|32,042|64|
|arrayBuffer (1024)|21,238|79|
|slice (0, 64)|58,269|77|
|slice (0, 512)|34,106|79|


<details>
<summary>Environment</summary>

* __Machine:__ linux x64 | 2 vCPUs | 6.8GB Mem
* __Run:__ Sat Oct 14 2023 01:34:19 GMT+0000 (Coordinated Universal Time)
</details>

<!--
{"environment":{"platform":"linux","arch":"x64","cpus":2,"totalMemory":6.759757995605469},"benchmarks":[{"name":"new Blob (128)","hz":3234.219257260789,"cycles":3,"stats":{"deviation":0.000027354775063951942,"mean":0.00030919363235965225,"moe":0.000005815402200586465,"rme":1.8808285785853516,"sem":0.0000029670419390747273,"variance":7.48283718799407e-10}},{"name":"new Blob (1024)","hz":412.46823434187644,"cycles":2,"stats":{"deviation":0.00036303756383781994,"mean":0.002424429123846528,"moe":0.00008444587911162854,"rme":3.4831242654620973,"sem":0.00004308463219981048,"variance":1.3179627275729918e-7}},{"name":"text (128)","hz":30627.609565946004,"cycles":4,"stats":{"deviation":0.0000019351977194077015,"mean":0.000032650279083871844,"moe":4.1384886824827953e-7,"rme":1.2675201556016933,"sem":2.111473817593263e-7,"variance":3.744990213200769e-12}},{"name":"text (1024)","hz":20449.178926076707,"cycles":3,"stats":{"deviation":0.00000580909428751391,"mean":0.00004890171892059706,"moe":0.0000012277650637728391,"rme":2.5106787468276766,"sem":6.264107468228771e-7,"variance":3.3745576441226745e-11}},{"name":"arrayBuffer (128)","hz":32042.072587258903,"cycles":4,"stats":{"deviation":0.0000016616413247973552,"mean":0.000031208967437319785,"moe":4.07102124575352e-7,"rme":1.3044395826070745,"sem":2.077051655996694e-7,"variance":2.7610518922743097e-12}},{"name":"arrayBuffer (1024)","hz":21237.649555655036,"cycles":4,"stats":{"deviation":0.000004693653750724436,"mean":0.00004708618989965986,"moe":0.0000010350315170309185,"rme":2.1981636637760644,"sem":5.280773046076115e-7,"variance":2.203038553168956e-11}},{"name":"slice (0, 64)","hz":58268.5888992351,"cycles":3,"stats":{"deviation":0.000004387213331200711,"mean":0.000017161905220140437,"moe":9.799399461390813e-7,"rme":5.709971786751672,"sem":4.999693602750414e-7,"variance":1.9247640813465237e-11}},{"name":"slice (0, 512)","hz":34106.32133996915,"cycles":4,"stats":{"deviation":0.000012751088416427317,"mean":0.000029320077941918094,"moe":0.0000028118346789882284,"rme":9.590133711644153,"sem":0.000001434609530096035,"variance":1.625902558035469e-10}}]}-->

## Comparison using `instanceof`

|name|ops/sec|samples|
|-|-|-|
|[True conditional] Using instanceof only|186,431|56|
|[True conditional] Using constructor name|147,039|96|
|[True conditional] Check if property is valid then instanceof |145,369|89|
|[False conditional] Using instanceof only|711,546,374|99|
|[False conditional] Using constructor name|711,012,360|97|
|[False conditional] Check if property is valid then instanceof |710,393,528|94|


<details>
<summary>Environment</summary>

* __Machine:__ linux x64 | 2 vCPUs | 6.8GB Mem
* __Run:__ Sat Oct 14 2023 01:38:44 GMT+0000 (Coordinated Universal Time)
</details>

<!--
{"environment":{"platform":"linux","arch":"x64","cpus":2,"totalMemory":6.759757995605469},"benchmarks":[{"name":"[True conditional] Using instanceof only","hz":186431.22694752403,"cycles":4,"stats":{"deviation":0.000001067643555158578,"mean":0.00000536390826994598,"moe":2.79632947622048e-7,"rme":5.213231352013113,"sem":1.4266987123573877e-7,"variance":1.1398627608716476e-12}},{"name":"[True conditional] Using constructor name","hz":147039.09863156595,"cycles":3,"stats":{"deviation":2.1990088769223852e-7,"mean":0.000006800912201629361,"moe":4.3989339121202735e-8,"rme":0.6468152773779932,"sem":2.244354036796058e-8,"variance":4.83564004078345e-14}},{"name":"[True conditional] Check if property is valid then instanceof ","hz":145368.9392529347,"cycles":3,"stats":{"deviation":4.0337741856876267e-7,"mean":0.000006879048613404613,"moe":8.380552487096401e-8,"rme":1.2182720254027477,"sem":4.275792085253266e-8,"variance":1.6271334181119876e-13}},{"name":"[False conditional] Using instanceof only","hz":711546373.8386632,"cycles":11,"stats":{"deviation":1.2003984263860308e-11,"mean":1.4053897774858748e-9,"moe":2.3646337913154004e-12,"rme":0.16825465996668434,"sem":1.2064458118956125e-12,"variance":1.4409563820700589e-22}},{"name":"[False conditional] Using constructor name","hz":711012359.7508119,"cycles":10,"stats":{"deviation":1.154460985267358e-11,"mean":1.40644531179524e-9,"moe":2.2974679670076795e-12,"rme":0.16335281206740307,"sem":1.1721775341875915e-12,"variance":1.3327801665044792e-22}},{"name":"[False conditional] Check if property is valid then instanceof ","hz":710393527.8499533,"cycles":6,"stats":{"deviation":3.159099495604374e-11,"mean":1.4076704823403407e-9,"moe":6.386390184071106e-12,"rme":0.45368502530885857,"sem":3.258362338811789e-12,"variance":9.97990962312781e-22}}]}-->

## Crypto Verify

|name|ops/sec|samples|
|-|-|-|
|crypto.createVerify('RSA-SHA256')|4,515|90|
|crypto.verify('RSA-SHA256')|4,499|94|


<details>
<summary>Environment</summary>

* __Machine:__ linux x64 | 2 vCPUs | 6.8GB Mem
* __Run:__ Sat Oct 14 2023 01:40:17 GMT+0000 (Coordinated Universal Time)
</details>

<!--
{"environment":{"platform":"linux","arch":"x64","cpus":2,"totalMemory":6.759757995605469},"benchmarks":[{"name":"crypto.createVerify('RSA-SHA256')","hz":4515.0193977735435,"cycles":4,"stats":{"deviation":0.0000042815054893696955,"mean":0.00022148299085782938,"moe":8.845681985135754e-7,"rme":0.39938425749423906,"sem":4.513103053640691e-7,"variance":1.8331289255502838e-11}},{"name":"crypto.verify('RSA-SHA256')","hz":4499.40281607116,"cycles":3,"stats":{"deviation":0.000008100742834345195,"mean":0.0002222517167007491,"moe":0.0000016376345408851729,"rme":0.7368377464954147,"sem":8.355278269822311e-7,"variance":6.562203446819503e-11}}]}-->