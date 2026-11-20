# Supplementary experimental results

The tables report accuracy as a percentage. SD is the sample standard deviation in percentage points. Where reported in Tables A.1–A.9 and A.11, the baseline is YOLO26n-OBB; Table A.10 uses each original YOLO variant as its baseline. Rows labeled CSPPF or DSC use only the named module. Tables A.2–A.4 provide individual run scores and seeds, while Tables A.5–A.10 report three-run means. Reference numbers follow the main manuscript.

Implementation and timing details. The archived YOLO26 implementation identifies its Ultralytics package version as 8.4.67. For the efficiency measurements in Section 4.4.1, each of the 100 measurement groups comprised 30 warm-up passes and 100 timed forward passes per model. DOTA-v1.0 images were prepared using 1024 × 1024 crops with a 500-pixel gap at scale factors of 0.5, 1.0, and 1.5, following the Ultralytics multi-scale cropping workflow [25]. UCAS-AOD followed the same training and validation partitioning approach and training configuration as DOTA-v1.0, including the input size.


## Table A.1 DOTA-v1.0 validation results across three runs

<table>
<tr>
<td>Configuration</td>
<td>Mean mAP50 (%)</td>
<td>Sample SD (pp)</td>
</tr>
<tr>
<td>Baseline</td>
<td>78.887</td>
<td>0.015</td>
</tr>
<tr>
<td>CSPPF</td>
<td>79.093</td>
<td>0.029</td>
</tr>
<tr>
<td>DSC</td>
<td>79.393</td>
<td>0.040</td>
</tr>
<tr>
<td>PCDSNet</td>
<td>79.923</td>
<td>0.023</td>
</tr>
</table>


## Table A.2 DOTA-v1.0 seeds and run scores

<table>
<tr>
<td>Configuration</td>
<td>Run</td>
<td>Random seed</td>
<td>mAP50 (%)</td>
</tr>
<tr>
<td>Baseline</td>
<td>1</td>
<td>3675759335</td>
<td>78.87</td>
</tr>
<tr>
<td>Baseline</td>
<td>2</td>
<td>422548288</td>
<td>78.90</td>
</tr>
<tr>
<td>Baseline</td>
<td>3</td>
<td>1068332517</td>
<td>78.89</td>
</tr>
<tr>
<td>CSPPF</td>
<td>1</td>
<td>2378683759</td>
<td>79.11</td>
</tr>
<tr>
<td>CSPPF</td>
<td>2</td>
<td>3729888869</td>
<td>79.06</td>
</tr>
<tr>
<td>CSPPF</td>
<td>3</td>
<td>2520263472</td>
<td>79.11</td>
</tr>
<tr>
<td>DSC</td>
<td>1</td>
<td>534831654</td>
<td>79.37</td>
</tr>
<tr>
<td>DSC</td>
<td>2</td>
<td>1442742160</td>
<td>79.37</td>
</tr>
<tr>
<td>DSC</td>
<td>3</td>
<td>6964122</td>
<td>79.44</td>
</tr>
<tr>
<td>PCDSNet</td>
<td>1</td>
<td>883592722</td>
<td>79.95</td>
</tr>
<tr>
<td>PCDSNet</td>
<td>2</td>
<td>2199121024</td>
<td>79.91</td>
</tr>
<tr>
<td>PCDSNet</td>
<td>3</td>
<td>1855559642</td>
<td>79.91</td>
</tr>
</table>


## Table A.3 HRSC2016 seeds and run scores

