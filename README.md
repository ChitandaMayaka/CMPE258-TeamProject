# CMPE258-TeamProject
## Deep Reinforcement Learning based Self-driving car
### Software and Hardware
#### Software
* Windows10 (64-bit)
* Python 3.6
* Anaconda 5.2.0
* Tensorflow 1.8.0
* Tensorboard 1.8.0
#### Hardware
* CPU: Intel(R) Core(TM)i7-6700k CPU @ 4.00GHz
* GPU: NVIDIA GeForce GTX 2080 Ti 32GB
* Memory: 32 GB

### How to run this project
1. Clone repository
2. Run `DQN_image.ipynb` in `algorithm` folder

#### For training
1. In "Set environment path" cell set os according to your system among `Windows`, `Mac`, `Linux`. `train_mode = True`
2. In "Training or Inference" cell set `saver=tf.train.Saver(max_to_keep=4, keep_checkpoint_every_n_hours=2)`, input 2 for training when prompted

#### For testing
1. Create `tmp` folder under `algorithm` folder to store pre-trained model files for using. Copy the model file trained from saved_networks to `tmp`
2. In "Set environment path" cell set os according to your system among `Windows`, `Mac`, `Linux`. train_mode = False
3. In "Set Parameters" cell set `load_path = './tmp/model.ckpt'`
4. In "Training or Inference" cell set `saver=tf.train.import_meta_graph('./tmp/model.ckpt.meta')`, input 1 for inference when prompted

### Project Link
https://github.com/ChitandaMayaka/CMPE258-TeamProject
### Reference
https://github.com/MLJejuCamp2017/DRL_based_SelfDrivingCarControl
