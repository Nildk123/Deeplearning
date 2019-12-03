# Validation accuracy for the base network given by 81.76

# Final Validation Accuracy 82.97 and best 83.02 at 45th epoch

# model definition
#  Layer 1
SeparableConv2D(filters= 32, kernel_size= (3,3), input_shape = (32,  32,  3), padding= 'same', activation= 'relu', use_bias= False)
BatchNormalization()
Dropout(0.05)
#output shape: (32\*32*32)
#receptive field:  3
#  Layer 2
SeparableConv2D(filters= 32, kernel_size= (3,3), activation= 'relu', use_bias= False, padding= 'same')
BatchNormalization()
Dropout(0.05)
#output shape:(32\*32*32)
#receptive field: 5
#  Layer 3
SeparableConv2D(filters= 32, kernel_size= (3,3), activation= 'relu', use_bias= False, padding= 'same')
BatchNormalization()
Dropout(0.05)
#output shape:(32\*32*32)
#receptive field: 7
#  Layer 4
SeparableConv2D(filters= 32, kernel_size= (3,3), activation= 'relu', use_bias= False)
BatchNormalization()
Dropout(0.05)
#output shape:(30\*30*32)
#receptive field: 9
#  Layer 5
SeparableConv2D(filters= 64, kernel_size= (3,3), activation= 'relu', use_bias= False, padding= 'same')
BatchNormalization()
Dropout(0.05)
#output shape:(30\*30*64)
#receptive field: 11
#  Layer 6
SeparableConv2D(filters= 64, kernel_size= (3,3), activation= 'relu', use_bias= False, padding= 'same')
BatchNormalization()
Dropout(0.05)
#output shape:(30\*30*64)
#receptive field: 13
#  Layer 7
SeparableConv2D(filters= 64, kernel_size= (3,3), activation= 'relu', use_bias= False)
BatchNormalization()
Dropout(0.05)
#output shape:(28\*28*64)
#receptive field: 15
#  Layer 8
SeparableConv2D(filters= 96, kernel_size= (3,3), activation= 'relu', use_bias= False, strides=(2,2))
BatchNormalization()
Dropout(0.05)
#output shape:(13\*13*96)
#receptive field: 17
#  Layer 9
SeparableConv2D(filters= 96, kernel_size= (3,3), activation= 'relu', use_bias= False)
BatchNormalization()
Dropout(0.05)
#output shape:(11\*11*96)
#receptive field: 21
#  Layer 10
SeparableConv2D(filters= 96, kernel_size= (3,3), activation= 'relu', use_bias= False)
BatchNormalization()
Dropout(0.05)
#output shape:(9\*9*96)
#receptive field: 25
#  Layer 11
SeparableConv2D(filters= 128, kernel_size= (3,3), activation= 'relu', use_bias= False, padding= 'same')
BatchNormalization()
Dropout(0.05)
#output shape:(9\*9*128)
#receptive field: 29
#  Layer 12
SeparableConv2D(filters= 128, kernel_size= (3,3), activation= 'relu', use_bias= False, strides=(2,2))
BatchNormalization()
Dropout(0.05)
#output shape:(4\*4*128)
#receptive field: 33
#  Layer 13
SeparableConv2D(filters= 128, kernel_size= (3,3), activation= 'relu', use_bias= False, padding= 'same')
BatchNormalization()
Dropout(0.05)
#output shape:(4\*4*128)
#receptive field: 41
#  Layer 14
SeparableConv2D(filters= 10, kernel_size= (1,1), activation= 'relu', use_bias= False)
BatchNormalization()
Dropout(0.05)
#output shape:(4\*4*10)
#receptive field: 41
#  Layer 15
GlobalAveragePooling2D()
Activation('softmax')

#  Logs
Epoch 00001: LearningRateScheduler setting learning rate to 0.003.
390/390 [==============================] - 46s 119ms/step - loss: 1.4890 - acc: 0.4695 - val_loss: 1.9512 - val_acc: 0.4677
Epoch 2/50

Epoch 00002: LearningRateScheduler setting learning rate to 0.0022744503.
390/390 [==============================] - 30s 76ms/step - loss: 1.0232 - acc: 0.6475 - val_loss: 1.1181 - val_acc: 0.6362
Epoch 3/50