<table>
<tr>
<td>Configuration</td>
<td>Run</td>
<td>Random seed</td>
<td>mAP50 (%)</td>
<td>mAP50:95 (%)</td>
</tr>
<tr>
<td>Baseline</td>
<td>1</td>
<td>1762348300</td>
<td>74.63</td>
<td>52.96</td>
</tr>
<tr>
<td>Baseline</td>
<td>2</td>
<td>2022366191</td>
<td>74.58</td>
<td>52.81</td>
</tr>
<tr>
<td>Baseline</td>
<td>3</td>
<td>2465180021</td>
<td>74.60</td>
<td>52.90</td>
</tr>
<tr>
<td>CSPPF</td>
<td>1</td>
<td>1334453262</td>
<td>74.53</td>
<td>53.36</td>
</tr>
<tr>
<td>CSPPF</td>
<td>2</td>
<td>2442645511</td>
<td>75.17</td>
<td>54.09</td>
</tr>
<tr>
<td>CSPPF</td>
<td>3</td>
<td>1984595556</td>
<td>75.02</td>
<td>53.98</td>
</tr>
<tr>
<td>DSC</td>
<td>1</td>
<td>4000231331</td>
<td>72.55</td>
<td>55.33</td>
</tr>
<tr>
<td>DSC</td>
<td>2</td>
<td>3032048367</td>
<td>73.61</td>
<td>56.17</td>
</tr>
<tr>
<td>DSC</td>
<td>3</td>
<td>958295836</td>
<td>72.97</td>
<td>55.84</td>
</tr>
<tr>
<td>PCDSNet</td>
<td>1</td>
<td>627529833</td>
<td>75.52</td>
<td>54.57</td>
</tr>
<tr>
<td>PCDSNet</td>
<td>2</td>
<td>1487817346</td>
<td>75.61</td>
<td>55.01</td>
</tr>
<tr>
<td>PCDSNet</td>
<td>3</td>
<td>1032634706</td>
<td>75.83</td>
<td>55.29</td>
</tr>
</table>


## Table A.4 UCAS-AOD seeds and run scores

<table>
<tr>
<td>Configuration</td>
<td>Run</td>
<td>Random seed</td>
<td>mAP50 (%)</td>
<td>mAP50:95 (%)</td>
</tr>
<tr>
<td>Baseline</td>
<td>1</td>
<td>110125225</td>
<td>96.47</td>
<td>74.30</td>
</tr>
<tr>
<td>Baseline</td>
<td>2</td>
<td>862491363</td>
<td>96.50</td>
<td>74.21</td>
</tr>
<tr>
<td>Baseline</td>
<td>3</td>
<td>3984113919</td>
<td>96.24</td>
<td>74.09</td>
</tr>
<tr>
<td>CSPPF</td>
<td>1</td>
<td>2470567238</td>
<td>96.74</td>
<td>73.79</td>
</tr>
<tr>
<td>CSPPF</td>
<td>2</td>
<td>3828411715</td>
<td>96.86</td>
<td>73.96</td>
</tr>
<tr>
<td>CSPPF</td>
<td>3</td>
<td>2583487048</td>
<td>96.08</td>
<td>72.97</td>
</tr>
<tr>
<td>DSC</td>
<td>1</td>
<td>3688754663</td>
<td>96.93</td>
<td>75.16</td>
</tr>
<tr>
<td>DSC</td>
<td>2</td>
<td>3469258912</td>
<td>97.05</td>
<td>75.29</td>
</tr>
<tr>
<td>DSC</td>
<td>3</td>
<td>868547875</td>
<td>96.89</td>
<td>75.15</td>
</tr>
<tr>
<td>PCDSNet</td>
<td>1</td>
<td>4079017673</td>
<td>96.75</td>
<td>74.37</td>
</tr>
<tr>
<td>PCDSNet</td>
<td>2</td>
<td>2269430747</td>
<td>97.01</td>
<td>74.69</td>
</tr>
<tr>
<td>PCDSNet</td>
<td>3</td>
<td>1107188134</td>
<td>97.16</td>
<td>74.97</td>
</tr>
</table>


## Table A.5 Channel attention and recalibration order on HRSC2016 and UCAS-AOD

