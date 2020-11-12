# Mixed-use decomposition

## Title: A framework for mixed-use decomposition based on temporal activity signatures extracted from big geo-data

## Abstract
Mixed use has been extensively applied as an urban planning principle and hinders the study of single urban functions. To address this problem, it is worth decomposing the mixed use. Inspired by the concept of spectral unmixing in remote sensing applications, this paper proposes a framework for mixed-use decomposition based on big geo-data. Mixed-use decomposition in terms of human activities differs from traditional land use research, and it is more reasonable to infer the actual urban function of land. The framework consists of four steps, namely temporal activity signature extraction, urban function base curve extraction, mixed-use decomposition, and result validation. First, the temporal activity signatures (TASs) of each zone are extracted as the proxy of human activity patterns. Second, the diurnal TASs of routine activities are extracted as urban function base curves (i.e. endmembers). Third, a linear decomposition model is used to decompose the mixed use and obtain multiple results (urban function composition, dynamic activity proportions, and the mixing index). Finally, result validation strategies are concluded. This framework offers method extensibility and has few requirements for the input data. It is validated by means of a case study of Beijing, based on a social media check-in dataset.

## Code description
The Jupyter Notebook file "mixed-use decomposition.ipynb" is the program to decompose temporal activity signatures (TASs) and obtain multiple results include urban function composition, dynamic activity proportions, and the mixing index. The program's inputs include extracted base curves (.csv) and observed TASs (.csv). Outputs are currently prints and easy to be organized as files. The decomposition is implemented based on the linear model using the [scipy.optimize](https://docs.scipy.org/doc/scipy/reference/optimize.html#module-scipy.optimize) in Python.

Please note that the program doesn't include the contents on data organization, base curve extraction, and result validation.

## Sample data
Sample data supporting the program include observed TASs (observed.csv) and extracted base curves (basecurve.csv). For both files, each row represents a curve (i.e., TAS or base curve), and columns represent corresponding temporal dimensions. All the curves are real and processed by sum normalization. Observed TASs are sampled from 451 zones. Base curves are detected based on POI types (illustrated in Figure 4(d) of the published article).

## Cite
Please consider citing our paper if this helps in your work:

Lun Wu, Ximeng Cheng, Chaogui Kang, Di Zhu, Zhou Huang & Yu Liu (2020). A framework for mixed-use decomposition based on temporal activity signatures extracted from big geo-data. International Journal of Digital Earth. 13:6, 708-726. [DOI](https://doi.org/10.1080/17538947.2018.1556353)