Epoch 00003: LearningRateScheduler setting learning rate to 0.0018315018.
390/390 [==============================] - 30s 76ms/step - loss: 0.8345 - acc: 0.7153 - val_loss: 0.8689 - val_acc: 0.7059
Epoch 4/50

Epoch 00004: LearningRateScheduler setting learning rate to 0.0015329586.
390/390 [==============================] - 30s 76ms/step - loss: 0.7229 - acc: 0.7541 - val_loss: 0.7697 - val_acc: 0.7428
Epoch 5/50

Epoch 00005: LearningRateScheduler setting learning rate to 0.0013181019.
390/390 [==============================] - 30s 76ms/step - loss: 0.6557 - acc: 0.7786 - val_loss: 0.6848 - val_acc: 0.7698
Epoch 6/50

Epoch 00006: LearningRateScheduler setting learning rate to 0.0011560694.
390/390 [==============================] - 30s 76ms/step - loss: 0.5994 - acc: 0.7987 - val_loss: 0.6422 - val_acc: 0.7808
Epoch 7/50

Epoch 00007: LearningRateScheduler setting learning rate to 0.0010295127.
390/390 [==============================] - 30s 76ms/step - loss: 0.5598 - acc: 0.8083 - val_loss: 0.6318 - val_acc: 0.7857
Epoch 8/50

Epoch 00008: LearningRateScheduler setting learning rate to 0.0009279307.
390/390 [==============================] - 30s 76ms/step - loss: 0.5232 - acc: 0.8226 - val_loss: 0.5963 - val_acc: 0.7994
Epoch 9/50

Epoch 00009: LearningRateScheduler setting learning rate to 0.0008445946.
390/390 [==============================] - 30s 76ms/step - loss: 0.4964 - acc: 0.8324 - val_loss: 0.6471 - val_acc: 0.7847
Epoch 10/50

Epoch 00010: LearningRateScheduler setting learning rate to 0.0007749935.
390/390 [==============================] - 30s 76ms/step - loss: 0.4691 - acc: 0.8416 - val_loss: 0.5732 - val_acc: 0.8069
Epoch 11/50

Epoch 00011: LearningRateScheduler setting learning rate to 0.0007159905.
390/390 [==============================] - 30s 76ms/step - loss: 0.4467 - acc: 0.8504 - val_loss: 0.5969 - val_acc: 0.8034
Epoch 12/50

Epoch 00012: LearningRateScheduler setting learning rate to 0.000665336.
390/390 [==============================] - 30s 76ms/step - loss: 0.4245 - acc: 0.8571 - val_loss: 0.5629 - val_acc: 0.8094
Epoch 13/50

Epoch 00013: LearningRateScheduler setting learning rate to 0.0006213753.
390/390 [==============================] - 30s 76ms/step - loss: 0.4085 - acc: 0.8609 - val_loss: 0.5501 - val_acc: 0.8180
Epoch 14/50

Epoch 00014: LearningRateScheduler setting learning rate to 0.0005828638.
390/390 [==============================] - 30s 76ms/step - loss: 0.3871 - acc: 0.8700 - val_loss: 0.5691 - val_acc: 0.8119
Epoch 15/50

Epoch 00015: LearningRateScheduler setting learning rate to 0.0005488474.
390/390 [==============================] - 30s 76ms/step - loss: 0.3718 - acc: 0.8763 - val_loss: 0.5416 - val_acc: 0.8232
Epoch 16/50

Epoch 00016: LearningRateScheduler setting learning rate to 0.0005185825.
390/390 [==============================] - 30s 76ms/step - loss: 0.3622 - acc: 0.8791 - val_loss: 0.5589 - val_acc: 0.8150
Epoch 17/50

Epoch 00017: LearningRateScheduler setting learning rate to 0.000491481.
390/390 [==============================] - 30s 76ms/step - loss: 0.3470 - acc: 0.8842 - val_loss: 0.5544 - val_acc: 0.8173
Epoch 18/50

Epoch 00018: LearningRateScheduler setting learning rate to 0.0004670715.
390/390 [==============================] - 30s 76ms/step - loss: 0.3364 - acc: 0.8878 - val_loss: 0.5592 - val_acc: 0.8194
Epoch 19/50