<table>
<tr>
<td>Configuration</td>
<td>HRSC2016mAP50 (%)</td>
<td>HRSC2016mAP50:95 (%)</td>
<td>UCAS-AODmAP50 (%)</td>
<td>UCAS-AODmAP50:95 (%)</td>
</tr>
<tr>
<td>Baseline</td>
<td>74.603</td>
<td>52.890</td>
<td>96.403</td>
<td>74.200</td>
</tr>
<tr>
<td>CSPPF before pooling</td>
<td>74.907</td>
<td>53.810</td>
<td>96.560</td>
<td>73.573</td>
</tr>
<tr>
<td>SE</td>
<td>73.813</td>
<td>51.872</td>
<td>96.501</td>
<td>74.107</td>
</tr>
<tr>
<td>CBAM</td>
<td>73.633</td>
<td>51.629</td>
<td>94.219</td>
<td>73.201</td>
</tr>
<tr>
<td>Recalibration after pooling</td>
<td>74.000</td>
<td>52.163</td>
<td>96.299</td>
<td>74.150</td>
</tr>
</table>


## Table A.6 Upsampling alternatives on HRSC2016 and UCAS-AOD

<table>
<tr>
<td>Configuration</td>
<td>HRSC2016mAP50 (%)</td>
<td>HRSC2016mAP50:95 (%)</td>
<td>UCAS-AODmAP50 (%)</td>
<td>UCAS-AODmAP50:95 (%)</td>
</tr>
<tr>
<td>Fixed nearest-neighbor</td>
<td>74.603</td>
<td>52.890</td>
<td>96.403</td>
<td>74.200</td>
</tr>
<tr>
<td>DSC</td>
<td>73.043</td>
<td>55.780</td>
<td>96.957</td>
<td>75.200</td>
</tr>
<tr>
<td>Bilinear interpolation</td>
<td>72.817</td>
<td>54.816</td>
<td>96.499</td>
<td>75.319</td>
</tr>
<tr>
<td>CARAFE</td>
<td>72.993</td>
<td>55.690</td>
<td>96.327</td>
<td>74.112</td>
</tr>
</table>


## Table A.7 CSPPF path ablation at a split ratio of 0.25

<table>
<tr>
<td>Configuration</td>
<td>HRSC2016mAP50 (%)</td>
<td>HRSC2016mAP50:95 (%)</td>
<td>UCAS-AODmAP50 (%)</td>
<td>UCAS-AODmAP50:95 (%)</td>
</tr>
<tr>
<td>Baseline</td>
<td>74.603</td>
<td>52.890</td>
<td>96.403</td>
<td>74.200</td>
</tr>
<tr>
<td>Local convolution only</td>
<td>74.700</td>
<td>53.100</td>
<td>96.450</td>
<td>73.300</td>
</tr>
<tr>
<td>Statistical recalibration only</td>
<td>74.800</td>
<td>53.500</td>
<td>96.500</td>
<td>73.450</td>
</tr>
<tr>
<td>Full CSPPF</td>
<td>74.907</td>
<td>53.810</td>
<td>96.560</td>
<td>73.573</td>
</tr>
</table>


## Table A.8 Sensitivity to the CSPPF channel split ratio

<table>
<tr>
<td>Split ratio</td>
<td>HRSC2016mAP50 (%)</td>
<td>HRSC2016mAP50:95 (%)</td>
<td>UCAS-AODmAP50 (%)</td>
<td>UCAS-AODmAP50:95 (%)</td>
</tr>
<tr>
<td>0.125</td>
<td>72.110</td>
<td>51.591</td>
<td>95.191</td>
<td>70.979</td>
</tr>
<tr>
<td>0.25</td>
<td>74.907</td>
<td>53.810</td>
<td>96.560</td>
<td>73.573</td>
</tr>
<tr>
<td>0.5</td>
<td>74.913</td>
<td>53.800</td>
<td>96.591</td>
<td>73.672</td>
</tr>
<tr>
<td>0.75</td>
<td>75.019</td>
<td>53.829</td>
<td>96.544</td>
<td>73.598</td>
</tr>
</table>


