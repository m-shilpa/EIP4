Total params: 14,586

Trainable params: 14,366

Non-trainable params: 220

**Score** : 99.49


**Logs of the 20 epoch:**


Train on 60000 samples, validate on 10000 samples
Epoch 1/20

Epoch 00001: LearningRateScheduler setting learning rate to 0.003.
60000/60000 [==============================] - 14s 228us/step - loss: 0.5366 - acc: 0.8492 - val_loss: 0.0984 - val_acc: 0.9799
Epoch 2/20

Epoch 00002: LearningRateScheduler setting learning rate to 0.0022744503.
60000/60000 [==============================] - 11s 176us/step - loss: 0.2571 - acc: 0.9220 - val_loss: 0.0531 - val_acc: 0.9886
Epoch 3/20

Epoch 00003: LearningRateScheduler setting learning rate to 0.0018315018.
60000/60000 [==============================] - 11s 175us/step - loss: 0.2043 - acc: 0.9369 - val_loss: 0.0396 - val_acc: 0.9908
Epoch 4/20

Epoch 00004: LearningRateScheduler setting learning rate to 0.0015329586.
60000/60000 [==============================] - 11s 176us/step - loss: 0.1703 - acc: 0.9461 - val_loss: 0.0356 - val_acc: 0.9908
Epoch 5/20

Epoch 00005: LearningRateScheduler setting learning rate to 0.0013181019.
60000/60000 [==============================] - 11s 176us/step - loss: 0.1553 - acc: 0.9486 - val_loss: 0.0295 - val_acc: 0.9928
Epoch 6/20

Epoch 00006: LearningRateScheduler setting learning rate to 0.0011560694.
60000/60000 [==============================] - 10s 175us/step - loss: 0.1418 - acc: 0.9508 - val_loss: 0.0273 - val_acc: 0.9929
Epoch 7/20

Epoch 00007: LearningRateScheduler setting learning rate to 0.0010295127.
60000/60000 [==============================] - 11s 176us/step - loss: 0.1306 - acc: 0.9527 - val_loss: 0.0264 - val_acc: 0.9927
Epoch 8/20

Epoch 00008: LearningRateScheduler setting learning rate to 0.0009279307.
60000/60000 [==============================] - 11s 176us/step - loss: 0.1243 - acc: 0.9537 - val_loss: 0.0256 - val_acc: 0.9932
Epoch 9/20

Epoch 00009: LearningRateScheduler setting learning rate to 0.0008445946.
60000/60000 [==============================] - 10s 175us/step - loss: 0.1211 - acc: 0.9529 - val_loss: 0.0233 - val_acc: 0.9933
Epoch 10/20

Epoch 00010: LearningRateScheduler setting learning rate to 0.0007749935.
60000/60000 [==============================] - 11s 176us/step - loss: 0.1156 - acc: 0.9538 - val_loss: 0.0226 - val_acc: 0.9926
Epoch 11/20

Epoch 00011: LearningRateScheduler setting learning rate to 0.0007159905.
60000/60000 [==============================] - 11s 177us/step - loss: 0.1108 - acc: 0.9549 - val_loss: 0.0208 - val_acc: 0.9937
Epoch 12/20

Epoch 00012: LearningRateScheduler setting learning rate to 0.000665336.
60000/60000 [==============================] - 11s 180us/step - loss: 0.1087 - acc: 0.9567 - val_loss: 0.0192 - val_acc: 0.9943
Epoch 13/20

Epoch 00013: LearningRateScheduler setting learning rate to 0.0006213753.
60000/60000 [==============================] - 11s 180us/step - loss: 0.1056 - acc: 0.9552 - val_loss: 0.0175 - val_acc: 0.9955
Epoch 14/20

Epoch 00014: LearningRateScheduler setting learning rate to 0.0005828638.
60000/60000 [==============================] - 11s 178us/step - loss: 0.1006 - acc: 0.9572 - val_loss: 0.0192 - val_acc: 0.9946
Epoch 15/20

Epoch 00015: LearningRateScheduler setting learning rate to 0.0005488474.
60000/60000 [==============================] - 11s 179us/step - loss: 0.1009 - acc: 0.9565 - val_loss: 0.0194 - val_acc: 0.9936
Epoch 16/20

Epoch 00016: LearningRateScheduler setting learning rate to 0.0005185825.
60000/60000 [==============================] - 11s 178us/step - loss: 0.1014 - acc: 0.9554 - val_loss: 0.0162 - val_acc: 0.9956
Epoch 17/20

Epoch 00017: LearningRateScheduler setting learning rate to 0.000491481.
60000/60000 [==============================] - 11s 179us/step - loss: 0.0969 - acc: 0.9575 - val_loss: 0.0172 - val_acc: 0.9946
Epoch 18/20

Epoch 00018: LearningRateScheduler setting learning rate to 0.0004670715.
60000/60000 [==============================] - 11s 179us/step - loss: 0.0945 - acc: 0.9582 - val_loss: 0.0172 - val_acc: 0.9945
Epoch 19/20

Epoch 00019: LearningRateScheduler setting learning rate to 0.0004449718.
60000/60000 [==============================] - 11s 178us/step - loss: 0.0953 - acc: 0.9582 - val_loss: 0.0166 - val_acc: 0.9950
Epoch 20/20

Epoch 00020: LearningRateScheduler setting learning rate to 0.000424869.
60000/60000 [==============================] - 11s 178us/step - loss: 0.0954 - acc: 0.9571 - val_loss: 0.0173 - val_acc: 0.9949



**Strategy taken to achieve the results** :

1. Went through all the 8 DNN code. 

2. Worked on the Eighth DNN code to achieve the target.

3. Decreased the no. of kernels in the 2nd convolution layer from 32 to 20 to decrease the parameters to 14,586.

4. Used the use_bias = False to exclude bias from the layer.

5. Trained the model for 20 epoch.

6. Achieved an accuracy of 99.49.