Epoch 00019: LearningRateScheduler setting learning rate to 0.0004449718.
390/390 [==============================] - 30s 76ms/step - loss: 0.3252 - acc: 0.8912 - val_loss: 0.5550 - val_acc: 0.8214
Epoch 20/50

Epoch 00020: LearningRateScheduler setting learning rate to 0.000424869.
390/390 [==============================] - 30s 76ms/step - loss: 0.3188 - acc: 0.8945 - val_loss: 0.5515 - val_acc: 0.8194
Epoch 21/50

Epoch 00021: LearningRateScheduler setting learning rate to 0.0004065041.
390/390 [==============================] - 30s 76ms/step - loss: 0.3089 - acc: 0.8959 - val_loss: 0.5517 - val_acc: 0.8219
Epoch 22/50

Epoch 00022: LearningRateScheduler setting learning rate to 0.000389661.
390/390 [==============================] - 30s 77ms/step - loss: 0.2979 - acc: 0.9013 - val_loss: 0.5559 - val_acc: 0.8242
Epoch 23/50

Epoch 00023: LearningRateScheduler setting learning rate to 0.0003741581.
390/390 [==============================] - 30s 76ms/step - loss: 0.2893 - acc: 0.9040 - val_loss: 0.5579 - val_acc: 0.8221
Epoch 24/50

Epoch 00024: LearningRateScheduler setting learning rate to 0.0003598417.
390/390 [==============================] - 30s 76ms/step - loss: 0.2847 - acc: 0.9054 - val_loss: 0.5540 - val_acc: 0.8232
Epoch 25/50

Epoch 00025: LearningRateScheduler setting learning rate to 0.0003465804.
390/390 [==============================] - 30s 76ms/step - loss: 0.2795 - acc: 0.9061 - val_loss: 0.5530 - val_acc: 0.8246
Epoch 26/50

Epoch 00026: LearningRateScheduler setting learning rate to 0.0003342618.
390/390 [==============================] - 30s 76ms/step - loss: 0.2700 - acc: 0.9099 - val_loss: 0.5590 - val_acc: 0.8240
Epoch 27/50

Epoch 00027: LearningRateScheduler setting learning rate to 0.0003227889.
390/390 [==============================] - 30s 76ms/step - loss: 0.2655 - acc: 0.9124 - val_loss: 0.5624 - val_acc: 0.8213
Epoch 28/50

Epoch 00028: LearningRateScheduler setting learning rate to 0.0003120774.
390/390 [==============================] - 30s 76ms/step - loss: 0.2651 - acc: 0.9118 - val_loss: 0.5579 - val_acc: 0.8244
Epoch 29/50

Epoch 00029: LearningRateScheduler setting learning rate to 0.000302054.
390/390 [==============================] - 30s 76ms/step - loss: 0.2616 - acc: 0.9119 - val_loss: 0.5741 - val_acc: 0.8203
Epoch 30/50

Epoch 00030: LearningRateScheduler setting learning rate to 0.0002926544.
390/390 [==============================] - 30s 76ms/step - loss: 0.2489 - acc: 0.9184 - val_loss: 0.5600 - val_acc: 0.8234
Epoch 31/50

Epoch 00031: LearningRateScheduler setting learning rate to 0.0002838221.
390/390 [==============================] - 30s 76ms/step - loss: 0.2490 - acc: 0.9165 - val_loss: 0.5669 - val_acc: 0.8232
Epoch 32/50

Epoch 00032: LearningRateScheduler setting learning rate to 0.0002755074.
390/390 [==============================] - 30s 76ms/step - loss: 0.2427 - acc: 0.9198 - val_loss: 0.5678 - val_acc: 0.8233
Epoch 33/50

Epoch 00033: LearningRateScheduler setting learning rate to 0.000267666.
390/390 [==============================] - 30s 76ms/step - loss: 0.2366 - acc: 0.9210 - val_loss: 0.5654 - val_acc: 0.8204
Epoch 34/50

Epoch 00034: LearningRateScheduler setting learning rate to 0.0002602585.
390/390 [==============================] - 30s 76ms/step - loss: 0.2322 - acc: 0.9238 - val_loss: 0.5661 - val_acc: 0.8254
Epoch 35/50

