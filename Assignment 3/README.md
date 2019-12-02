**Base Model - Validation Accuracy:** 81.85

**My Model - Validation Accuracy:** 81.70

**Model**

model = Sequential()

model.add(SeparableConv2D(32, kernel_size=(3, 3), strides=(1,1), input_shape=(32,32,3))) # o/p: 30 ,r:3

model.add(BatchNormalization())

model.add(Activation('relu'))

model.add(Dropout(0.15))

model.add(SeparableConv2D(64, kernel_size=(3, 3), strides=(1,1),kernel_regularizer=regularizers.l2(0.000001)))  # o/p: 28 ,r:5

model.add(BatchNormalization())

model.add(Activation('relu'))

model.add(Dropout(0.15))

model.add(SeparableConv2D(128, kernel_size=(3, 3), strides=(1,1),kernel_regularizer=regularizers.l2(0.000001)))  # o/p: 26 ,r:7

model.add(BatchNormalization())

model.add(Activation('relu'))

model.add(Dropout(0.15))

model.add(SeparableConv2D(256, kernel_size=(3, 3), strides=(1,1),kernel_regularizer=regularizers.l2(0.000001)))  # o/p: 24 ,r:9

model.add(BatchNormalization())

model.add(Activation('relu'))

model.add(Dropout(0.15))

model.add(MaxPooling2D(pool_size=(2,2))) # o/p: 12 r:10

model.add(SeparableConv2D(128, kernel_size=(3, 3), strides=(1,1),kernel_regularizer=regularizers.l2(0.000001)))  # o/p: 10 ,r:14

model.add(BatchNormalization())

model.add(Activation('relu'))

model.add(Dropout(0.15))

model.add(SeparableConv2D(10, kernel_size=(3, 3), strides=(1,1),kernel_regularizer=regularizers.l2(0.000001)))  # o/p: 8 ,r:18

model.add(GlobalAveragePooling2D())

model.add(Activation('softmax'))


**Logs**

Epoch 1/50

Epoch 00001: LearningRateScheduler setting learning rate to 0.003.
1562/1562 [==============================] - 50s 32ms/step - loss: 1.3709 - acc: 0.5059 - val_loss: 1.2684 - val_acc: 0.5463
Epoch 2/50

Epoch 00002: LearningRateScheduler setting learning rate to 0.0022744503.
1562/1562 [==============================] - 45s 29ms/step - loss: 1.0258 - acc: 0.6371 - val_loss: 1.0137 - val_acc: 0.6418
Epoch 3/50

Epoch 00003: LearningRateScheduler setting learning rate to 0.0018315018.
1562/1562 [==============================] - 45s 29ms/step - loss: 0.8922 - acc: 0.6862 - val_loss: 0.9901 - val_acc: 0.6656
Epoch 4/50

Epoch 00004: LearningRateScheduler setting learning rate to 0.0015329586.
1562/1562 [==============================] - 45s 29ms/step - loss: 0.8032 - acc: 0.7202 - val_loss: 0.8071 - val_acc: 0.7210
Epoch 5/50

Epoch 00005: LearningRateScheduler setting learning rate to 0.0013181019.
1562/1562 [==============================] - 45s 29ms/step - loss: 0.7453 - acc: 0.7393 - val_loss: 0.8510 - val_acc: 0.7096
Epoch 6/50

Epoch 00006: LearningRateScheduler setting learning rate to 0.0011560694.
1562/1562 [==============================] - 45s 29ms/step - loss: 0.6974 - acc: 0.7600 - val_loss: 0.7401 - val_acc: 0.7487
Epoch 7/50

Epoch 00007: LearningRateScheduler setting learning rate to 0.0010295127.
1562/1562 [==============================] - 45s 29ms/step - loss: 0.6632 - acc: 0.7683 - val_loss: 0.7856 - val_acc: 0.7322
Epoch 8/50

Epoch 00008: LearningRateScheduler setting learning rate to 0.0009279307.
1562/1562 [==============================] - 45s 29ms/step - loss: 0.6338 - acc: 0.7783 - val_loss: 0.6853 - val_acc: 0.7612
Epoch 9/50

Epoch 00009: LearningRateScheduler setting learning rate to 0.0008445946.
1562/1562 [==============================] - 45s 29ms/step - loss: 0.6030 - acc: 0.7897 - val_loss: 0.6703 - val_acc: 0.7701
Epoch 10/50

Epoch 00010: LearningRateScheduler setting learning rate to 0.0007749935.
1562/1562 [==============================] - 45s 29ms/step - loss: 0.5850 - acc: 0.7972 - val_loss: 0.6339 - val_acc: 0.7837
Epoch 11/50

Epoch 00011: LearningRateScheduler setting learning rate to 0.0007159905.
1562/1562 [==============================] - 45s 28ms/step - loss: 0.5639 - acc: 0.8030 - val_loss: 0.6262 - val_acc: 0.7834
Epoch 12/50

Epoch 00012: LearningRateScheduler setting learning rate to 0.000665336.
1562/1562 [==============================] - 44s 28ms/step - loss: 0.5491 - acc: 0.8086 - val_loss: 0.6346 - val_acc: 0.7833
Epoch 13/50

