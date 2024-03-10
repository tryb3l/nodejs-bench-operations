## Object.keys vs Object.getOwnPropertyNames comparison

|name|ops/sec|samples|
|-|-|-|
|Using Object.keys()|90,035,857|90|
|Using Object.getOwnPropertyNames()|90,439,786|95|


<details>
<summary>Environment</summary>

* __Machine:__ linux x64 | 4 vCPUs | 15.6GB Mem
* __Run:__ Sun Mar 10 2024 15:54:31 GMT+0000 (Coordinated Universal Time)
</details>

<!--
{"environment":{"platform":"linux","arch":"x64","cpus":4,"totalMemory":15.606491088867188},"benchmarks":[{"name":"Using Object.keys()","opsSec":90035857.38520935,"samples":5},{"name":"Using Object.getOwnPropertyNames()","opsSec":90439785.87219489,"samples":6}]}-->