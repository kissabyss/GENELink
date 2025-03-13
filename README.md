## Graph attention network for link prediction of gene regulations from single cell RNA-sequencing data

![](https://github.com/zpliulab/GENELink/blob/main/Figure/Framework.jpg)

## Dependencies

- Python == 3.8
- Pytorch == 1.6.0
- scikit-learn==1.0.2
- numpy==1.20.3
- scanpy==1.7.2
- gseapy==0.10.8

## Usage

1. **Preparing for gene expression profiles and gene-gene adjacent matrix**

   GENELink integrates gene expression matrix **(N×M)** with prior gene topology **(N×N)** to learn low-dimensional vertorized representations with supervision.

2. **Command to run GENElink**

   To train an ab initio model, simply uses the script 'main.py'.

   ` python main.py`

   To apply dot product as score metric:

   Type == 'dot', flag== False

   To apply causal inference:

   Type == 'MLP', flag==True

## License

GENELink is licensed under the MIT License.

conda create -n GENElink python==3.8
conda activate GENElink
pip install numpy==1.20.3
pip install scanpy==1.7.2
pip install gseapy==0.10.8
pip install scikit-learn==1.0.2
pip install torch==1.6.0 torchvision==0.7.0
