![Banner Scout report](https://www.example.com/banner.png)
# Scout Report - 2024-04-26 11:47:29
## Summary
 - [unused_imports](unused_imports) (1 results) (Unknown)
 - [Check Soroban version](check-soroban-version) (1 results) (Enhancement)
 - [Overflow Check](overflow-check) (1 results) (Critical)
 - [Unsafe Unwrap](unsafe-unwrap) (33 results) (Medium)
## Local detectors
### unused_imports
**Impact:** Unknown
**Description:** 
**More about:** [here]()
<table style="width: 100%; table-layout: fixed;"><thead><tr><th style="width: 20%;">ID</th><th style="width: 60%;">Detection</th><th style="width: 20%;">Status</th></tr></thead><tbody>
<tr><td>8</td><td><a href="link-to-github">src/soroswap_pair_token/mod.rs:10:9 - 10:42</a></td><td><ul><li>- [ ] False Positive </li><li>- [ ] Acknowledged</li><li>- [ ] Resolved</li></ul></td></tr>
</tbody></table>
</tbody></table>
## Best practices
### Check Soroban version
**Impact:** Enhancement
**Description:** Use the latest version of Soroban
**More about:** [here](https://github.com/CoinFabrik/scout-soroban/tree/main/detectors/soroban-version)
<table style="width: 100%; table-layout: fixed;"><thead><tr><th style="width: 20%;">ID</th><th style="width: 60%;">Detection</th><th style="width: 20%;">Status</th></tr></thead><tbody>
<tr><td>7</td><td><a href="link-to-github">src/lib.rs:1:1 - 1:1</a></td><td><ul><li>- [ ] False Positive </li><li>- [ ] Acknowledged</li><li>- [ ] Resolved</li></ul></td></tr>
</tbody></table>
</tbody></table>
## Arithmetic
### Overflow Check
**Impact:** Critical
**Description:** Use `overflow-checks = true` in Cargo.toml profile
**More about:** [here](https://github.com/CoinFabrik/scout-soroban/tree/main/detectors/overflow-check)
<table style="width: 100%; table-layout: fixed;"><thead><tr><th style="width: 20%;">ID</th><th style="width: 60%;">Detection</th><th style="width: 20%;">Status</th></tr></thead><tbody>
<tr><td>6</td><td><a href="link-to-github">src/lib.rs:1:1 - 1:1</a></td><td><ul><li>- [ ] False Positive </li><li>- [ ] Acknowledged</li><li>- [ ] Resolved</li></ul></td></tr>
</tbody></table>
</tbody></table>
## Validations and error handling
### Unsafe Unwrap
**Impact:** Medium
**Description:** Unsafe usage of `unwrap`
**More about:** [here](https://github.com/CoinFabrik/scout-soroban/tree/main/detectors/unsafe-unwrap)
### Unused Return Enum
**Impact:** Minor
**Description:** If any of the variants (Ok/Err) is not used, the code could be simplified or it could imply a bug
**More about:** [here](https://github.com/CoinFabrik/scout-soroban/tree/main/detectors/unused-return-enum)
### Unsafe Expect
**Impact:** Medium
**Description:** Unsafe usage of `expect`
**More about:** [here](https://github.com/CoinFabrik/scout-soroban/tree/main/detectors/unsafe-expect)
### Avoid panic! macro
**Impact:** Enhancement
**Description:** The panic! macro is used to stop execution when a condition is not met. Even when this does not break the execution of the contract, it is recommended to use Result instead of panic! because it will stop the execution of the caller contract
**More about:** [here](https://github.com/CoinFabrik/scout-soroban/tree/main/detectors/avoid-panic-error)
<table style="width: 100%; table-layout: fixed;"><thead><tr><th style="width: 20%;">ID</th><th style="width: 60%;">Detection</th><th style="width: 20%;">Status</th></tr></thead><tbody>
<tr><td>0</td><td><a href="link-to-github">src/soroswap_pair_token/allowance.rs:36:9 - 36:76</a></td><td><ul><li>- [ ] False Positive </li><li>- [ ] Acknowledged</li><li>- [ ] Resolved</li></ul></td></tr>
<tr><td>1</td><td><a href="link-to-github">src/soroswap_pair_token/allowance.rs:54:9 - 54:42</a></td><td><ul><li>- [ ] False Positive </li><li>- [ ] Acknowledged</li><li>- [ ] Resolved</li></ul></td></tr>
<tr><td>2</td><td><a href="link-to-github">src/soroswap_pair_token/balance.rs:36:9 - 36:40</a></td><td><ul><li>- [ ] False Positive </li><li>- [ ] Acknowledged</li><li>- [ ] Resolved</li></ul></td></tr>
<tr><td>3</td><td><a href="link-to-github">src/soroswap_pair_token/total_supply.rs:25:9 - 25:45</a></td><td><ul><li>- [ ] False Positive </li><li>- [ ] Acknowledged</li><li>- [ ] Resolved</li></ul></td></tr>
<tr><td>4</td><td><a href="link-to-github">src/storage.rs:95:9 - 95:59</a></td><td><ul><li>- [ ] False Positive </li><li>- [ ] Acknowledged</li><li>- [ ] Resolved</li></ul></td></tr>
<tr><td>5</td><td><a href="link-to-github">src/storage.rs:103:9 - 103:59</a></td><td><ul><li>- [ ] False Positive </li><li>- [ ] Acknowledged</li><li>- [ ] Resolved</li></ul></td></tr>
<tr><td>9</td><td><a href="link-to-github">src/soroswap_pair_token/allowance.rs:43:9 - 45:23</a></td><td><ul><li>- [ ] False Positive </li><li>- [ ] Acknowledged</li><li>- [ ] Resolved</li></ul></td></tr>
<tr><td>10</td><td><a href="link-to-github">src/soroswap_pair_token/balance.rs:27:5 - 28:68</a></td><td><ul><li>- [ ] False Positive </li><li>- [ ] Acknowledged</li><li>- [ ] Resolved</li></ul></td></tr>
<tr><td>11</td><td><a href="link-to-github">src/soroswap_pair_token/total_supply.rs:17:5 - 18:77</a></td><td><ul><li>- [ ] False Positive </li><li>- [ ] Acknowledged</li><li>- [ ] Resolved</li></ul></td></tr>
<tr><td>12</td><td><a href="link-to-github">src/soroswap_pair_token/total_supply.rs:27:5 - 28:78</a></td><td><ul><li>- [ ] False Positive </li><li>- [ ] Acknowledged</li><li>- [ ] Resolved</li></ul></td></tr>
<tr><td>13</td><td><a href="link-to-github">src/storage.rs:27:9 - 27:31</a></td><td><ul><li>- [ ] False Positive </li><li>- [ ] Acknowledged</li><li>- [ ] Resolved</li></ul></td></tr>
<tr><td>14</td><td><a href="link-to-github">src/storage.rs:38:5 - 39:32</a></td><td><ul><li>- [ ] False Positive </li><li>- [ ] Acknowledged</li><li>- [ ] Resolved</li></ul></td></tr>
<tr><td>15</td><td><a href="link-to-github">src/storage.rs:48:5 - 49:31</a></td><td><ul><li>- [ ] False Positive </li><li>- [ ] Acknowledged</li><li>- [ ] Resolved</li></ul></td></tr>
<tr><td>16</td><td><a href="link-to-github">src/storage.rs:53:5 - 54:31</a></td><td><ul><li>- [ ] False Positive </li><li>- [ ] Acknowledged</li><li>- [ ] Resolved</li></ul></td></tr>
<tr><td>17</td><td><a href="link-to-github">src/storage.rs:58:5 - 59:33</a></td><td><ul><li>- [ ] False Positive </li><li>- [ ] Acknowledged</li><li>- [ ] Resolved</li></ul></td></tr>
<tr><td>18</td><td><a href="link-to-github">src/storage.rs:63:5 - 64:33</a></td><td><ul><li>- [ ] False Positive </li><li>- [ ] Acknowledged</li><li>- [ ] Resolved</li></ul></td></tr>
<tr><td>19</td><td><a href="link-to-github">src/strings.rs:16:30 - 16:78</a></td><td><ul><li>- [ ] False Positive </li><li>- [ ] Acknowledged</li><li>- [ ] Resolved</li></ul></td></tr>
<tr><td>20</td><td><a href="link-to-github">src/strings.rs:28:30 - 28:83</a></td><td><ul><li>- [ ] False Positive </li><li>- [ ] Acknowledged</li><li>- [ ] Resolved</li></ul></td></tr>
<tr><td>21</td><td><a href="link-to-github">src/lib.rs:214:27 - 214:68</a></td><td><ul><li>- [ ] False Positive </li><li>- [ ] Acknowledged</li><li>- [ ] Resolved</li></ul></td></tr>
<tr><td>22</td><td><a href="link-to-github">src/lib.rs:288:9 - 288:94</a></td><td><ul><li>- [ ] False Positive </li><li>- [ ] Acknowledged</li><li>- [ ] Resolved</li></ul></td></tr>
<tr><td>23</td><td><a href="link-to-github">src/lib.rs:289:9 - 289:94</a></td><td><ul><li>- [ ] False Positive </li><li>- [ ] Acknowledged</li><li>- [ ] Resolved</li></ul></td></tr>
<tr><td>24</td><td><a href="link-to-github">src/lib.rs:291:9 - 291:73</a></td><td><ul><li>- [ ] False Positive </li><li>- [ ] Acknowledged</li><li>- [ ] Resolved</li></ul></td></tr>
<tr><td>25</td><td><a href="link-to-github">src/lib.rs:292:9 - 292:73</a></td><td><ul><li>- [ ] False Positive </li><li>- [ ] Acknowledged</li><li>- [ ] Resolved</li></ul></td></tr>
<tr><td>26</td><td><a href="link-to-github">src/lib.rs:329:9 - 329:87</a></td><td><ul><li>- [ ] False Positive </li><li>- [ ] Acknowledged</li><li>- [ ] Resolved</li></ul></td></tr>
<tr><td>27</td><td><a href="link-to-github">src/lib.rs:339:9 - 339:110</a></td><td><ul><li>- [ ] False Positive </li><li>- [ ] Acknowledged</li><li>- [ ] Resolved</li></ul></td></tr>
<tr><td>28</td><td><a href="link-to-github">src/lib.rs:340:9 - 340:110</a></td><td><ul><li>- [ ] False Positive </li><li>- [ ] Acknowledged</li><li>- [ ] Resolved</li></ul></td></tr>
<tr><td>29</td><td><a href="link-to-github">src/lib.rs:357:27 - 357:68</a></td><td><ul><li>- [ ] False Positive </li><li>- [ ] Acknowledged</li><li>- [ ] Resolved</li></ul></td></tr>
<tr><td>30</td><td><a href="link-to-github">src/lib.rs:374:9 - 374:67</a></td><td><ul><li>- [ ] False Positive </li><li>- [ ] Acknowledged</li><li>- [ ] Resolved</li></ul></td></tr>
<tr><td>31</td><td><a href="link-to-github">src/lib.rs:375:9 - 375:67</a></td><td><ul><li>- [ ] False Positive </li><li>- [ ] Acknowledged</li><li>- [ ] Resolved</li></ul></td></tr>
<tr><td>32</td><td><a href="link-to-github">src/lib.rs:452:13 - 452:77</a></td><td><ul><li>- [ ] False Positive </li><li>- [ ] Acknowledged</li><li>- [ ] Resolved</li></ul></td></tr>
<tr><td>33</td><td><a href="link-to-github">src/lib.rs:456:17 - 456:108</a></td><td><ul><li>- [ ] False Positive </li><li>- [ ] Acknowledged</li><li>- [ ] Resolved</li></ul></td></tr>
<tr><td>34</td><td><a href="link-to-github">src/lib.rs:457:17 - 457:104</a></td><td><ul><li>- [ ] False Positive </li><li>- [ ] Acknowledged</li><li>- [ ] Resolved</li></ul></td></tr>
<tr><td>35</td><td><a href="link-to-github">src/lib.rs:458:17 - 458:94</a></td><td><ul><li>- [ ] False Positive </li><li>- [ ] Acknowledged</li><li>- [ ] Resolved</li></ul></td></tr>
</tbody></table>
