### Implementation
- [ ] Let the user decide if they want to use speaker embeddings or utterance embeddings for training the synthesizer.
- [ ] Multi-GPU training support for the encoder
- [ ] Figure out which device is best to compute the loss on the encoder
- [ ] Move on to a pytorch implementation of the synthesizer?
- [ ] Post-generation cleaning routines for the vocoder?

### Toolbox
- [ ] Handle multiple users in the toolbox
- [ ] Allow for saving generated wavs in the toolbox
- [ ] Use the top left space to draw a legend (rather than doing it inside the plot), and give the possibility to remove speakers from there
- [x] Display vocoder generation

### Code style
- [ ] Object-oriented inference rather than the current static style
- [ ] Setup a config file to allow for default argparse values (mainly datasets_root).
- [ ] Change the structure of the hparams file for each model. I think a namespace is the better solution.
- [ ] Properly document all inference functions
