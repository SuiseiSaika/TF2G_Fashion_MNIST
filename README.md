# Dataset: Fashion MNIST
## Best Result:
## ●DNN_GGWP
### Model Structure:
#### Input size: (60000, 784)
#### Activation Function: Exponential Linear Units(ELUs)
#### Dense_Layer_1(units=128) - BatchNormalization()
#### Dense_Layer_2(units=128) - BatchNormalization()
#### Dense_Layer_3(units=256) - Dropout_Layer(rate=0.125) - BatchNormalization()
#### Dense_Layer_4(units=256) - Dropout_Layer(rate=0.125) - BatchNormalization()
#### Dense_Layer_5(units=512) - Dropout_Layer(rate=0.25) - BatchNormalization()
#### Dense_Layer_6(units=512) - Dropout_Layer(rate=0.25) - BatchNormalization()
#### Dense_Layer_7(units=256) - BatchNormalization()
#### Dense_Layer_8(units=128) - BatchNormalization()
#### Dense_Layer_9(units=64) - BatchNormalization()
#### Output_Layer(units=10) - Activation_Layer(Softmax)
### Data Augmentation:
#### width_shift_range=0.1
#### height_shift_range=0.1
#### horizontal_flip=True
### Phase 1
### Optimizer:
#### Adam, initial learning rate=1e-2
#### LearningRateScheduler: None
### Hyper Parameters:
#### epoch = 100
#### batch size = 128
### Result:
#### test loss: 0.3353
#### test accuracy: 0.8775
### Phase 2
### Optimizer:
#### Adam, initial learning rate=5e-3
#### LearningRateScheduler: None
### Hyper Parameters:
#### epoch = 100
#### batch size = 256
### Result:
#### test loss: 0.3245
#### test accuracy: 0.8853
### Phase 3
### Optimizer:
#### SGD, initial learning rate=5e-3
#### LearningRateScheduler: None
### Hyper Parameters:
#### epoch = 100
#### batch size = 512
### Result:
#### test loss: 0.3062
#### test accuracy: 0.8965
### Phase 4
### Optimizer:
#### SGD, initial learning rate=1e-3
#### LearningRateScheduler: None
### Hyper Parameters:
#### epoch = 50
#### batch size = 1024
### Result:
#### test loss: 0.2956
#### test accuracy: 0.9011
### Phase 5
### Optimizer:
#### SGD, initial learning rate=1e-3
#### LearningRateScheduler: None
### Hyper Parameters:
#### epoch = 50
#### batch size = 2048
### Result:
#### test loss: 0.2955
#### test accuracy: 0.9005
### Phase 6
### Optimizer:
#### SGD, initial learning rate=1e-4
#### LearningRateScheduler: None
### Hyper Parameters:
#### epoch = 50
#### batch size = 4096
### Result:
#### test loss: 0.2955
#### test accuracy: 0.9010

## ●DNN_Baseline
### Model Structure:
#### Input size: (60000, 784)
#### Activation Function: Exponential Linear Units(ELUs)
#### Dense_Layer_1(units=128) 
#### Dense_Layer_2(units=128)
#### Dense_Layer_3(units=256) 
#### Dense_Layer_4(units=256) 
#### Dense_Layer_5(units=512) 
#### Dense_Layer_6(units=512)
#### Output_Layer(units=10) - Activation_Layer(Softmax)
### Optimizer:
#### SGD, initial learning rate=0.01
#### LearningRateScheduler: drop 0.9 per 10 epochs
### Hyper Parameters:
#### epoch = 100
#### batch size = 256
### Result:
#### test loss: 0.2777
#### test accuracy: 0.8881

## ●DNN_Slim_Baseline
### Model Structure:
#### Input size: (60000, 784)
#### Activation Function: Exponential Linear Units(ELUs)
#### Dense_Layer_1(units=128)
#### Dense_Layer_2(units=128)
#### Dense_Layer_3(units=256)
#### Dense_Layer_4(units=256)
#### Dense_Layer_5(units=512)
#### Dense_Layer_6(units=512)
#### Dense_Layer_7(units=256)
#### Dense_Layer_8(units=128)
#### Dense_Layer_9(units=64)
#### Output_Layer(units=10) - Activation_Layer(Softmax)
### Optimizer:
#### SGD, initial learning rate=0.01
#### LearningRateScheduler: drop 0.9 per 10 epochs
### Hyper Parameters:
#### epoch = 100
#### batch size = 256
### Result:
#### test loss: 0.2219
#### test accuracy: 0.8842

## ●DNN_Normal
### Model Structure:
#### Input size: (60000, 784)
#### Activation Function: Exponential Linear Units(ELUs)
#### Dense_Layer_1(units=128) - Dropout_Layer(rate=0.125) - BatchNormalization()
#### Dense_Layer_2(units=128) - Dropout_Layer(rate=0.125) - BatchNormalization()
#### Dense_Layer_3(units=256) - Dropout_Layer(rate=0.25) - BatchNormalization()
#### Dense_Layer_4(units=256) - Dropout_Layer(rate=0.25) - BatchNormalization()
#### Dense_Layer_5(units=512) - Dropout_Layer(rate=0.5) - BatchNormalization()
#### Dense_Layer_6(units=512) - Dropout_Layer(rate=0.5) - BatchNormalization()
#### Output_Layer(units=10) - Activation_Layer(Softmax)
### Optimizer:
#### SGD, initial learning rate=0.1
#### LearningRateScheduler: drop 0.5 per 10 epochs
### Hyper Parameters:
#### epoch = 100
#### batch size = 256
### Result:
#### test loss: 0.4007
#### test accuracy: 0.8758

