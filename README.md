# MolGAN
AI for a cure, a combination of Laten-GAN and VAE-JTNN to create 100% valid drug like molecules

Models, trainer and data_utils modified from original [LatentGan](https://github.com/Dierme/latent-gan)

Encoder and decoder for VAE-JTNN modified from [Mol-CycleGAN](https://github.com/ardigen/mol-cycle-gan)

Pretrained latent space also used from Mol-CycleGAN, and used pretrained decoder wieghts from [VAE-JTNN repository](https://github.com/wengong-jin/icml18-jtnn)

I recommend using the models in a jupyter notebook and to get the required data set using:
```
!wget http://molcyclegan.ardigen.com/X_JTVAE_250k_rndm_zinc.csv
```

For training, you can directly run the notebook within the repository.

Then due to environment constraints and requirements of the original VAE-JTNN repository, create the required environment using conda:
```
conda create env -f environment.py
```

Then just use:
```
python decode.py
```
Check at the bottom of the decode.py file for specifics on fields to set data path and file to decode path

