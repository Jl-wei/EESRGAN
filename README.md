1. Create `saved` folder in this project, change the path at `config_GAN.json` and in other files
2. Download the datasets from [here](https://gdo152.llnl.gov/cowc/download/cowc-m/datasets/DetectionPatches_256x256.tgz)
3. Edit the dataset path at line 31, 32 of `scripts_for_datasets/prepare_image.py`, then run `python ./scripts_for_datasets/prepare_image.py`
4. Download pretrained model, and change the `pretrain_model_G`, `pretrain_model_D`, `pretrain_model_FRCNN` of `config_GAN.json`
5. Run `python test.py -c config_GAN.json` or `python train.py -c config_GAN.json`