Epoch 00013: LearningRateScheduler setting learning rate to 0.0006213753.
1562/1562 [==============================] - 44s 28ms/step - loss: 0.5344 - acc: 0.8156 - val_loss: 0.6541 - val_acc: 0.7780
Epoch 14/50

Epoch 00014: LearningRateScheduler setting learning rate to 0.0005828638.
1562/1562 [==============================] - 45s 29ms/step - loss: 0.5185 - acc: 0.8200 - val_loss: 0.6526 - val_acc: 0.7778
Epoch 15/50

Epoch 00015: LearningRateScheduler setting learning rate to 0.0005488474.
1562/1562 [==============================] - 44s 28ms/step - loss: 0.5059 - acc: 0.8237 - val_loss: 0.6308 - val_acc: 0.7869
Epoch 16/50

Epoch 00016: LearningRateScheduler setting learning rate to 0.0005185825.
1562/1562 [==============================] - 45s 29ms/step - loss: 0.4961 - acc: 0.8278 - val_loss: 0.5692 - val_acc: 0.8079
Epoch 17/50

Epoch 00017: LearningRateScheduler setting learning rate to 0.000491481.
1562/1562 [==============================] - 45s 28ms/step - loss: 0.4861 - acc: 0.8305 - val_loss: 0.5759 - val_acc: 0.8072
Epoch 18/50

Epoch 00018: LearningRateScheduler setting learning rate to 0.0004670715.
1562/1562 [==============================] - 45s 29ms/step - loss: 0.4765 - acc: 0.8342 - val_loss: 0.5672 - val_acc: 0.8115
Epoch 19/50

Epoch 00019: LearningRateScheduler setting learning rate to 0.0004449718.
1562/1562 [==============================] - 44s 28ms/step - loss: 0.4683 - acc: 0.8370 - val_loss: 0.5726 - val_acc: 0.8084
Epoch 20/50

Epoch 00020: LearningRateScheduler setting learning rate to 0.000424869.
1562/1562 [==============================] - 44s 28ms/step - loss: 0.4559 - acc: 0.8411 - val_loss: 0.5748 - val_acc: 0.8055
Epoch 21/50

Epoch 00021: LearningRateScheduler setting learning rate to 0.0004065041.
1562/1562 [==============================] - 45s 29ms/step - loss: 0.4492 - acc: 0.8432 - val_loss: 0.5637 - val_acc: 0.8099
Epoch 22/50

Epoch 00022: LearningRateScheduler setting learning rate to 0.000389661.
1562/1562 [==============================] - 44s 28ms/step - loss: 0.4438 - acc: 0.8438 - val_loss: 0.5665 - val_acc: 0.8088
Epoch 23/50

Epoch 00023: LearningRateScheduler setting learning rate to 0.0003741581.
1562/1562 [==============================] - 44s 28ms/step - loss: 0.4376 - acc: 0.8479 - val_loss: 0.5458 - val_acc: 0.8163
Epoch 24/50

Epoch 00024: LearningRateScheduler setting learning rate to 0.0003598417.
1562/1562 [==============================] - 44s 28ms/step - loss: 0.4333 - acc: 0.8481 - val_loss: 0.5660 - val_acc: 0.8094
Epoch 25/50

Epoch 00025: LearningRateScheduler setting learning rate to 0.0003465804.
1562/1562 [==============================] - 45s 29ms/step - loss: 0.4307 - acc: 0.8500 - val_loss: 0.5487 - val_acc: 0.8157
Epoch 26/50

Epoch 00026: LearningRateScheduler setting learning rate to 0.0003342618.
1562/1562 [==============================] - 44s 28ms/step - loss: 0.4212 - acc: 0.8533 - val_loss: 0.5842 - val_acc: 0.8011
Epoch 27/50

Epoch 00027: LearningRateScheduler setting learning rate to 0.0003227889.
1562/1562 [==============================] - 44s 28ms/step - loss: 0.4186 - acc: 0.8528 - val_loss: 0.5463 - val_acc: 0.8174
Epoch 28/50

Epoch 00028: LearningRateScheduler setting learning rate to 0.0003120774.
1562/1562 [==============================] - 45s 29ms/step - loss: 0.4102 - acc: 0.8562 - val_loss: 0.5688 - val_acc: 0.8110
Epoch 29/50

Epoch 00029: LearningRateScheduler setting learning rate to 0.000302054.
1562/1562 [==============================] - 45s 29ms/step - loss: 0.4043 - acc: 0.8583 - val_loss: 0.5606 - val_acc: 0.8114
Epoch 30/50

Epoch 00030: LearningRateScheduler setting learning rate to 0.0002926544.
1562/1562 [==============================] - 44s 28ms/step - loss: 0.4043 - acc: 0.8583 - val_loss: 0.5541 - val_acc: 0.8178
Epoch 31/50

Epoch 00031: LearningRateScheduler setting learning rate to 0.0002838221.
1562/1562 [==============================] - 45s 29ms/step - loss: 0.3995 - acc: 0.8599 - val_loss: 0.5422 - val_acc: 0.8196
Epoch 32/50

