Pretrained models come as an archive that contains **all three models** (speaker encoder, synthesizer, vocoder). The archive comes with the same directory structure as the repo, and you're expected to merge its contents with the root of the repository.

### Initial commit (latest release) [\[Google drive\]](https://drive.google.com/file/d/1n1sPXvT34yXFLT47QZA6FIRGrwMeSsZc/view?usp=sharing) [\[Dropbox\]](https://www.dropbox.com/s/5udq50bkpw2hipy/pretrained.zip?dl=0)

Please ensure the files are extracted to these locations within your local copy of the repository:
```
encoder\saved_models\pretrained.pt
synthesizer\saved_models\logs-pretrained\taco_pretrained\checkpoint
synthesizer\saved_models\logs-pretrained\taco_pretrained\tacotron_model.ckpt-278000.data-00000-of-00001
synthesizer\saved_models\logs-pretrained\taco_pretrained\tacotron_model.ckpt-278000.index
synthesizer\saved_models\logs-pretrained\taco_pretrained\tacotron_model.ckpt-278000.meta
vocoder\saved_models\pretrained\pretrained.pt
```

If desired, the below checksums can be used to verify the integrity of pretrained.zip:
```
md5: 30459b5c0904110dc6b1447c28095554
sha1: 8e344861a76c52f9b73929a64357dc1776b640cb
sha256: 9dee6d64b2d9d1dd45b5d2d5c94ee3412e386d4b3378724a805e5e9418c7d255
```

Here is some information about the models. For reference, the GPUs used for training are GTX 1080 Ti.
* **Encoder**: trained 1.56M steps (20 days with a single GPU) with a batch size of 64  
* **Synthesizer**: trained 278k steps (1 week with 4 GPUs) with a batch size of 144  
* **Vocoder**: trained 428k steps (4 days with a single GPU) with a batch size of 100