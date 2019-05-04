# BachRNN

Within magenta, we install everything magenta and collected a dataset within Polypony-RNN. 
We then trained and generated data using command line calls such as:

polyphony_rnn_train --run_dir=/tmp/polyphony_rnn/logdir/run1 --sequence_example_file=/tmp/polyphony_rnn/sequence_examples/training_poly_tracks.tfrecord --hparams="batch_size=64,rnn_layer_sizes=[64,64]" --num_training_steps=15000

polyphony_rnn_generate --run_dir=/tmp/polyphony_rnn/logdir/run2 --hparams="batch_size=64,rnn_layer_sizes=[64,64]" --output_dir=/tmp/polyphony_rnn/generated2 --num_outputs=10 --num_steps=512 --primer_pitches="[67,64,60]" --condition_on_primer=true --inject_primer_during_generation=false

After running numerous trials, you can use the neural-transfer-audio directory, where if you run the Jupyter notebook you can combine styles.
