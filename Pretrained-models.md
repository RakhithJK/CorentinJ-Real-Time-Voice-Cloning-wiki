Pretrained models come as an archive that contains **all three models** (speaker encoder, synthesizer, vocoder). The archive comes with the same directory structure as the repo, and you're expected to merge its contents with the root of the repository.

### Initial commit (latest release) [\[Google drive\]](https://drive.google.com/file/d/1n1sPXvT34yXFLT47QZA6FIRGrwMeSsZc/view?usp=sharing) [\[MEGA\]](https://megaupload.nz/F982Z8x6n5/pretrained_12_06_19_zip)

Please ensure the files are extracted to these locations within your local copy of the repository:
```
encoder\saved_models\pretrained.pt
synthesizer\saved_models\logs-pretrained\taco_pretrained\checkpoint
synthesizer\saved_models\logs-pretrained\taco_pretrained\tacotron_model.ckpt-278000.data-00000-of-00001
synthesizer\saved_models\logs-pretrained\taco_pretrained\tacotron_model.ckpt-278000.index
synthesizer\saved_models\logs-pretrained\taco_pretrained\tacotron_model.ckpt-278000.meta
vocoder\saved_models\pretrained\pretrained.pt
```

Here is some information about the models. For reference, the GPUs used for training are GTX 1080 Ti.
* **Encoder**: trained 1.56M steps (20 days with a single GPU) with a batch size of 64  
* **Synthesizer**: trained 278k steps (1 week with 4 GPUs) with a batch size of 144  
* **Vocoder**: trained 428k steps (4 days with a single GPU) with a batch size of 100