## ●DNN_Slim
### Model Structure:
#### Input size: (60000, 784)
#### Activation Function: Exponential Linear Units(ELUs)
#### Dense_Layer_1(units=128) - Dropout_Layer(rate=0.125) - BatchNormalization()
#### Dense_Layer_2(units=128) - Dropout_Layer(rate=0.125) - BatchNormalization()
#### Dense_Layer_3(units=256) - Dropout_Layer(rate=0.25) - BatchNormalization()
#### Dense_Layer_4(units=256) - Dropout_Layer(rate=0.25) - BatchNormalization()
#### Dense_Layer_5(units=512) - Dropout_Layer(rate=0.5) - BatchNormalization()
#### Dense_Layer_6(units=512) - Dropout_Layer(rate=0.5) - BatchNormalization()
#### Dense_Layer_7(units=256) - BatchNormalization()
#### Dense_Layer_8(units=128) - BatchNormalization()
#### Dense_Layer_9(units=64) - BatchNormalization()
#### Output_Layer(units=10) - Activation_Layer(Softmax)
### Optimizer:
#### SGD, initial learning rate=0.1
#### LearningRateScheduler: drop 0.5 per 10 epochs
### Hyper Parameters:
#### epoch = 100
#### batch size = 256
### Result:
#### test loss: 0.3796
#### test accuracy: 0.8740

## ●DNN_DataAugmentation_NADAM
### Model Structure:
#### Input size: (60000, 784)
#### Activation Function: Exponential Linear Units(ELUs)
#### Dense_Layer_1(units=128) - Dropout_Layer(rate=0.125) - BatchNormalization()
#### Dense_Layer_2(units=128) - Dropout_Layer(rate=0.125) - BatchNormalization()
#### Dense_Layer_3(units=256) - Dropout_Layer(rate=0.25) - BatchNormalization()
#### Dense_Layer_4(units=256) - Dropout_Layer(rate=0.25) - BatchNormalization()
#### Dense_Layer_5(units=512) - Dropout_Layer(rate=0.5) - BatchNormalization()
#### Dense_Layer_6(units=512) - Dropout_Layer(rate=0.5) - BatchNormalization()
#### Dense_Layer_7(units=256) - BatchNormalization()
#### Dense_Layer_8(units=128) - BatchNormalization()
#### Dense_Layer_9(units=64) - BatchNormalization()
#### Output_Layer(units=10) - Activation_Layer(Softmax)
### Optimizer:
#### NADAM, initial learning rate=0.002
#### LearningRateScheduler: None
### Hyper Parameters:
#### epoch = 100
#### batch size = 512
### Result:
#### test loss: 0.3689
#### test accuracy: 0.8702

## ●DNN_DataAugmentation_SGD
### Model Structure:
#### Input size: (60000, 784)
#### Activation Function: Exponential Linear Units(ELUs)
#### Dense_Layer_1(units=128) - Dropout_Layer(rate=0.125) - BatchNormalization()
#### Dense_Layer_2(units=128) - Dropout_Layer(rate=0.125) - BatchNormalization()
#### Dense_Layer_3(units=256) - Dropout_Layer(rate=0.25) - BatchNormalization()
#### Dense_Layer_4(units=256) - Dropout_Layer(rate=0.25) - BatchNormalization()
#### Dense_Layer_5(units=512) - Dropout_Layer(rate=0.5) - BatchNormalization()
#### Dense_Layer_6(units=512) - Dropout_Layer(rate=0.5) - BatchNormalization()
#### Dense_Layer_7(units=256) - BatchNormalization()
#### Dense_Layer_8(units=128) - BatchNormalization()
#### Dense_Layer_9(units=64) - BatchNormalization()
#### Output_Layer(units=10) - Activation_Layer(Softmax)
### Data Augmentation:
#### width_shift_range=0.1
#### height_shift_range=0.1
#### horizontal_flip=True
### Optimizer:
#### SGD, initial learning rate=0.1
#### LearningRateScheduler: drop 0.5 per 10 epochs
### Hyper Parameters:
#### epoch = 100
#### batch size = 512
### Result:
#### test loss: 0.5527
#### test accuracy: 0.7940

## ●DNN_DataAugmentation_SGD_1000epochtest
### Model Structure:
#### Input size: (60000, 784)
#### Activation Function: Exponential Linear Units(ELUs)
#### Dense_Layer_1(units=128) - Dropout_Layer(rate=0.125) - BatchNormalization()
#### Dense_Layer_2(units=128) - Dropout_Layer(rate=0.125) - BatchNormalization()
#### Dense_Layer_3(units=256) - Dropout_Layer(rate=0.25) - BatchNormalization()
#### Dense_Layer_4(units=256) - Dropout_Layer(rate=0.25) - BatchNormalization()
#### Dense_Layer_5(units=512) - Dropout_Layer(rate=0.5) - BatchNormalization()
#### Dense_Layer_6(units=512) - Dropout_Layer(rate=0.5) - BatchNormalization()
#### Dense_Layer_7(units=256) - BatchNormalization()
#### Dense_Layer_8(units=128) - BatchNormalization()
#### Dense_Layer_9(units=64) - BatchNormalization()
#### Output_Layer(units=10) - Activation_Layer(Softmax)
### Data Augmentation:
#### width_shift_range=0.1
#### height_shift_range=0.1
#### horizontal_flip=True
### Optimizer:
#### SGD, initial learning rate=0.1
#### LearningRateScheduler: drop 0.9 per 10 epochs
### Hyper Parameters:
#### epoch = 1000
#### batch size = 128
### Result:
#### test loss: 0.3232
#### test accuracy: 0.8699