Epoch 00032: LearningRateScheduler setting learning rate to 0.0002755074.
1562/1562 [==============================] - 45s 29ms/step - loss: 0.3941 - acc: 0.8611 - val_loss: 0.5560 - val_acc: 0.8144
Epoch 33/50

Epoch 00033: LearningRateScheduler setting learning rate to 0.000267666.
1562/1562 [==============================] - 45s 29ms/step - loss: 0.3934 - acc: 0.8632 - val_loss: 0.5697 - val_acc: 0.8111
Epoch 34/50

Epoch 00034: LearningRateScheduler setting learning rate to 0.0002602585.
1562/1562 [==============================] - 45s 29ms/step - loss: 0.3863 - acc: 0.8636 - val_loss: 0.5450 - val_acc: 0.8202
Epoch 35/50

Epoch 00035: LearningRateScheduler setting learning rate to 0.00025325.
1562/1562 [==============================] - 45s 29ms/step - loss: 0.3835 - acc: 0.8651 - val_loss: 0.5650 - val_acc: 0.8115
Epoch 36/50

Epoch 00036: LearningRateScheduler setting learning rate to 0.0002466091.
1562/1562 [==============================] - 45s 29ms/step - loss: 0.3796 - acc: 0.8665 - val_loss: 0.5539 - val_acc: 0.8151
Epoch 37/50

Epoch 00037: LearningRateScheduler setting learning rate to 0.0002403076.
1562/1562 [==============================] - 45s 29ms/step - loss: 0.3782 - acc: 0.8660 - val_loss: 0.5474 - val_acc: 0.8167
Epoch 38/50

Epoch 00038: LearningRateScheduler setting learning rate to 0.0002343201.
1562/1562 [==============================] - 45s 29ms/step - loss: 0.3761 - acc: 0.8682 - val_loss: 0.5556 - val_acc: 0.8159
Epoch 39/50

Epoch 00039: LearningRateScheduler setting learning rate to 0.0002286237.
1562/1562 [==============================] - 45s 29ms/step - loss: 0.3713 - acc: 0.8700 - val_loss: 0.5511 - val_acc: 0.8165
Epoch 40/50

Epoch 00040: LearningRateScheduler setting learning rate to 0.0002231977.
1562/1562 [==============================] - 45s 29ms/step - loss: 0.3712 - acc: 0.8690 - val_loss: 0.5521 - val_acc: 0.8165
Epoch 41/50

Epoch 00041: LearningRateScheduler setting learning rate to 0.0002180233.
1562/1562 [==============================] - 45s 29ms/step - loss: 0.3619 - acc: 0.8719 - val_loss: 0.5620 - val_acc: 0.8124
Epoch 42/50

Epoch 00042: LearningRateScheduler setting learning rate to 0.0002130833.
1562/1562 [==============================] - 45s 29ms/step - loss: 0.3657 - acc: 0.8702 - val_loss: 0.5501 - val_acc: 0.8168
Epoch 43/50

Epoch 00043: LearningRateScheduler setting learning rate to 0.0002083623.
1562/1562 [==============================] - 45s 29ms/step - loss: 0.3620 - acc: 0.8705 - val_loss: 0.5420 - val_acc: 0.8182
Epoch 44/50

Epoch 00044: LearningRateScheduler setting learning rate to 0.0002038459.
1562/1562 [==============================] - 45s 29ms/step - loss: 0.3582 - acc: 0.8738 - val_loss: 0.5628 - val_acc: 0.8123
Epoch 45/50

Epoch 00045: LearningRateScheduler setting learning rate to 0.0001995211.
1562/1562 [==============================] - 45s 29ms/step - loss: 0.3551 - acc: 0.8764 - val_loss: 0.5460 - val_acc: 0.8183
Epoch 46/50

Epoch 00046: LearningRateScheduler setting learning rate to 0.0001953761.
1562/1562 [==============================] - 45s 29ms/step - loss: 0.3542 - acc: 0.8736 - val_loss: 0.5456 - val_acc: 0.8204
Epoch 47/50

Epoch 00047: LearningRateScheduler setting learning rate to 0.0001913998.
1562/1562 [==============================] - 45s 29ms/step - loss: 0.3531 - acc: 0.8768 - val_loss: 0.5479 - val_acc: 0.8183
Epoch 48/50

Epoch 00048: LearningRateScheduler setting learning rate to 0.0001875821.
1562/1562 [==============================] - 45s 29ms/step - loss: 0.3498 - acc: 0.8763 - val_loss: 0.5355 - val_acc: 0.8224
Epoch 49/50

Epoch 00049: LearningRateScheduler setting learning rate to 0.0001839137.
1562/1562 [==============================] - 45s 29ms/step - loss: 0.3464 - acc: 0.8776 - val_loss: 0.5429 - val_acc: 0.8194
Epoch 50/50

Epoch 00050: LearningRateScheduler setting learning rate to 0.000180386.
1562/1562 [==============================] - 45s 29ms/step - loss: 0.3457 - acc: 0.8793 - val_loss: 0.5470 - val_acc: 0.8170
Model took 2243.26 seconds to train
