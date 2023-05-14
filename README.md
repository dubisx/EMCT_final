
# EMCT_final
Repository for the EMCT final project. AI Assisted Musical Composition.

The notebooks are named after their specific use cases:

1. midi_encode_to_token.ipynb notebook handles encoding the MIDI dataset to tokens, as well as augmenting them to improve learning performance of the model.

2. tf_transformer_model_training.ipyng notebook handles token preprocessing and the training of the model, using Transformers and Tensorflow.

3. Generator.ipynb notebook is used to generate new musical compositions, and is the notebook you should be focusing on.



How to use (you can skip 1.x and 2.x steps if you only want to generate MIDI compositions): 

1.1. Choose or collect an appropriate MIDI dataset
1.2. Run the second notebook to encode the data to specified path.

2.1. Load in the tokenized dataset.
2.2. Run the cell that handles creating batches of Input and Target sequences.
2.3. Split the data to train/val/test subsets.
2.4. Initiate the model.
2.5. Train the model on the dataset.
2.6. Save the trained model and its weights to specified path.

3.1. Initialize the tokenizer, choose and initialize the model, and load in the model weights from their directories.
3.2. Select a MIDI file to use as a prompt. You can view the plotted piano roll and listen to the loaded file inside the notebook.
3.3. Configure generation settings and generate.
3.4. Save the midi file to specified path.

(optional)
3.5. Plot and view the generated MIDI in a piano roll.
3.6. Listen to the synthesized MIDI file.
3.7. Download the MIDI file.