Epoch 00035: LearningRateScheduler setting learning rate to 0.00025325.
390/390 [==============================] - 30s 76ms/step - loss: 0.2335 - acc: 0.9231 - val_loss: 0.5680 - val_acc: 0.8237
Epoch 36/50

Epoch 00036: LearningRateScheduler setting learning rate to 0.0002466091.
390/390 [==============================] - 30s 76ms/step - loss: 0.2275 - acc: 0.9249 - val_loss: 0.5751 - val_acc: 0.8225
Epoch 37/50

Epoch 00037: LearningRateScheduler setting learning rate to 0.0002403076.
390/390 [==============================] - 30s 76ms/step - loss: 0.2254 - acc: 0.9258 - val_loss: 0.5724 - val_acc: 0.8260
Epoch 38/50

Epoch 00038: LearningRateScheduler setting learning rate to 0.0002343201.
390/390 [==============================] - 30s 76ms/step - loss: 0.2193 - acc: 0.9273 - val_loss: 0.5728 - val_acc: 0.8245
Epoch 39/50

Epoch 00039: LearningRateScheduler setting learning rate to 0.0002286237.
390/390 [==============================] - 30s 76ms/step - loss: 0.2161 - acc: 0.9293 - val_loss: 0.5669 - val_acc: 0.8261
Epoch 40/50

Epoch 00040: LearningRateScheduler setting learning rate to 0.0002231977.
390/390 [==============================] - 30s 76ms/step - loss: 0.2102 - acc: 0.9301 - val_loss: 0.5743 - val_acc: 0.8269
Epoch 41/50

Epoch 00041: LearningRateScheduler setting learning rate to 0.0002180233.
390/390 [==============================] - 30s 76ms/step - loss: 0.2115 - acc: 0.9303 - val_loss: 0.5745 - val_acc: 0.8241
Epoch 42/50

Epoch 00042: LearningRateScheduler setting learning rate to 0.0002130833.
390/390 [==============================] - 30s 76ms/step - loss: 0.2115 - acc: 0.9303 - val_loss: 0.5751 - val_acc: 0.8277
Epoch 43/50

Epoch 00043: LearningRateScheduler setting learning rate to 0.0002083623.
390/390 [==============================] - 30s 76ms/step - loss: 0.2052 - acc: 0.9324 - val_loss: 0.5830 - val_acc: 0.8267
Epoch 44/50

Epoch 00044: LearningRateScheduler setting learning rate to 0.0002038459.
390/390 [==============================] - 30s 76ms/step - loss: 0.2026 - acc: 0.9327 - val_loss: 0.5756 - val_acc: 0.8302
Epoch 45/50

Epoch 00045: LearningRateScheduler setting learning rate to 0.0001995211.
390/390 [==============================] - 30s 76ms/step - loss: 0.2022 - acc: 0.9326 - val_loss: 0.5725 - val_acc: 0.8277
Epoch 46/50

Epoch 00046: LearningRateScheduler setting learning rate to 0.0001953761.
390/390 [==============================] - 30s 76ms/step - loss: 0.1935 - acc: 0.9359 - val_loss: 0.5815 - val_acc: 0.8290
Epoch 47/50

Epoch 00047: LearningRateScheduler setting learning rate to 0.0001913998.
390/390 [==============================] - 29s 76ms/step - loss: 0.1961 - acc: 0.9350 - val_loss: 0.5776 - val_acc: 0.8292
Epoch 48/50

Epoch 00048: LearningRateScheduler setting learning rate to 0.0001875821.
390/390 [==============================] - 30s 76ms/step - loss: 0.1912 - acc: 0.9369 - val_loss: 0.5765 - val_acc: 0.8283
Epoch 49/50

Epoch 00049: LearningRateScheduler setting learning rate to 0.0001839137.
390/390 [==============================] - 30s 76ms/step - loss: 0.1912 - acc: 0.9363 - val_loss: 0.5814 - val_acc: 0.8299
Epoch 50/50

Epoch 00050: LearningRateScheduler setting learning rate to 0.000180386.
390/390 [==============================] - 30s 76ms/step - loss: 0.1911 - acc: 0.9359 - val_loss: 0.5820 - val_acc: 0.8297
Model took 1500.74 seconds to train
