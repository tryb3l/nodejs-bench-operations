## Stream.Writable

|name|ops/sec|samples|
|-|-|-|
|streams.Writable writing 1e3 * "some data"|6,646|93|
|streams.web.WritableStream writing 1e3 * "some data"|1,021|47|


<details>
<summary>Environment</summary>

* __Machine:__ linux x64 | 4 vCPUs | 15.2GB Mem
* __Run:__ Sat May 04 2024 01:05:23 GMT+0000 (Coordinated Universal Time)
</details>

<!--
{"environment":{"platform":"linux","arch":"x64","cpus":4,"totalMemory":15.245216369628906},"benchmarks":[{"name":"streams.Writable writing 1e3 * \"some data\"","opsSec":6645.613058895063,"samples":4},{"name":"streams.web.WritableStream writing 1e3 * \"some data\"","opsSec":1020.7822604845217,"samples":3}]}-->