## Table A.9 Sensitivity to the number of DSC sampling groups

<table>
<tr>
<td>Sampling groups</td>
<td>HRSC2016mAP50 (%)</td>
<td>HRSC2016mAP50:95 (%)</td>
<td>UCAS-AODmAP50 (%)</td>
<td>UCAS-AODmAP50:95 (%)</td>
</tr>
<tr>
<td>1</td>
<td>72.611</td>
<td>54.017</td>
<td>96.510</td>
<td>74.629</td>
</tr>
<tr>
<td>2</td>
<td>72.186</td>
<td>55.467</td>
<td>96.549</td>
<td>74.721</td>
</tr>
<tr>
<td>4</td>
<td>73.043</td>
<td>55.780</td>
<td>96.957</td>
<td>75.200</td>
</tr>
<tr>
<td>8</td>
<td>73.193</td>
<td>56.297</td>
<td>97.160</td>
<td>75.562</td>
</tr>
</table>


## Table A.10 Transfer across YOLO versions on DOTA-v1.0

<table>
<tr>
<td>Model</td>
<td>Original mAP50 (%)</td>
<td>With CSPPF and DSC (%)</td>
<td>Difference (pp)</td>
</tr>
<tr>
<td>YOLOv8n-OBB</td>
<td>77.970</td>
<td>78.107</td>
<td>+0.137</td>
</tr>
<tr>
<td>YOLO11n-OBB</td>
<td>78.471</td>
<td>78.496</td>
<td>+0.025</td>
</tr>
<tr>
<td>YOLO12n-OBB</td>
<td>78.533</td>
<td>79.020</td>
<td>+0.487</td>
</tr>
</table>


## Table A.11 Module-composition results (mean ± SD). Δ denotes the mAP change at an IoU threshold of 0.5, in percentage points before rounding.

<table>
<tr>
<td>Configuration</td>
<td>P5 unit / scope</td>
<td>Neck fusion</td>
<td>Params</td>
<td colspan="3">HRSC2016</td>
<td colspan="3">UCAS-AOD</td>
</tr>
<tr>
<td></td>
<td></td>
<td></td>
<td></td>
<td>mAP50 (%)</td>
<td>mAP50:95 (%)</td>
<td>Δ (pp)</td>
<td>mAP50 (%)</td>
<td>mAP50:95 (%)</td>
<td>Δ (pp)</td>
</tr>
<tr>
<td colspan="10">Module composition</td>
</tr>
<tr>
<td>Baseline</td>
<td>SPPF</td>
<td>Fixed upsampling + Concat</td>
<td>–</td>
<td>74.603±0.025</td>
<td>52.890±0.075</td>
<td>–</td>
<td>96.403±0.142</td>
<td>74.200±0.105</td>
<td>–</td>
</tr>
<tr>
<td>Channel sel.</td>
<td>CSPPF@P5</td>
<td>Fixed upsampling + Concat</td>
<td>+111.4K</td>
<td>74.907±0.335</td>
<td>53.810±0.394</td>
<td>+0.303</td>
<td>96.560±0.420</td>
<td>73.573±0.529</td>
<td>+0.157</td>
</tr>
<tr>
<td>Dynamic samp.</td>
<td>SPPF</td>
<td>DSC</td>
<td>+12.4K</td>
<td>73.043±0.534</td>
<td>55.780±0.423</td>
<td>−1.560</td>
<td>96.957±0.083</td>
<td>75.200±0.078</td>
<td>+0.553</td>
</tr>
<tr>
<td>PCDSNet</td>
<td>CSPPF@P5</td>
<td>DSC</td>
<td>+123.7K</td>
<td>75.653±0.159</td>
<td>54.957±0.363</td>
<td>+1.050</td>
<td>96.973±0.207</td>
<td>74.677±0.300</td>
<td>+0.570</td>
</tr>
</table>
