**Base Model - Validation Accuracy:** 82.3
**My Model - Validation Accuracy:** 80.54

**Model**


model = Sequential()

model.add(SeparableConv2D(32, kernel_size=(3, 3), activation='relu', strides=(1,1), input_shape=(32,32,3))) # o/p: 30, r: 3
model.add(Convolution2D(32, 1, 1))  # o/p: 30, r: 3
model.add(BatchNormalization())
model.add(Dropout(0.15))

model.add(SeparableConv2D(64, kernel_size=(3, 3), activation='relu',strides=(2,2))) # o/p: 14, r: 5
model.add(Convolution2D(64, 1, 1))  # o/p: 14, r: 5
model.add(BatchNormalization())
model.add(Dropout(0.15))

model.add(SeparableConv2D(128, kernel_size=(3, 3), activation='relu',strides=(1,1))) # o/p: 12, r: 9
model.add(Convolution2D(128, 1, 1)) # o/p: 12, r: 9
model.add(BatchNormalization())
model.add(Dropout(0.15))

model.add(SeparableConv2D(256, kernel_size=(3, 3), activation='relu',strides=(2,2))) # o/p: 5, r: 13
model.add(BatchNormalization())
model.add(Dropout(0.15))

model.add(SeparableConv2D(10, kernel_size=(5, 5), activation='relu',strides=(1,1))) # o/p: 1, r: 29
model.add(Flatten())
model.add(Activation('softmax'))

**Logs**

Epoch 1/50

Epoch 00001: LearningRateScheduler setting learning rate to 0.003.
1562/1562 [==============================] - 21s 13ms/step - loss: 1.3588 - acc: 0.5207 - val_loss: 1.2498 - val_acc: 0.5843
Epoch 2/50

Epoch 00002: LearningRateScheduler setting learning rate to 0.0022744503.
1562/1562 [==============================] - 19s 12ms/step - loss: 1.0069 - acc: 0.6504 - val_loss: 0.9416 - val_acc: 0.6749
Epoch 3/50

Epoch 00003: LearningRateScheduler setting learning rate to 0.0018315018.
1562/1562 [==============================] - 19s 12ms/step - loss: 0.8797 - acc: 0.6940 - val_loss: 1.0726 - val_acc: 0.6403
Epoch 4/50

Epoch 00004: LearningRateScheduler setting learning rate to 0.0015329586.
1562/1562 [==============================] - 20s 13ms/step - loss: 0.8005 - acc: 0.7216 - val_loss: 0.8252 - val_acc: 0.7170
Epoch 5/50

Epoch 00005: LearningRateScheduler setting learning rate to 0.0013181019.
1562/1562 [==============================] - 20s 13ms/step - loss: 0.7438 - acc: 0.7415 - val_loss: 0.7521 - val_acc: 0.7419
Epoch 6/50

Epoch 00006: LearningRateScheduler setting learning rate to 0.0011560694.
1562/1562 [==============================] - 20s 13ms/step - loss: 0.6986 - acc: 0.7571 - val_loss: 0.7112 - val_acc: 0.7565
Epoch 7/50

Epoch 00007: LearningRateScheduler setting learning rate to 0.0010295127.
1562/1562 [==============================] - 20s 13ms/step - loss: 0.6638 - acc: 0.7699 - val_loss: 0.7264 - val_acc: 0.7484
Epoch 8/50

Epoch 00008: LearningRateScheduler setting learning rate to 0.0009279307.
1562/1562 [==============================] - 19s 12ms/step - loss: 0.6401 - acc: 0.7776 - val_loss: 0.6790 - val_acc: 0.7667
Epoch 9/50

Epoch 00009: LearningRateScheduler setting learning rate to 0.0008445946.
1562/1562 [==============================] - 20s 13ms/step - loss: 0.6150 - acc: 0.7867 - val_loss: 0.6665 - val_acc: 0.7714
Epoch 10/50

Epoch 00010: LearningRateScheduler setting learning rate to 0.0007749935.
1562/1562 [==============================] - 20s 13ms/step - loss: 0.5847 - acc: 0.7962 - val_loss: 0.6744 - val_acc: 0.7706
Epoch 11/50

Epoch 00011: LearningRateScheduler setting learning rate to 0.0007159905.
1562/1562 [==============================] - 20s 13ms/step - loss: 0.5719 - acc: 0.8004 - val_loss: 0.6639 - val_acc: 0.7760
Epoch 12/50

Epoch 00012: LearningRateScheduler setting learning rate to 0.000665336.
1562/1562 [==============================] - 20s 13ms/step - loss: 0.5572 - acc: 0.8056 - val_loss: 0.6440 - val_acc: 0.7805
Epoch 13/50

Epoch 00013: LearningRateScheduler setting learning rate to 0.0006213753.
1562/1562 [==============================] - 20s 13ms/step - loss: 0.5441 - acc: 0.8113 - val_loss: 0.7014 - val_acc: 0.7651
Epoch 14/50

