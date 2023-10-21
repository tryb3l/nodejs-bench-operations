## Parsing Integer

|name|ops/sec|samples|
|-|-|-|
|Using parseInt(x, 10) - small number (2 len)|217,024,630|91|
|Using parseInt(x, 10) - big number (10 len)|15,284,371|91|
|Using + - small number (2 len)|594,313,720|97|
|Using + - big number (10 len)|593,539,262|93|


<details>
<summary>Environment</summary>

* __Machine:__ linux x64 | 2 vCPUs | 6.8GB Mem
* __Run:__ Sat Oct 21 2023 13:07:41 GMT+0000 (Coordinated Universal Time)
</details>

<!--
{"environment":{"platform":"linux","arch":"x64","cpus":2,"totalMemory":6.7597503662109375},"benchmarks":[{"name":"Using parseInt(x, 10) - small number (2 len)","opsSec":217024629.91713628,"samples":6},{"name":"Using parseInt(x, 10) - big number (10 len)","opsSec":15284370.544729333,"samples":7},{"name":"Using + - small number (2 len)","opsSec":594313719.9057946,"samples":8},{"name":"Using + - big number (10 len)","opsSec":593539261.7908756,"samples":6}]}-->