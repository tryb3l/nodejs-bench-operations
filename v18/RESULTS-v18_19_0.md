## Adding property

|name|ops/sec|samples|
|-|-|-|
|Directly in the object|819,505,367|97|
|Using dot notation|787,157,794|94|
|Using define property (writable)|4,260,711|95|
|Using define property initialized (writable)|5,897,360|90|
|Using define property (getter)|2,286,029|88|


<details>
<summary>Environment</summary>

* __Machine:__ linux x64 | 4 vCPUs | 15.6GB Mem
* __Run:__ Tue Mar 12 2024 18:19:58 GMT+0000 (Coordinated Universal Time)
</details>

<!--
{"environment":{"platform":"linux","arch":"x64","cpus":4,"totalMemory":15.606491088867188},"benchmarks":[{"name":"Directly in the object","opsSec":819505367.0324596,"samples":6},{"name":"Using dot notation","opsSec":787157793.5177962,"samples":8},{"name":"Using define property (writable)","opsSec":4260711.370325327,"samples":5},{"name":"Using define property initialized (writable)","opsSec":5897360.34853542,"samples":5},{"name":"Using define property (getter)","opsSec":2286029.163858436,"samples":3}]}-->

## Array.append (number)

|type|amount|time elapsed|
|-|-|-|
array.push|10|0.014ms
new Array(length)|10|0.002ms
array.push|100|0.103ms
new Array(length)|100|0.014ms
array.push|1,000|0.039ms
new Array(length)|1,000|0.02ms
array.push|10,000|0.325ms
new Array(length)|10,000|0.206ms
array.push|1,000,000|22.839ms
new Array(length)|1,000,000|14.82ms
array.push|100,000,000|970.14ms
new Array(length)|100,000,000|3,616.563ms
## Array.append (string)

|type|amount|time elapsed|
|-|-|-|
array.push|10|0.006ms
new Array(length)|10|0.017ms
array.push|100|0.076ms
new Array(length)|100|0.008ms
array.push|1,000|0.033ms
new Array(length)|1,000|0.015ms
array.push|10,000|0.258ms
new Array(length)|10,000|3.355ms
array.push|1,000,000|61.532ms
new Array(length)|1,000,000|2.537ms
array.push|100,000,000|1,412.406ms
new Array(length)|100,000,000|4,103.942ms