Epoch 00014: LearningRateScheduler setting learning rate to 0.0005828638.
1562/1562 [==============================] - 20s 13ms/step - loss: 0.5281 - acc: 0.8148 - val_loss: 0.6430 - val_acc: 0.7821
Epoch 15/50

Epoch 00015: LearningRateScheduler setting learning rate to 0.0005488474.
1562/1562 [==============================] - 20s 13ms/step - loss: 0.5144 - acc: 0.8220 - val_loss: 0.6297 - val_acc: 0.7852
Epoch 16/50

Epoch 00016: LearningRateScheduler setting learning rate to 0.0005185825.
1562/1562 [==============================] - 20s 13ms/step - loss: 0.5047 - acc: 0.8227 - val_loss: 0.6371 - val_acc: 0.7857
Epoch 17/50

Epoch 00017: LearningRateScheduler setting learning rate to 0.000491481.
1562/1562 [==============================] - 20s 13ms/step - loss: 0.4955 - acc: 0.8268 - val_loss: 0.6286 - val_acc: 0.7904
Epoch 18/50

Epoch 00018: LearningRateScheduler setting learning rate to 0.0004670715.
1562/1562 [==============================] - 20s 13ms/step - loss: 0.4858 - acc: 0.8300 - val_loss: 0.6238 - val_acc: 0.7945
Epoch 19/50

Epoch 00019: LearningRateScheduler setting learning rate to 0.0004449718.
1562/1562 [==============================] - 20s 13ms/step - loss: 0.4760 - acc: 0.8321 - val_loss: 0.6453 - val_acc: 0.7832
Epoch 20/50

Epoch 00020: LearningRateScheduler setting learning rate to 0.000424869.
1562/1562 [==============================] - 20s 13ms/step - loss: 0.4717 - acc: 0.8353 - val_loss: 0.6557 - val_acc: 0.7831
Epoch 21/50

Epoch 00021: LearningRateScheduler setting learning rate to 0.0004065041.
1562/1562 [==============================] - 20s 13ms/step - loss: 0.4632 - acc: 0.8394 - val_loss: 0.6363 - val_acc: 0.7896
Epoch 22/50

Epoch 00022: LearningRateScheduler setting learning rate to 0.000389661.
1562/1562 [==============================] - 20s 13ms/step - loss: 0.4545 - acc: 0.8402 - val_loss: 0.6259 - val_acc: 0.7964
Epoch 23/50

Epoch 00023: LearningRateScheduler setting learning rate to 0.0003741581.
1562/1562 [==============================] - 20s 13ms/step - loss: 0.4534 - acc: 0.8422 - val_loss: 0.6253 - val_acc: 0.7903
Epoch 24/50

Epoch 00024: LearningRateScheduler setting learning rate to 0.0003598417.
1562/1562 [==============================] - 20s 13ms/step - loss: 0.4432 - acc: 0.8461 - val_loss: 0.6176 - val_acc: 0.7955
Epoch 25/50

Epoch 00025: LearningRateScheduler setting learning rate to 0.0003465804.
1562/1562 [==============================] - 19s 12ms/step - loss: 0.4421 - acc: 0.8445 - val_loss: 0.6238 - val_acc: 0.7949
Epoch 26/50

Epoch 00026: LearningRateScheduler setting learning rate to 0.0003342618.
1562/1562 [==============================] - 20s 13ms/step - loss: 0.4364 - acc: 0.8477 - val_loss: 0.6270 - val_acc: 0.7954
Epoch 27/50

Epoch 00027: LearningRateScheduler setting learning rate to 0.0003227889.
1562/1562 [==============================] - 20s 13ms/step - loss: 0.4311 - acc: 0.8492 - val_loss: 0.6258 - val_acc: 0.7974
Epoch 28/50

Epoch 00028: LearningRateScheduler setting learning rate to 0.0003120774.
1562/1562 [==============================] - 20s 13ms/step - loss: 0.4261 - acc: 0.8485 - val_loss: 0.6266 - val_acc: 0.7962
Epoch 29/50

Epoch 00029: LearningRateScheduler setting learning rate to 0.000302054.
1562/1562 [==============================] - 20s 12ms/step - loss: 0.4194 - acc: 0.8534 - val_loss: 0.6281 - val_acc: 0.7950
Epoch 30/50

Epoch 00030: LearningRateScheduler setting learning rate to 0.0002926544.
1562/1562 [==============================] - 20s 13ms/step - loss: 0.4216 - acc: 0.8511 - val_loss: 0.6189 - val_acc: 0.7974
Epoch 31/50

Epoch 00031: LearningRateScheduler setting learning rate to 0.0002838221.
1562/1562 [==============================] - 20s 13ms/step - loss: 0.4189 - acc: 0.8516 - val_loss: 0.6247 - val_acc: 0.7987
Epoch 32/50

