# [NTIRE 2025 Challenge on Image Super-Resolution (x4)](https://cvlai.net/ntire/2025/) @ [CVPR 2025](https://cvpr.thecvf.com/)

### Environments

```sh
conda create -n NTIRE-SR python=3.8
conda activate NTIRE-SR
pip install -r requirements.txt
```

## How to test our ATM model?

1. `git clone https://github.com/EquationWalker/NTIRE25_ATM.git`

2.  Download Pretrained weight using `model_zoo/team10_atm/team10_atm.txt` and put it to `model_zoo/team10_atm/`.

3. Test our ATM model:

   ```bash
   CUDA_VISIBLE_DEVICES=0 python test.py --test_dir [path to test data dir] --save_dir [path to your save dir] --model_id 10
   ```

   -  Be sure the change the directories `--test_dir` and `--save_dir`.
