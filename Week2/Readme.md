First 20 epochs:
  Train on 60000 samples, validate on 10000 samples
Epoch 1/20

Epoch 00001: LearningRateScheduler setting learning rate to 0.003.
60000/60000 [==============================] - 9s 146us/step - loss: 0.5521 - acc: 0.8426 - val_loss: 0.1040 - val_acc: 0.9816
Epoch 2/20

Epoch 00002: LearningRateScheduler setting learning rate to 0.0022744503.
60000/60000 [==============================] - 6s 98us/step - loss: 0.2627 - acc: 0.9199 - val_loss: 0.0587 - val_acc: 0.9882
Epoch 3/20

Epoch 00003: LearningRateScheduler setting learning rate to 0.0018315018.
60000/60000 [==============================] - 6s 98us/step - loss: 0.2033 - acc: 0.9378 - val_loss: 0.0515 - val_acc: 0.9881
Epoch 4/20

Epoch 00004: LearningRateScheduler setting learning rate to 0.0015329586.
60000/60000 [==============================] - 6s 97us/step - loss: 0.1735 - acc: 0.9455 - val_loss: 0.0378 - val_acc: 0.9911
Epoch 5/20

Epoch 00005: LearningRateScheduler setting learning rate to 0.0013181019.
60000/60000 [==============================] - 6s 98us/step - loss: 0.1573 - acc: 0.9472 - val_loss: 0.0306 - val_acc: 0.9922
Epoch 6/20

Epoch 00006: LearningRateScheduler setting learning rate to 0.0011560694.
60000/60000 [==============================] - 6s 97us/step - loss: 0.1476 - acc: 0.9490 - val_loss: 0.0297 - val_acc: 0.9912
Epoch 7/20

Epoch 00007: LearningRateScheduler setting learning rate to 0.0010295127.
60000/60000 [==============================] - 6s 97us/step - loss: 0.1365 - acc: 0.9512 - val_loss: 0.0357 - val_acc: 0.9902
Epoch 8/20

Epoch 00008: LearningRateScheduler setting learning rate to 0.0009279307.
60000/60000 [==============================] - 6s 96us/step - loss: 0.1291 - acc: 0.9523 - val_loss: 0.0290 - val_acc: 0.9925
Epoch 9/20

Epoch 00009: LearningRateScheduler setting learning rate to 0.0008445946.
60000/60000 [==============================] - 6s 97us/step - loss: 0.1249 - acc: 0.9516 - val_loss: 0.0269 - val_acc: 0.9927
Epoch 10/20

Epoch 00010: LearningRateScheduler setting learning rate to 0.0007749935.
60000/60000 [==============================] - 6s 97us/step - loss: 0.1184 - acc: 0.9537 - val_loss: 0.0343 - val_acc: 0.9898
Epoch 11/20

Epoch 00011: LearningRateScheduler setting learning rate to 0.0007159905.
60000/60000 [==============================] - 6s 100us/step - loss: 0.1152 - acc: 0.9539 - val_loss: 0.0245 - val_acc: 0.9927
Epoch 12/20

Epoch 00012: LearningRateScheduler setting learning rate to 0.000665336.
60000/60000 [==============================] - 6s 99us/step - loss: 0.1114 - acc: 0.9543 - val_loss: 0.0239 - val_acc: 0.9928
Epoch 13/20

Epoch 00013: LearningRateScheduler setting learning rate to 0.0006213753.
60000/60000 [==============================] - 6s 96us/step - loss: 0.1080 - acc: 0.9542 - val_loss: 0.0239 - val_acc: 0.9931
Epoch 14/20

Epoch 00014: LearningRateScheduler setting learning rate to 0.0005828638.
60000/60000 [==============================] - 6s 98us/step - loss: 0.1054 - acc: 0.9562 - val_loss: 0.0220 - val_acc: 0.9941
Epoch 15/20

Epoch 00015: LearningRateScheduler setting learning rate to 0.0005488474.
60000/60000 [==============================] - 6s 97us/step - loss: 0.1071 - acc: 0.9547 - val_loss: 0.0213 - val_acc: 0.9946
Epoch 16/20

Epoch 00016: LearningRateScheduler setting learning rate to 0.0005185825.
60000/60000 [==============================] - 6s 96us/step - loss: 0.1048 - acc: 0.9551 - val_loss: 0.0234 - val_acc: 0.9941
Epoch 17/20

Epoch 00017: LearningRateScheduler setting learning rate to 0.000491481.
60000/60000 [==============================] - 6s 95us/step - loss: 0.1011 - acc: 0.9557 - val_loss: 0.0236 - val_acc: 0.9932
Epoch 18/20

Epoch 00018: LearningRateScheduler setting learning rate to 0.0004670715.
60000/60000 [==============================] - 6s 96us/step - loss: 0.0986 - acc: 0.9577 - val_loss: 0.0203 - val_acc: 0.9949
Epoch 19/20

Epoch 00019: LearningRateScheduler setting learning rate to 0.0004449718.
60000/60000 [==============================] - 6s 96us/step - loss: 0.0986 - acc: 0.9566 - val_loss: 0.0215 - val_acc: 0.9948
Epoch 20/20

Epoch 00020: LearningRateScheduler setting learning rate to 0.000424869.
60000/60000 [==============================] - 6s 96us/step - loss: 0.0954 - acc: 0.9572 - val_loss: 0.0238 - val_acc: 0.9935
<keras.callbacks.History at 0x7fe3cd7b94a8>



#####################
Results on validation data:
[0.023769141756091267, 0.9935]

######################
For this I have reduced the number of channels in the 2nd convolution layer(from 32 to 25 of your code) and removed bias and changed the learning rate.
This have reduced the number of parameters and enhance accuracy.

I have also done some experients on changing Adam to SGD and using GAp and all are gining me accuracy > 99.4. 
Please go throuh the colab code. 