Epoch 00032: LearningRateScheduler setting learning rate to 0.0002755074.
1562/1562 [==============================] - 20s 13ms/step - loss: 0.4106 - acc: 0.8566 - val_loss: 0.6221 - val_acc: 0.7993
Epoch 33/50

Epoch 00033: LearningRateScheduler setting learning rate to 0.000267666.
1562/1562 [==============================] - 19s 12ms/step - loss: 0.4104 - acc: 0.8543 - val_loss: 0.6187 - val_acc: 0.7982
Epoch 34/50

Epoch 00034: LearningRateScheduler setting learning rate to 0.0002602585.
1562/1562 [==============================] - 20s 13ms/step - loss: 0.4046 - acc: 0.8559 - val_loss: 0.6287 - val_acc: 0.7945
Epoch 35/50

Epoch 00035: LearningRateScheduler setting learning rate to 0.00025325.
1562/1562 [==============================] - 20s 13ms/step - loss: 0.4007 - acc: 0.8580 - val_loss: 0.6215 - val_acc: 0.7998
Epoch 36/50

Epoch 00036: LearningRateScheduler setting learning rate to 0.0002466091.
1562/1562 [==============================] - 19s 12ms/step - loss: 0.3981 - acc: 0.8597 - val_loss: 0.6217 - val_acc: 0.7991
Epoch 37/50

Epoch 00037: LearningRateScheduler setting learning rate to 0.0002403076.
1562/1562 [==============================] - 20s 13ms/step - loss: 0.3933 - acc: 0.8607 - val_loss: 0.6204 - val_acc: 0.8022
Epoch 38/50

Epoch 00038: LearningRateScheduler setting learning rate to 0.0002343201.
1562/1562 [==============================] - 20s 13ms/step - loss: 0.3881 - acc: 0.8620 - val_loss: 0.6343 - val_acc: 0.7983
Epoch 39/50

Epoch 00039: LearningRateScheduler setting learning rate to 0.0002286237.
1562/1562 [==============================] - 19s 12ms/step - loss: 0.3928 - acc: 0.8607 - val_loss: 0.6202 - val_acc: 0.8029
Epoch 40/50

Epoch 00040: LearningRateScheduler setting learning rate to 0.0002231977.
1562/1562 [==============================] - 20s 13ms/step - loss: 0.3826 - acc: 0.8644 - val_loss: 0.6197 - val_acc: 0.8038
Epoch 41/50

Epoch 00041: LearningRateScheduler setting learning rate to 0.0002180233.
1562/1562 [==============================] - 20s 13ms/step - loss: 0.3873 - acc: 0.8630 - val_loss: 0.6223 - val_acc: 0.8027
Epoch 42/50

Epoch 00042: LearningRateScheduler setting learning rate to 0.0002130833.
1562/1562 [==============================] - 20s 13ms/step - loss: 0.3768 - acc: 0.8676 - val_loss: 0.6267 - val_acc: 0.8034
Epoch 43/50

Epoch 00043: LearningRateScheduler setting learning rate to 0.0002083623.
1562/1562 [==============================] - 20s 13ms/step - loss: 0.3803 - acc: 0.8663 - val_loss: 0.6235 - val_acc: 0.8029
Epoch 44/50

Epoch 00044: LearningRateScheduler setting learning rate to 0.0002038459.
1562/1562 [==============================] - 20s 13ms/step - loss: 0.3785 - acc: 0.8653 - val_loss: 0.6286 - val_acc: 0.8017
Epoch 45/50

Epoch 00045: LearningRateScheduler setting learning rate to 0.0001995211.
1562/1562 [==============================] - 20s 13ms/step - loss: 0.3742 - acc: 0.8687 - val_loss: 0.6222 - val_acc: 0.8032
Epoch 46/50

Epoch 00046: LearningRateScheduler setting learning rate to 0.0001953761.
1562/1562 [==============================] - 20s 13ms/step - loss: 0.3734 - acc: 0.8690 - val_loss: 0.6253 - val_acc: 0.8018
Epoch 47/50

Epoch 00047: LearningRateScheduler setting learning rate to 0.0001913998.
1562/1562 [==============================] - 20s 13ms/step - loss: 0.3680 - acc: 0.8697 - val_loss: 0.6231 - val_acc: 0.8059
Epoch 48/50

Epoch 00048: LearningRateScheduler setting learning rate to 0.0001875821.
1562/1562 [==============================] - 20s 13ms/step - loss: 0.3694 - acc: 0.8696 - val_loss: 0.6297 - val_acc: 0.8035
Epoch 49/50

Epoch 00049: LearningRateScheduler setting learning rate to 0.0001839137.
1562/1562 [==============================] - 20s 13ms/step - loss: 0.3665 - acc: 0.8707 - val_loss: 0.6218 - val_acc: 0.8064
Epoch 50/50

Epoch 00050: LearningRateScheduler setting learning rate to 0.000180386.
1562/1562 [==============================] - 20s 13ms/step - loss: 0.3660 - acc: 0.8708 - val_loss: 0.6284 - val_acc: 0.8054
