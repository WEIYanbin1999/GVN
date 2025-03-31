# ICML 2025 GVN Rebuttal (Supplement Tables and Figures)
##### Table A: Link prediction effectiveness of positional encodings (Hits@100). We adopt 2-GCN+2-MLP as the decoder.
||Cora|Citeseer|Pubmed|
|---|---|---|---|
|VSF|71.32±0.70|60.96±0.68|48.27±0.51|
|2-D Axis in Image|38.57±1.22|33.29±1.80|25.34±0.95|
|Laplacian PE|55.14±0.84|52.03±1.17|46.80±0.75|
|Distance|42.03±0.82|56.65±0.43|44.21±0.36|
|Degree/Centrality|42.80±1.52|44.15±1.61|34.90±1.23|

##### Table B: Node Classification Accuracy of GCN compared with GCN+VSF (\%).
||Cora|Citeseer|
|---|---|---|
|GCN|87.79±0.49|71.29±0.32|
|GCN+VSF|89.30±0.33|74.26±0.51|

##### Figure A: Inference time and the use of GPU memory of different methods on Cora (linear scale axis).
![3af08fbaf19750b1aa2bd3411ae9f408](https://github.com/user-attachments/assets/b8ec7825-499f-4bcc-bbad-2b625108afd6)


##### Table C: Time scalability comparison (/s) on Erdos-Renyi graphs w.r.t. increasing node counts. O(VE) time contributions in E-GVN and GVN are explicitly listed in parentheses.
|\# Node |100|500|1000|5000|
|---|---|---|---|---|
|GCN|1.91|18.88|80.35|1859.9836|
|E-GVN|5.02(3.56)|52.29(21.32)|187.61(44.28)|2065.44(76.56)|
|SEAL|459.38|9765.47|40257.88|-|
|GVN|4196.21(3448.96)|91527.96(78251.26)|-|-|

##### Table D:  Link prediction performance of E-GVN on Cora with varying layout algorithms (Hits@100).
||fdp|dot|sfdp|neato|circo|twopi|osage|
|---|---|---|---|---|---|---|---|
|Hits@100|**91.56**|**91.54**|91.26|91.17|90.67|90.58|89.60|
