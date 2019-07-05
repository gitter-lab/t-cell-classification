# Cell Images

There are two types of example images in this directory.

|Type|File/Directory|Description|
|:---:|:---:|:---:|
|Example images| [`examples`](./examples)| A few randomly picked images to demonstrate microscopy images|
|Subsampled images| [`sample_images.zip`](./sample_images.zip)| A 10% stratified subsample from the full dataset. These images are used to run the notebooks in this repository|

## Cell Image Activity Count

All cell images came from 6 donors. We are interested in classifying T-cell activity status: activated or quiescent.

||Donor 1|Donor 2|Donor 3|Donor 4|Donor 5|Donor 6|
|:---:|:---:|:---:|:---:|:---:|:---:|:---:|
|Example Activated|1|1|1|1|1|1|
|Example Quiescent|1|1|1|1|1|1|
|Subsampled Activated|27|65|48|49|69|44|
|Subsampled Quiescent|163|15|127|162|25|58|
|Full Activated|271|656|487|494|694|446|
|Full Quiescent|1631|152|1276|1629|252|589|

Only the example and subsampled images are available.

## Cell Image Filename Encoding

All image files share the same name string encoding.

```
CD3_1_act_9_3_33.png
CD[$1]_[$2]_[$3]_[$4]_[$5]_[$6].png

$1: 3 or 8, type of this T-cell
$2: Donor ID
$3: Activity, 'act' means activated while `noact` means quiescent
$4: Batch ID
$5: Plate ID
$6: Cell ID
```

For example, `CD3_1_act_9_3_33.png` is the image of the 33th cell from Plate 3 in Batch 9. This cell is an activated CD3 T-cell.

## File Structure

In order to run the notebooks, you want to decompress [`sample_images.zip`](./sample_images.zip) first. The files should have the following structure:

```
./
|-- README.md
|-- examples
|   |-- CD3_1_act_9_3_33.png
|   |-- ...
|   `-- CD8_6_noact_12_3_64.png
|-- sample_images
|   `-- original
|       |-- donor_1
|       |   |-- activated
|       |   |   |-- CD3_1_act_9_1_12.png
|       |   |   |-- ...
|       |   |   `-- CD8_1_act_4_5_4.png
|       |   `-- quiescent
|       |       |-- CD3_1_noact_10_1_103.png
|       |       |-- ...
|       |       `-- CD8_1_noact_2_6_99.png
|       |-- donor_2
|       |   |-- activated
|       |   |   |-- CD3_2_act_2_1_23.png
|       |   |   |-- ...
|       |   |   `-- CD8_2_act_4_8_35.png
|       |   `-- quiescent
|       |       |-- CD3_2_noact_1_1_47.png
|       |       |-- ...
|       |       `-- CD8_2_noact_3_9_31.png
|       |-- donor_3
|       |   |-- activated
|       |   |   |-- CD3_3_act_7_1_19.png
|       |   |   |-- ...
|       |   |   `-- CD8_3_act_6_6_24.png
|       |   `-- quiescent
|       |       |-- CD3_3_noact_8_1_110.png
|       |       |-- ...
|       |       `-- CD8_3_noact_5_5_91.png
|       |-- donor_4
|       |   |-- activated
|       |   |   |-- CD3_4_act_11_1_2.png
|       |   |   |-- ...
|       |   |   `-- CD8_4_act_3_6_64.png
|       |   `-- quiescent
|       |       |-- CD3_4_noact_12_1_104.png
|       |       |-- ...
|       |       `-- CD8_4_noact_1_6_93.png
|       |-- donor_5
|       |   |-- activated
|       |   |   |-- CD3_5_act_4_1_16.png
|       |   |   |-- ...
|       |   |   `-- CD8_5_act_7_4_18.png
|       |   `-- quiescent
|       |       |-- CD3_5_noact_1_2_3.png
|       |       |-- ...
|       |       `-- CD8_5_noact_8_4_6.png
|       `-- donor_6
|           |-- activated
|           |   |-- CD3_6_act_10_1_10.png
|           |   |-- ...
|           |   `-- CD8_6_act_11_6_51.png
|           `-- quiescent
|               |-- CD3_6_noact_9_1_2.png
|               |-- ...
|               `-- CD8_6_noact_12_5_9.png
`-- sample_images.zip

21 directories, 866 files
```
