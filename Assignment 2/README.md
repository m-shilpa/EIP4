Total params: 13,314

Trainable params: 13,122

Non-trainable params: 192

**Score** : 99.49


**Logs of the 20 epoch:**


Train on 60000 samples, validate on 10000 samples
Epoch 1/20

Epoch 00001: LearningRateScheduler setting learning rate to 0.003.
60000/60000 [==============================] - 14s 239us/step - loss: 0.2168 - acc: 0.9313 - val_loss: 0.0455 - val_acc: 0.9862
Epoch 2/20

Epoch 00002: LearningRateScheduler setting learning rate to 0.0022744503.
60000/60000 [==============================] - 8s 140us/step - loss: 0.0622 - acc: 0.9807 - val_loss: 0.0556 - val_acc: 0.9834
Epoch 3/20

Epoch 00003: LearningRateScheduler setting learning rate to 0.0018315018.
60000/60000 [==============================] - 8s 140us/step - loss: 0.0513 - acc: 0.9844 - val_loss: 0.0333 - val_acc: 0.9894
Epoch 4/20

Epoch 00004: LearningRateScheduler setting learning rate to 0.0015329586.
60000/60000 [==============================] - 9s 144us/step - loss: 0.0409 - acc: 0.9878 - val_loss: 0.0292 - val_acc: 0.9918
Epoch 5/20

Epoch 00005: LearningRateScheduler setting learning rate to 0.0013181019.
60000/60000 [==============================] - 9s 145us/step - loss: 0.0368 - acc: 0.9883 - val_loss: 0.0228 - val_acc: 0.9926
Epoch 6/20

Epoch 00006: LearningRateScheduler setting learning rate to 0.0011560694.
60000/60000 [==============================] - 9s 145us/step - loss: 0.0339 - acc: 0.9893 - val_loss: 0.0269 - val_acc: 0.9919
Epoch 7/20

Epoch 00007: LearningRateScheduler setting learning rate to 0.0010295127.
60000/60000 [==============================] - 8s 139us/step - loss: 0.0316 - acc: 0.9903 - val_loss: 0.0279 - val_acc: 0.9911
Epoch 8/20

Epoch 00008: LearningRateScheduler setting learning rate to 0.0009279307.
60000/60000 [==============================] - 9s 144us/step - loss: 0.0285 - acc: 0.9909 - val_loss: 0.0258 - val_acc: 0.9929
Epoch 9/20

Epoch 00009: LearningRateScheduler setting learning rate to 0.0008445946.
60000/60000 [==============================] - 8s 140us/step - loss: 0.0276 - acc: 0.9916 - val_loss: 0.0244 - val_acc: 0.9922
Epoch 10/20

Epoch 00010: LearningRateScheduler setting learning rate to 0.0007749935.
60000/60000 [==============================] - 9s 144us/step - loss: 0.0258 - acc: 0.9919 - val_loss: 0.0216 - val_acc: 0.9933
Epoch 11/20

Epoch 00011: LearningRateScheduler setting learning rate to 0.0007159905.
60000/60000 [==============================] - 8s 134us/step - loss: 0.0243 - acc: 0.9920 - val_loss: 0.0234 - val_acc: 0.9931
Epoch 12/20

Epoch 00012: LearningRateScheduler setting learning rate to 0.000665336.
60000/60000 [==============================] - 8s 136us/step - loss: 0.0239 - acc: 0.9922 - val_loss: 0.0198 - val_acc: 0.9944
Epoch 13/20

Epoch 00013: LearningRateScheduler setting learning rate to 0.0006213753.
60000/60000 [==============================] - 8s 138us/step - loss: 0.0227 - acc: 0.9922 - val_loss: 0.0201 - val_acc: 0.9941
Epoch 14/20

Epoch 00014: LearningRateScheduler setting learning rate to 0.0005828638.
60000/60000 [==============================] - 9s 142us/step - loss: 0.0208 - acc: 0.9934 - val_loss: 0.0234 - val_acc: 0.9936
Epoch 15/20

Epoch 00015: LearningRateScheduler setting learning rate to 0.0005488474.
60000/60000 [==============================] - 9s 143us/step - loss: 0.0200 - acc: 0.9937 - val_loss: 0.0204 - val_acc: 0.9942
Epoch 16/20

Epoch 00016: LearningRateScheduler setting learning rate to 0.0005185825.
60000/60000 [==============================] - 8s 135us/step - loss: 0.0203 - acc: 0.9937 - val_loss: 0.0201 - val_acc: 0.9945
Epoch 17/20

Epoch 00017: LearningRateScheduler setting learning rate to 0.000491481.
60000/60000 [==============================] - 9s 142us/step - loss: 0.0193 - acc: 0.9940 - val_loss: 0.0210 - val_acc: 0.9941
Epoch 18/20

Epoch 00018: LearningRateScheduler setting learning rate to 0.0004670715.
60000/60000 [==============================] - 8s 139us/step - loss: 0.0189 - acc: 0.9938 - val_loss: 0.0206 - val_acc: 0.9942
Epoch 19/20

Epoch 00019: LearningRateScheduler setting learning rate to 0.0004449718.
60000/60000 [==============================] - 8s 142us/step - loss: 0.0200 - acc: 0.9934 - val_loss: 0.0211 - val_acc: 0.9936
Epoch 20/20

Epoch 00020: LearningRateScheduler setting learning rate to 0.000424869.
60000/60000 [==============================] - 8s 138us/step - loss: 0.0171 - acc: 0.9941 - val_loss: 0.0179 - val_acc: 0.9949


**Strategy taken to achieve the results** :

1. Went through all the 8 DNN code. 

2. Worked on the Eighth DNN code to achieve the target.

3. Used the use_bias = False to exclude bias from the convolution layer.

4. Decreased the no. of kernels in the 2nd convolution layer from 32 to 20 and from 16 to 12 in the 7th layer which contributed to the  decrease in the no. of parameters.

5. Removed the BatchNormalization and Dropout from the last layer as it need not be used in the last layer.

6. Trained the model for 20 epoch.

7. Achieved an accuracy of 99.49.

