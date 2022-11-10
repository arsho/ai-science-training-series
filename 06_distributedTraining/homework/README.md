# Scaling MNIST example
Please put your homework in this folder. This includes
1. tensorflow2_mnist_hvd.py code
2. accuracy plots for 1, 2, 4, 8, 16 GPU runs. 

And provide the link to your ./homework folder. 

## Run results

```
(2022-07-01//base) arsho@thetagpu14:~/ai-science-training-series/06_distributedTraining/homework$ mpirun -n 1 python tensorflow2_mnist_hvd.py
# I am rank 0 of 1
2022-11-09 20:04:31.949841: W tensorflow/core/common_runtime/gpu/gpu_bfc_allocator.cc:42] Overriding orig_value setting because the TF_FORCE_GPU_ALLOW_GROWTH environment variable is set. Original config value was 0.
Epoch - 0, step #000000/000234	Loss: 2.302877
Epoch - 0, step #000100/000234	Loss: 0.166046
Epoch - 0, step #000200/000234	Loss: 0.173881
E[0], train Loss: 0.405412, training Acc: 0.876, val loss: 0.079, val Acc: 0.973	 Time: 12.247 seconds
Epoch - 1, step #000000/000234	Loss: 0.230077
Epoch - 1, step #000100/000234	Loss: 0.271981
Epoch - 1, step #000200/000234	Loss: 0.078985
E[1], train Loss: 0.153748, training Acc: 0.954, val loss: 0.058, val Acc: 0.981	 Time: 1.548 seconds
Epoch - 2, step #000000/000234	Loss: 0.164889
Epoch - 2, step #000100/000234	Loss: 0.115753
Epoch - 2, step #000200/000234	Loss: 0.097287
E[2], train Loss: 0.130289, training Acc: 0.960, val loss: 0.050, val Acc: 0.984	 Time: 1.546 seconds
Epoch - 3, step #000000/000234	Loss: 0.200317
Epoch - 3, step #000100/000234	Loss: 0.133525
Epoch - 3, step #000200/000234	Loss: 0.091892
E[3], train Loss: 0.117627, training Acc: 0.963, val loss: 0.050, val Acc: 0.984	 Time: 1.542 seconds
Epoch - 4, step #000000/000234	Loss: 0.082438
Epoch - 4, step #000100/000234	Loss: 0.106313
Epoch - 4, step #000200/000234	Loss: 0.111218
E[4], train Loss: 0.107683, training Acc: 0.967, val loss: 0.050, val Acc: 0.983	 Time: 1.544 seconds
Epoch - 5, step #000000/000234	Loss: 0.169532
Epoch - 5, step #000100/000234	Loss: 0.124373
Epoch - 5, step #000200/000234	Loss: 0.091744
E[5], train Loss: 0.110689, training Acc: 0.966, val loss: 0.044, val Acc: 0.986	 Time: 1.540 seconds
Epoch - 6, step #000000/000234	Loss: 0.111177
Epoch - 6, step #000100/000234	Loss: 0.102808
Epoch - 6, step #000200/000234	Loss: 0.098121
E[6], train Loss: 0.103094, training Acc: 0.969, val loss: 0.039, val Acc: 0.987	 Time: 1.542 seconds
Epoch - 7, step #000000/000234	Loss: 0.053500
Epoch - 7, step #000100/000234	Loss: 0.116341
Epoch - 7, step #000200/000234	Loss: 0.048698
E[7], train Loss: 0.094707, training Acc: 0.972, val loss: 0.040, val Acc: 0.987	 Time: 1.545 seconds
Epoch - 8, step #000000/000234	Loss: 0.136195
Epoch - 8, step #000100/000234	Loss: 0.035165
Epoch - 8, step #000200/000234	Loss: 0.118073
E[8], train Loss: 0.097818, training Acc: 0.971, val loss: 0.047, val Acc: 0.984	 Time: 1.547 seconds
Epoch - 9, step #000000/000234	Loss: 0.112084
Epoch - 9, step #000100/000234	Loss: 0.072766
Epoch - 9, step #000200/000234	Loss: 0.040518
E[9], train Loss: 0.090272, training Acc: 0.973, val loss: 0.040, val Acc: 0.987	 Time: 1.545 seconds
Epoch - 10, step #000000/000234	Loss: 0.032429
Epoch - 10, step #000100/000234	Loss: 0.087034
Epoch - 10, step #000200/000234	Loss: 0.062432
E[10], train Loss: 0.091393, training Acc: 0.972, val loss: 0.043, val Acc: 0.986	 Time: 1.543 seconds
Epoch - 11, step #000000/000234	Loss: 0.093520
Epoch - 11, step #000100/000234	Loss: 0.084565
Epoch - 11, step #000200/000234	Loss: 0.103846
E[11], train Loss: 0.086825, training Acc: 0.974, val loss: 0.039, val Acc: 0.987	 Time: 1.546 seconds
Epoch - 12, step #000000/000234	Loss: 0.036966
Epoch - 12, step #000100/000234	Loss: 0.034830
Epoch - 12, step #000200/000234	Loss: 0.158249
E[12], train Loss: 0.086619, training Acc: 0.974, val loss: 0.036, val Acc: 0.988	 Time: 1.564 seconds
Epoch - 13, step #000000/000234	Loss: 0.035483
Epoch - 13, step #000100/000234	Loss: 0.064752
Epoch - 13, step #000200/000234	Loss: 0.071975
E[13], train Loss: 0.082917, training Acc: 0.975, val loss: 0.040, val Acc: 0.989	 Time: 1.545 seconds
Epoch - 14, step #000000/000234	Loss: 0.036867
Epoch - 14, step #000100/000234	Loss: 0.089628
Epoch - 14, step #000200/000234	Loss: 0.060843
E[14], train Loss: 0.084350, training Acc: 0.975, val loss: 0.045, val Acc: 0.986	 Time: 1.570 seconds
Epoch - 15, step #000000/000234	Loss: 0.077879
Epoch - 15, step #000100/000234	Loss: 0.042069
Epoch - 15, step #000200/000234	Loss: 0.091471
E[15], train Loss: 0.083867, training Acc: 0.974, val loss: 0.043, val Acc: 0.987	 Time: 1.545 seconds
Total training time: 35.50042009353638 seconds
(2022-07-01//base) arsho@thetagpu14:~/ai-science-training-series/06_distributedTraining/homework$ mpirun -n 2 python tensorflow2_mnist_hvd.py
# I am rank 0 of 2
# I am rank 1 of 2
2022-11-09 20:06:12.258050: W tensorflow/core/common_runtime/gpu/gpu_bfc_allocator.cc:42] Overriding orig_value setting because the TF_FORCE_GPU_ALLOW_GROWTH environment variable is set. Original config value was 0.
2022-11-09 20:06:12.267983: W tensorflow/core/common_runtime/gpu/gpu_bfc_allocator.cc:42] Overriding orig_value setting because the TF_FORCE_GPU_ALLOW_GROWTH environment variable is set. Original config value was 0.
Epoch - 0, step #000000/000234	Loss: 2.308513
Epoch - 0, step #000100/000234	Loss: 0.413791
Epoch - 0, step #000200/000234	Loss: 0.305479
E[0], train Loss: 0.541393, training Acc: 0.831, val loss: 0.123, val Acc: 0.962	 Time: 9.908 seconds
E[0], train Loss: 0.541393, training Acc: 0.831, val loss: 0.106, val Acc: 0.966	 Time: 11.181 seconds
Epoch - 1, step #000000/000234	Loss: 0.296083
Epoch - 1, step #000100/000234	Loss: 0.179279
Epoch - 1, step #000200/000234	Loss: 0.284857
E[1], train Loss: 0.229032, training Acc: 0.931, val loss: 0.090, val Acc: 0.972	 Time: 2.548 seconds
E[1], train Loss: 0.229032, training Acc: 0.931, val loss: 0.082, val Acc: 0.974	 Time: 2.856 seconds
Epoch - 2, step #000000/000234	Loss: 0.158269
Epoch - 2, step #000100/000234	Loss: 0.219943
Epoch - 2, step #000200/000234	Loss: 0.131691
E[2], train Loss: 0.194177, training Acc: 0.941, val loss: 0.087, val Acc: 0.976	 Time: 3.161 seconds
E[2], train Loss: 0.194177, training Acc: 0.941, val loss: 0.083, val Acc: 0.975	 Time: 2.866 seconds
Epoch - 3, step #000000/000234	Loss: 0.232357
Epoch - 3, step #000100/000234	Loss: 0.153233
Epoch - 3, step #000200/000234	Loss: 0.171931
E[3], train Loss: 0.179529, training Acc: 0.946, val loss: 0.081, val Acc: 0.974	 Time: 2.736 seconds
E[3], train Loss: 0.179529, training Acc: 0.946, val loss: 0.071, val Acc: 0.977	 Time: 2.797 seconds
Epoch - 4, step #000000/000234	Loss: 0.210555
Epoch - 4, step #000100/000234	Loss: 0.257789
Epoch - 4, step #000200/000234	Loss: 0.173695
E[4], train Loss: 0.171052, training Acc: 0.949, val loss: 0.069, val Acc: 0.979	 Time: 2.669 seconds
E[4], train Loss: 0.171052, training Acc: 0.949, val loss: 0.078, val Acc: 0.977	 Time: 2.847 seconds
Epoch - 5, step #000000/000234	Loss: 0.180791
Epoch - 5, step #000100/000234	Loss: 0.164776
Epoch - 5, step #000200/000234	Loss: 0.092862
E[5], train Loss: 0.165048, training Acc: 0.951, val loss: 0.063, val Acc: 0.981	 Time: 2.889 seconds
E[5], train Loss: 0.165048, training Acc: 0.951, val loss: 0.064, val Acc: 0.980	 Time: 2.868 seconds
Epoch - 6, step #000000/000234	Loss: 0.175289
Epoch - 6, step #000100/000234	Loss: 0.201719
Epoch - 6, step #000200/000234	Loss: 0.171621
E[6], train Loss: 0.162305, training Acc: 0.951, val loss: 0.065, val Acc: 0.979	 Time: 2.892 seconds
E[6], train Loss: 0.162305, training Acc: 0.951, val loss: 0.061, val Acc: 0.981	 Time: 2.857 seconds
Epoch - 7, step #000000/000234	Loss: 0.260601
Epoch - 7, step #000100/000234	Loss: 0.136394
Epoch - 7, step #000200/000234	Loss: 0.139470
E[7], train Loss: 0.152472, training Acc: 0.955, val loss: 0.068, val Acc: 0.979	 Time: 2.886 seconds
E[7], train Loss: 0.152472, training Acc: 0.955, val loss: 0.067, val Acc: 0.980	 Time: 2.849 seconds
Epoch - 8, step #000000/000234	Loss: 0.181262
Epoch - 8, step #000100/000234	Loss: 0.175559
Epoch - 8, step #000200/000234	Loss: 0.199647
E[8], train Loss: 0.160817, training Acc: 0.952, val loss: 0.068, val Acc: 0.978	 Time: 2.802 seconds
E[8], train Loss: 0.160817, training Acc: 0.952, val loss: 0.069, val Acc: 0.978	 Time: 2.924 seconds
Epoch - 9, step #000000/000234	Loss: 0.165758
Epoch - 9, step #000100/000234	Loss: 0.158756
Epoch - 9, step #000200/000234	Loss: 0.099672
E[9], train Loss: 0.155901, training Acc: 0.954, val loss: 0.064, val Acc: 0.981	 Time: 2.945 seconds
E[9], train Loss: 0.155901, training Acc: 0.954, val loss: 0.062, val Acc: 0.982	 Time: 2.918 seconds
Epoch - 10, step #000000/000234	Loss: 0.129490
Epoch - 10, step #000100/000234	Loss: 0.161221
Epoch - 10, step #000200/000234	Loss: 0.161047
E[10], train Loss: 0.156960, training Acc: 0.952, val loss: 0.072, val Acc: 0.979	 Time: 3.001 seconds
E[10], train Loss: 0.156960, training Acc: 0.952, val loss: 0.068, val Acc: 0.980	 Time: 2.604 seconds
Epoch - 11, step #000000/000234	Loss: 0.140278
Epoch - 11, step #000100/000234	Loss: 0.165399
Epoch - 11, step #000200/000234	Loss: 0.187561
E[11], train Loss: 0.160686, training Acc: 0.952, val loss: 0.070, val Acc: 0.980	 Time: 2.577 seconds
E[11], train Loss: 0.160686, training Acc: 0.952, val loss: 0.064, val Acc: 0.981	 Time: 2.897 seconds
Epoch - 12, step #000000/000234	Loss: 0.116094
Epoch - 12, step #000100/000234	Loss: 0.197019
Epoch - 12, step #000200/000234	Loss: 0.164818
E[12], train Loss: 0.152378, training Acc: 0.954, val loss: 0.068, val Acc: 0.979	 Time: 2.773 seconds
E[12], train Loss: 0.152378, training Acc: 0.954, val loss: 0.071, val Acc: 0.979	 Time: 2.823 seconds
Epoch - 13, step #000000/000234	Loss: 0.145353
Epoch - 13, step #000100/000234	Loss: 0.131716
Epoch - 13, step #000200/000234	Loss: 0.176487
E[13], train Loss: 0.149035, training Acc: 0.955, val loss: 0.062, val Acc: 0.981	 Time: 2.886 seconds
E[13], train Loss: 0.149035, training Acc: 0.955, val loss: 0.064, val Acc: 0.982	 Time: 2.859 seconds
Epoch - 14, step #000000/000234	Loss: 0.167711
Epoch - 14, step #000100/000234	Loss: 0.124033
Epoch - 14, step #000200/000234	Loss: 0.167812
E[14], train Loss: 0.145224, training Acc: 0.956, val loss: 0.061, val Acc: 0.981	 Time: 2.858 seconds
E[14], train Loss: 0.145224, training Acc: 0.956, val loss: 0.059, val Acc: 0.980	 Time: 2.487 seconds
Epoch - 15, step #000000/000234	Loss: 0.131264
Epoch - 15, step #000100/000234	Loss: 0.149700
Epoch - 15, step #000200/000234	Loss: 0.105294
E[15], train Loss: 0.153216, training Acc: 0.954, val loss: 0.066, val Acc: 0.980	 Time: 2.453 seconds
Total training time: 51.9938428401947 seconds
E[15], train Loss: 0.153216, training Acc: 0.954, val loss: 0.058, val Acc: 0.982	 Time: 2.820 seconds
Total training time: 53.50179934501648 seconds
(2022-07-01//base) arsho@thetagpu14:~/ai-science-training-series/06_distributedTraining/homework$ mpirun -n 4 python tensorflow2_mnist_hvd.py
# I am rank 3 of 4
# I am rank 1 of 4
# I am rank 2 of 4
# I am rank 0 of 4
2022-11-09 20:07:39.700156: W tensorflow/core/common_runtime/gpu/gpu_bfc_allocator.cc:42] Overriding orig_value setting because the TF_FORCE_GPU_ALLOW_GROWTH environment variable is set. Original config value was 0.
2022-11-09 20:07:39.714507: W tensorflow/core/common_runtime/gpu/gpu_bfc_allocator.cc:42] Overriding orig_value setting because the TF_FORCE_GPU_ALLOW_GROWTH environment variable is set. Original config value was 0.
2022-11-09 20:07:39.723580: W tensorflow/core/common_runtime/gpu/gpu_bfc_allocator.cc:42] Overriding orig_value setting because the TF_FORCE_GPU_ALLOW_GROWTH environment variable is set. Original config value was 0.
2022-11-09 20:07:39.742075: W tensorflow/core/common_runtime/gpu/gpu_bfc_allocator.cc:42] Overriding orig_value setting because the TF_FORCE_GPU_ALLOW_GROWTH environment variable is set. Original config value was 0.
Epoch - 0, step #000000/000234	Loss: 2.305609
Epoch - 0, step #000100/000234	Loss: 2.301514
Epoch - 0, step #000200/000234	Loss: 2.306116
E[0], train Loss: 2.393079, training Acc: 0.111, val loss: 2.302, val Acc: 0.101	 Time: 12.141 seconds
E[0], train Loss: 2.393079, training Acc: 0.111, val loss: 2.302, val Acc: 0.101	 Time: 12.192 seconds
E[0], train Loss: 2.393079, training Acc: 0.111, val loss: 2.302, val Acc: 0.101	 Time: 12.102 seconds
E[0], train Loss: 2.393079, training Acc: 0.111, val loss: 2.302, val Acc: 0.101	 Time: 12.079 seconds
Epoch - 1, step #000000/000234	Loss: 2.304775
Epoch - 1, step #000100/000234	Loss: 2.302737
Epoch - 1, step #000200/000234	Loss: 2.301514
E[1], train Loss: 2.301901, training Acc: 0.111, val loss: 2.301, val Acc: 0.113	 Time: 1.727 seconds
E[1], train Loss: 2.301901, training Acc: 0.111, val loss: 2.301, val Acc: 0.113	 Time: 1.733 seconds
E[1], train Loss: 2.301901, training Acc: 0.111, val loss: 2.301, val Acc: 0.113	 Time: 1.731 seconds
E[1], train Loss: 2.301901, training Acc: 0.111, val loss: 2.301, val Acc: 0.113	 Time: 1.733 seconds
Epoch - 2, step #000000/000234	Loss: 2.302719
Epoch - 2, step #000100/000234	Loss: 2.298100
Epoch - 2, step #000200/000234	Loss: 2.302197
E[2], train Loss: 2.301711, training Acc: 0.113, val loss: 2.303, val Acc: 0.113	 Time: 2.110 seconds
E[2], train Loss: 2.301711, training Acc: 0.113, val loss: 2.303, val Acc: 0.113	 Time: 2.107 seconds
E[2], train Loss: 2.301711, training Acc: 0.113, val loss: 2.303, val Acc: 0.113	 Time: 2.111 seconds
E[2], train Loss: 2.301711, training Acc: 0.113, val loss: 2.303, val Acc: 0.113	 Time: 2.118 seconds
Epoch - 3, step #000000/000234	Loss: 2.303790
Epoch - 3, step #000100/000234	Loss: 2.301724
Epoch - 3, step #000200/000234	Loss: 2.301646
E[3], train Loss: 2.301848, training Acc: 0.112, val loss: 2.303, val Acc: 0.113	 Time: 2.019 seconds
E[3], train Loss: 2.301848, training Acc: 0.112, val loss: 2.303, val Acc: 0.113	 Time: 2.016 seconds
E[3], train Loss: 2.301848, training Acc: 0.112, val loss: 2.303, val Acc: 0.113	 Time: 2.018 seconds
E[3], train Loss: 2.301848, training Acc: 0.112, val loss: 2.303, val Acc: 0.113	 Time: 2.024 seconds
Epoch - 4, step #000000/000234	Loss: 2.301404
Epoch - 4, step #000100/000234	Loss: 2.302459
Epoch - 4, step #000200/000234	Loss: 2.305940
E[4], train Loss: 2.301787, training Acc: 0.112, val loss: 2.301, val Acc: 0.113	 Time: 1.823 seconds
E[4], train Loss: 2.301787, training Acc: 0.112, val loss: 2.301, val Acc: 0.113	 Time: 1.827 seconds
E[4], train Loss: 2.301787, training Acc: 0.112, val loss: 2.301, val Acc: 0.113	 Time: 1.829 seconds
E[4], train Loss: 2.301787, training Acc: 0.112, val loss: 2.301, val Acc: 0.113	 Time: 1.827 seconds
Epoch - 5, step #000000/000234	Loss: 2.299600
Epoch - 5, step #000100/000234	Loss: 2.297811
Epoch - 5, step #000200/000234	Loss: 2.305851
E[5], train Loss: 2.301817, training Acc: 0.111, val loss: 2.302, val Acc: 0.103	 Time: 1.787 seconds
E[5], train Loss: 2.301817, training Acc: 0.111, val loss: 2.302, val Acc: 0.103	 Time: 1.789 seconds
E[5], train Loss: 2.301817, training Acc: 0.111, val loss: 2.302, val Acc: 0.103	 Time: 1.788 seconds
E[5], train Loss: 2.301817, training Acc: 0.111, val loss: 2.302, val Acc: 0.103	 Time: 1.797 seconds
Epoch - 6, step #000000/000234	Loss: 2.304062
Epoch - 6, step #000100/000234	Loss: 2.303291
Epoch - 6, step #000200/000234	Loss: 2.298653
E[6], train Loss: 2.301882, training Acc: 0.111, val loss: 2.302, val Acc: 0.113	 Time: 2.085 seconds
E[6], train Loss: 2.301882, training Acc: 0.111, val loss: 2.302, val Acc: 0.113	 Time: 2.088 seconds
E[6], train Loss: 2.301882, training Acc: 0.111, val loss: 2.302, val Acc: 0.113	 Time: 2.090 seconds
E[6], train Loss: 2.301882, training Acc: 0.111, val loss: 2.302, val Acc: 0.113	 Time: 2.085 seconds
Epoch - 7, step #000000/000234	Loss: 2.300997
Epoch - 7, step #000100/000234	Loss: 2.298686
Epoch - 7, step #000200/000234	Loss: 2.301125
E[7], train Loss: 2.301859, training Acc: 0.111, val loss: 2.302, val Acc: 0.113	 Time: 1.912 seconds
E[7], train Loss: 2.301859, training Acc: 0.111, val loss: 2.302, val Acc: 0.113	 Time: 1.914 seconds
E[7], train Loss: 2.301859, training Acc: 0.111, val loss: 2.302, val Acc: 0.113	 Time: 1.913 seconds
E[7], train Loss: 2.301859, training Acc: 0.111, val loss: 2.302, val Acc: 0.113	 Time: 1.914 seconds
Epoch - 8, step #000000/000234	Loss: 2.301054
Epoch - 8, step #000100/000234	Loss: 2.306045
Epoch - 8, step #000200/000234	Loss: 2.303510
E[8], train Loss: 2.301828, training Acc: 0.112, val loss: 2.302, val Acc: 0.113	 Time: 1.781 seconds
E[8], train Loss: 2.301828, training Acc: 0.112, val loss: 2.302, val Acc: 0.113	 Time: 1.788 seconds
E[8], train Loss: 2.301828, training Acc: 0.112, val loss: 2.302, val Acc: 0.113	 Time: 1.787 seconds
E[8], train Loss: 2.301828, training Acc: 0.112, val loss: 2.302, val Acc: 0.113	 Time: 1.789 seconds
Epoch - 9, step #000000/000234	Loss: 2.303279
Epoch - 9, step #000100/000234	Loss: 2.300484
Epoch - 9, step #000200/000234	Loss: 2.299609
E[9], train Loss: 2.301845, training Acc: 0.112, val loss: 2.303, val Acc: 0.103	 Time: 1.995 seconds
E[9], train Loss: 2.301845, training Acc: 0.112, val loss: 2.303, val Acc: 0.103	 Time: 2.000 seconds
E[9], train Loss: 2.301845, training Acc: 0.112, val loss: 2.303, val Acc: 0.103	 Time: 1.999 seconds
E[9], train Loss: 2.301845, training Acc: 0.112, val loss: 2.303, val Acc: 0.103	 Time: 2.000 seconds
Epoch - 10, step #000000/000234	Loss: 2.301897
Epoch - 10, step #000100/000234	Loss: 2.303309
Epoch - 10, step #000200/000234	Loss: 2.300501
E[10], train Loss: 2.302048, training Acc: 0.110, val loss: 2.303, val Acc: 0.101	 Time: 1.947 seconds
E[10], train Loss: 2.302048, training Acc: 0.110, val loss: 2.303, val Acc: 0.101	 Time: 1.948 seconds
E[10], train Loss: 2.302048, training Acc: 0.110, val loss: 2.303, val Acc: 0.101	 Time: 1.951 seconds
E[10], train Loss: 2.302048, training Acc: 0.110, val loss: 2.303, val Acc: 0.101	 Time: 1.948 seconds
Epoch - 11, step #000000/000234	Loss: 2.300954
Epoch - 11, step #000100/000234	Loss: 2.301264
Epoch - 11, step #000200/000234	Loss: 2.300340
E[11], train Loss: 2.301851, training Acc: 0.111, val loss: 2.303, val Acc: 0.113	 Time: 1.786 seconds
E[11], train Loss: 2.301851, training Acc: 0.111, val loss: 2.303, val Acc: 0.113	 Time: 1.792 seconds
E[11], train Loss: 2.301851, training Acc: 0.111, val loss: 2.303, val Acc: 0.113	 Time: 1.790 seconds
E[11], train Loss: 2.301851, training Acc: 0.111, val loss: 2.303, val Acc: 0.113	 Time: 1.797 seconds
Epoch - 12, step #000000/000234	Loss: 2.300502
Epoch - 12, step #000100/000234	Loss: 2.298581
Epoch - 12, step #000200/000234	Loss: 2.305641
E[12], train Loss: 2.301961, training Acc: 0.111, val loss: 2.302, val Acc: 0.113	 Time: 1.949 seconds
E[12], train Loss: 2.301961, training Acc: 0.111, val loss: 2.302, val Acc: 0.113	 Time: 1.948 seconds
E[12], train Loss: 2.301961, training Acc: 0.111, val loss: 2.302, val Acc: 0.113	 Time: 1.949 seconds
E[12], train Loss: 2.301961, training Acc: 0.111, val loss: 2.302, val Acc: 0.113	 Time: 1.944 seconds
Epoch - 13, step #000000/000234	Loss: 2.301675
Epoch - 13, step #000100/000234	Loss: 2.298824
Epoch - 13, step #000200/000234	Loss: 2.301489
E[13], train Loss: 2.302166, training Acc: 0.110, val loss: 2.301, val Acc: 0.113	 Time: 1.806 seconds
E[13], train Loss: 2.302166, training Acc: 0.110, val loss: 2.301, val Acc: 0.113	 Time: 1.808 seconds
E[13], train Loss: 2.302166, training Acc: 0.110, val loss: 2.301, val Acc: 0.113	 Time: 1.806 seconds
E[13], train Loss: 2.302166, training Acc: 0.110, val loss: 2.301, val Acc: 0.113	 Time: 1.812 seconds
Epoch - 14, step #000000/000234	Loss: 2.304490
Epoch - 14, step #000100/000234	Loss: 2.306334
Epoch - 14, step #000200/000234	Loss: 2.299392
E[14], train Loss: 2.301981, training Acc: 0.111, val loss: 2.302, val Acc: 0.113	 Time: 1.887 seconds
E[14], train Loss: 2.301981, training Acc: 0.111, val loss: 2.302, val Acc: 0.113	 Time: 1.893 seconds
E[14], train Loss: 2.301981, training Acc: 0.111, val loss: 2.302, val Acc: 0.113	 Time: 1.894 seconds
E[14], train Loss: 2.301981, training Acc: 0.111, val loss: 2.302, val Acc: 0.113	 Time: 1.898 seconds
Epoch - 15, step #000000/000234	Loss: 2.300350
Epoch - 15, step #000100/000234	Loss: 2.296149
Epoch - 15, step #000200/000234	Loss: 2.304871
E[15], train Loss: 2.301762, training Acc: 0.112, val loss: 2.302, val Acc: 0.113	 Time: 2.213 seconds
E[15], train Loss: 2.301762, training Acc: 0.112, val loss: 2.302, val Acc: 0.113	 Time: 2.217 seconds
E[15], train Loss: 2.301762, training Acc: 0.112, val loss: 2.302, val Acc: 0.113	 Time: 2.217 seconds
Total training time: 41.065815448760986 seconds
Total training time: 40.951860189437866 seconds
E[15], train Loss: 2.301762, training Acc: 0.112, val loss: 2.302, val Acc: 0.113	 Time: 2.224 seconds
Total training time: 41.02560639381409 seconds
Total training time: 41.00516223907471 seconds
(2022-07-01//base) arsho@thetagpu14:~/ai-science-training-series/06_distributedTraining/homework$ mpirun -n 8 python tensorflow2_mnist_hvd.py
# I am rank 1 of 8
# I am rank 6 of 8
# I am rank 7 of 8
# I am rank 0 of 8
# I am rank 2 of 8
# I am rank 3 of 8
# I am rank 4 of 8
# I am rank 5 of 8
2022-11-09 20:08:51.331459: W tensorflow/core/common_runtime/gpu/gpu_bfc_allocator.cc:42] Overriding orig_value setting because the TF_FORCE_GPU_ALLOW_GROWTH environment variable is set. Original config value was 0.
2022-11-09 20:08:51.349660: W tensorflow/core/common_runtime/gpu/gpu_bfc_allocator.cc:42] Overriding orig_value setting because the TF_FORCE_GPU_ALLOW_GROWTH environment variable is set. Original config value was 0.
2022-11-09 20:08:51.358530: W tensorflow/core/common_runtime/gpu/gpu_bfc_allocator.cc:42] Overriding orig_value setting because the TF_FORCE_GPU_ALLOW_GROWTH environment variable is set. Original config value was 0.
2022-11-09 20:08:51.361906: W tensorflow/core/common_runtime/gpu/gpu_bfc_allocator.cc:42] Overriding orig_value setting because the TF_FORCE_GPU_ALLOW_GROWTH environment variable is set. Original config value was 0.
2022-11-09 20:08:51.370014: W tensorflow/core/common_runtime/gpu/gpu_bfc_allocator.cc:42] Overriding orig_value setting because the TF_FORCE_GPU_ALLOW_GROWTH environment variable is set. Original config value was 0.
2022-11-09 20:08:51.375361: W tensorflow/core/common_runtime/gpu/gpu_bfc_allocator.cc:42] Overriding orig_value setting because the TF_FORCE_GPU_ALLOW_GROWTH environment variable is set. Original config value was 0.
2022-11-09 20:08:51.378155: W tensorflow/core/common_runtime/gpu/gpu_bfc_allocator.cc:42] Overriding orig_value setting because the TF_FORCE_GPU_ALLOW_GROWTH environment variable is set. Original config value was 0.
2022-11-09 20:08:51.380197: W tensorflow/core/common_runtime/gpu/gpu_bfc_allocator.cc:42] Overriding orig_value setting because the TF_FORCE_GPU_ALLOW_GROWTH environment variable is set. Original config value was 0.
Epoch - 0, step #000000/000234	Loss: 2.306998
Epoch - 0, step #000100/000234	Loss: 2.301041
Epoch - 0, step #000200/000234	Loss: 2.301433
E[0], train Loss: 2.651521, training Acc: 0.111, val loss: 2.302, val Acc: 0.113	 Time: 18.394 seconds
E[0], train Loss: 2.651521, training Acc: 0.111, val loss: 2.302, val Acc: 0.113	 Time: 18.302 seconds
E[0], train Loss: 2.651521, training Acc: 0.111, val loss: 2.302, val Acc: 0.113	 Time: 18.351 seconds
E[0], train Loss: 2.651521, training Acc: 0.111, val loss: 2.302, val Acc: 0.113	 Time: 18.418 seconds
E[0], train Loss: 2.651521, training Acc: 0.111, val loss: 2.302, val Acc: 0.113	 Time: 18.377 seconds
E[0], train Loss: 2.651521, training Acc: 0.111, val loss: 2.302, val Acc: 0.113	 Time: 18.319 seconds
E[0], train Loss: 2.651521, training Acc: 0.111, val loss: 2.302, val Acc: 0.113	 Time: 18.368 seconds
E[0], train Loss: 2.651521, training Acc: 0.111, val loss: 2.302, val Acc: 0.113	 Time: 18.361 seconds
Epoch - 1, step #000000/000234	Loss: 2.300161
Epoch - 1, step #000100/000234	Loss: 2.303894
Epoch - 1, step #000200/000234	Loss: 2.301862
E[1], train Loss: 2.302070, training Acc: 0.111, val loss: 2.301, val Acc: 0.113	 Time: 2.071 seconds
E[1], train Loss: 2.302070, training Acc: 0.111, val loss: 2.301, val Acc: 0.113	 Time: 2.063 seconds
E[1], train Loss: 2.302070, training Acc: 0.111, val loss: 2.301, val Acc: 0.113	 Time: 2.073 seconds
E[1], train Loss: 2.302070, training Acc: 0.111, val loss: 2.301, val Acc: 0.113	 Time: 2.060 seconds
E[1], train Loss: 2.302070, training Acc: 0.111, val loss: 2.301, val Acc: 0.113	 Time: 2.054 seconds
E[1], train Loss: 2.302070, training Acc: 0.111, val loss: 2.301, val Acc: 0.113	 Time: 2.053 seconds
E[1], train Loss: 2.302070, training Acc: 0.111, val loss: 2.301, val Acc: 0.113	 Time: 2.058 seconds
E[1], train Loss: 2.302070, training Acc: 0.111, val loss: 2.301, val Acc: 0.113	 Time: 2.060 seconds
Epoch - 2, step #000000/000234	Loss: 2.302085
Epoch - 2, step #000100/000234	Loss: 2.295670
Epoch - 2, step #000200/000234	Loss: 2.302107
E[2], train Loss: 2.301935, training Acc: 0.111, val loss: 2.302, val Acc: 0.113	 Time: 1.931 seconds
E[2], train Loss: 2.301935, training Acc: 0.111, val loss: 2.302, val Acc: 0.113	 Time: 1.931 seconds
E[2], train Loss: 2.301935, training Acc: 0.111, val loss: 2.302, val Acc: 0.113	 Time: 1.933 seconds
E[2], train Loss: 2.301935, training Acc: 0.111, val loss: 2.302, val Acc: 0.113	 Time: 1.930 seconds
E[2], train Loss: 2.301935, training Acc: 0.111, val loss: 2.302, val Acc: 0.113	 Time: 1.934 seconds
E[2], train Loss: 2.301935, training Acc: 0.111, val loss: 2.302, val Acc: 0.113	 Time: 1.932 seconds
E[2], train Loss: 2.301935, training Acc: 0.111, val loss: 2.302, val Acc: 0.113	 Time: 1.940 seconds
E[2], train Loss: 2.301935, training Acc: 0.111, val loss: 2.302, val Acc: 0.113	 Time: 1.932 seconds
Epoch - 3, step #000000/000234	Loss: 2.302150
Epoch - 3, step #000100/000234	Loss: 2.299687
Epoch - 3, step #000200/000234	Loss: 2.300640
E[3], train Loss: 2.301989, training Acc: 0.111, val loss: 2.302, val Acc: 0.113	 Time: 1.929 seconds
E[3], train Loss: 2.301989, training Acc: 0.111, val loss: 2.302, val Acc: 0.113	 Time: 1.930 seconds
E[3], train Loss: 2.301989, training Acc: 0.111, val loss: 2.302, val Acc: 0.113	 Time: 1.926 seconds
E[3], train Loss: 2.301989, training Acc: 0.111, val loss: 2.302, val Acc: 0.113	 Time: 1.925 seconds
E[3], train Loss: 2.301989, training Acc: 0.111, val loss: 2.302, val Acc: 0.113	 Time: 1.928 seconds
E[3], train Loss: 2.301989, training Acc: 0.111, val loss: 2.302, val Acc: 0.113	 Time: 1.931 seconds
E[3], train Loss: 2.301989, training Acc: 0.111, val loss: 2.302, val Acc: 0.113	 Time: 1.933 seconds
E[3], train Loss: 2.301989, training Acc: 0.111, val loss: 2.302, val Acc: 0.113	 Time: 1.932 seconds
Epoch - 4, step #000000/000234	Loss: 2.300567
Epoch - 4, step #000100/000234	Loss: 2.303193
Epoch - 4, step #000200/000234	Loss: 2.302567
E[4], train Loss: 2.301999, training Acc: 0.111, val loss: 2.304, val Acc: 0.113	 Time: 2.054 seconds
E[4], train Loss: 2.301999, training Acc: 0.111, val loss: 2.304, val Acc: 0.113	 Time: 2.054 seconds
E[4], train Loss: 2.301999, training Acc: 0.111, val loss: 2.304, val Acc: 0.113	 Time: 2.054 seconds
E[4], train Loss: 2.301999, training Acc: 0.111, val loss: 2.304, val Acc: 0.113	 Time: 2.054 seconds
E[4], train Loss: 2.301999, training Acc: 0.111, val loss: 2.304, val Acc: 0.113	 Time: 2.058 seconds
E[4], train Loss: 2.301999, training Acc: 0.111, val loss: 2.304, val Acc: 0.113	 Time: 2.054 seconds
E[4], train Loss: 2.301999, training Acc: 0.111, val loss: 2.304, val Acc: 0.113	 Time: 2.061 seconds
E[4], train Loss: 2.301999, training Acc: 0.111, val loss: 2.304, val Acc: 0.113	 Time: 2.057 seconds
Epoch - 5, step #000000/000234	Loss: 2.306083
Epoch - 5, step #000100/000234	Loss: 2.297890
Epoch - 5, step #000200/000234	Loss: 2.304049
E[5], train Loss: 2.302144, training Acc: 0.110, val loss: 2.302, val Acc: 0.113	 Time: 1.919 seconds
E[5], train Loss: 2.302144, training Acc: 0.110, val loss: 2.302, val Acc: 0.113	 Time: 1.926 seconds
E[5], train Loss: 2.302144, training Acc: 0.110, val loss: 2.302, val Acc: 0.113	 Time: 1.922 seconds
E[5], train Loss: 2.302144, training Acc: 0.110, val loss: 2.302, val Acc: 0.113	 Time: 1.924 seconds
E[5], train Loss: 2.302144, training Acc: 0.110, val loss: 2.302, val Acc: 0.113	 Time: 1.929 seconds
E[5], train Loss: 2.302144, training Acc: 0.110, val loss: 2.302, val Acc: 0.113	 Time: 1.926 seconds
E[5], train Loss: 2.302144, training Acc: 0.110, val loss: 2.302, val Acc: 0.113	 Time: 1.927 seconds
E[5], train Loss: 2.302144, training Acc: 0.110, val loss: 2.302, val Acc: 0.113	 Time: 1.925 seconds
Epoch - 6, step #000000/000234	Loss: 2.300677
Epoch - 6, step #000100/000234	Loss: 2.303640
Epoch - 6, step #000200/000234	Loss: 2.305257
E[6], train Loss: 2.302086, training Acc: 0.112, val loss: 2.302, val Acc: 0.113	 Time: 2.039 seconds
E[6], train Loss: 2.302086, training Acc: 0.112, val loss: 2.302, val Acc: 0.113	 Time: 2.038 seconds
E[6], train Loss: 2.302086, training Acc: 0.112, val loss: 2.302, val Acc: 0.113	 Time: 2.039 seconds
E[6], train Loss: 2.302086, training Acc: 0.112, val loss: 2.302, val Acc: 0.113	 Time: 2.041 seconds
E[6], train Loss: 2.302086, training Acc: 0.112, val loss: 2.302, val Acc: 0.113	 Time: 2.037 seconds
E[6], train Loss: 2.302086, training Acc: 0.112, val loss: 2.302, val Acc: 0.113	 Time: 2.042 seconds
E[6], train Loss: 2.302086, training Acc: 0.112, val loss: 2.302, val Acc: 0.113	 Time: 2.041 seconds
E[6], train Loss: 2.302086, training Acc: 0.112, val loss: 2.302, val Acc: 0.113	 Time: 2.043 seconds
Epoch - 7, step #000000/000234	Loss: 2.297984
Epoch - 7, step #000100/000234	Loss: 2.303073
Epoch - 7, step #000200/000234	Loss: 2.302372
E[7], train Loss: 2.301994, training Acc: 0.110, val loss: 2.301, val Acc: 0.113	 Time: 1.968 seconds
E[7], train Loss: 2.301994, training Acc: 0.110, val loss: 2.301, val Acc: 0.113	 Time: 1.971 seconds
E[7], train Loss: 2.301994, training Acc: 0.110, val loss: 2.301, val Acc: 0.113	 Time: 1.968 seconds
E[7], train Loss: 2.301994, training Acc: 0.110, val loss: 2.301, val Acc: 0.113	 Time: 1.970 seconds
E[7], train Loss: 2.301994, training Acc: 0.110, val loss: 2.301, val Acc: 0.113	 Time: 1.971 seconds
E[7], train Loss: 2.301994, training Acc: 0.110, val loss: 2.301, val Acc: 0.113	 Time: 1.971 seconds
E[7], train Loss: 2.301994, training Acc: 0.110, val loss: 2.301, val Acc: 0.113	 Time: 1.972 seconds
E[7], train Loss: 2.301994, training Acc: 0.110, val loss: 2.301, val Acc: 0.113	 Time: 1.973 seconds
Epoch - 8, step #000000/000234	Loss: 2.302720
Epoch - 8, step #000100/000234	Loss: 2.302892
Epoch - 8, step #000200/000234	Loss: 2.302094
E[8], train Loss: 2.302105, training Acc: 0.110, val loss: 2.301, val Acc: 0.113	 Time: 1.869 seconds
E[8], train Loss: 2.302105, training Acc: 0.110, val loss: 2.301, val Acc: 0.113	 Time: 1.871 seconds
E[8], train Loss: 2.302105, training Acc: 0.110, val loss: 2.301, val Acc: 0.113	 Time: 1.871 seconds
E[8], train Loss: 2.302105, training Acc: 0.110, val loss: 2.301, val Acc: 0.113	 Time: 1.875 seconds
E[8], train Loss: 2.302105, training Acc: 0.110, val loss: 2.301, val Acc: 0.113	 Time: 1.874 seconds
E[8], train Loss: 2.302105, training Acc: 0.110, val loss: 2.301, val Acc: 0.113	 Time: 1.874 seconds
E[8], train Loss: 2.302105, training Acc: 0.110, val loss: 2.301, val Acc: 0.113	 Time: 1.870 seconds
E[8], train Loss: 2.302105, training Acc: 0.110, val loss: 2.301, val Acc: 0.113	 Time: 1.874 seconds
Epoch - 9, step #000000/000234	Loss: 2.302431
Epoch - 9, step #000100/000234	Loss: 2.304149
Epoch - 9, step #000200/000234	Loss: 2.303067
E[9], train Loss: 2.302098, training Acc: 0.110, val loss: 2.301, val Acc: 0.113	 Time: 1.938 seconds
E[9], train Loss: 2.302098, training Acc: 0.110, val loss: 2.301, val Acc: 0.113	 Time: 1.939 seconds
E[9], train Loss: 2.302098, training Acc: 0.110, val loss: 2.301, val Acc: 0.113	 Time: 1.945 seconds
E[9], train Loss: 2.302098, training Acc: 0.110, val loss: 2.301, val Acc: 0.113	 Time: 1.946 seconds
E[9], train Loss: 2.302098, training Acc: 0.110, val loss: 2.301, val Acc: 0.113	 Time: 1.947 seconds
E[9], train Loss: 2.302098, training Acc: 0.110, val loss: 2.301, val Acc: 0.113	 Time: 1.945 seconds
E[9], train Loss: 2.302098, training Acc: 0.110, val loss: 2.301, val Acc: 0.113	 Time: 1.948 seconds
E[9], train Loss: 2.302098, training Acc: 0.110, val loss: 2.301, val Acc: 0.113	 Time: 1.946 seconds
Epoch - 10, step #000000/000234	Loss: 2.300002
Epoch - 10, step #000100/000234	Loss: 2.298950
Epoch - 10, step #000200/000234	Loss: 2.301614
E[10], train Loss: 2.302067, training Acc: 0.111, val loss: 2.302, val Acc: 0.113	 Time: 2.023 seconds
E[10], train Loss: 2.302067, training Acc: 0.111, val loss: 2.302, val Acc: 0.113	 Time: 2.023 seconds
E[10], train Loss: 2.302067, training Acc: 0.111, val loss: 2.302, val Acc: 0.113	 Time: 2.029 seconds
E[10], train Loss: 2.302067, training Acc: 0.111, val loss: 2.302, val Acc: 0.113	 Time: 2.029 seconds
E[10], train Loss: 2.302067, training Acc: 0.111, val loss: 2.302, val Acc: 0.113	 Time: 2.026 seconds
E[10], train Loss: 2.302067, training Acc: 0.111, val loss: 2.302, val Acc: 0.113	 Time: 2.027 seconds
E[10], train Loss: 2.302067, training Acc: 0.111, val loss: 2.302, val Acc: 0.113	 Time: 2.028 seconds
E[10], train Loss: 2.302067, training Acc: 0.111, val loss: 2.302, val Acc: 0.113	 Time: 2.030 seconds
Epoch - 11, step #000000/000234	Loss: 2.303018
Epoch - 11, step #000100/000234	Loss: 2.305015
Epoch - 11, step #000200/000234	Loss: 2.301347
E[11], train Loss: 2.302324, training Acc: 0.109, val loss: 2.301, val Acc: 0.113	 Time: 2.129 seconds
E[11], train Loss: 2.302324, training Acc: 0.109, val loss: 2.301, val Acc: 0.113	 Time: 2.132 seconds
E[11], train Loss: 2.302324, training Acc: 0.109, val loss: 2.301, val Acc: 0.113	 Time: 2.135 seconds
E[11], train Loss: 2.302324, training Acc: 0.109, val loss: 2.301, val Acc: 0.113	 Time: 2.132 seconds
E[11], train Loss: 2.302324, training Acc: 0.109, val loss: 2.301, val Acc: 0.113	 Time: 2.133 seconds
E[11], train Loss: 2.302324, training Acc: 0.109, val loss: 2.301, val Acc: 0.113	 Time: 2.130 seconds
E[11], train Loss: 2.302324, training Acc: 0.109, val loss: 2.301, val Acc: 0.113	 Time: 2.136 seconds
E[11], train Loss: 2.302324, training Acc: 0.109, val loss: 2.301, val Acc: 0.113	 Time: 2.136 seconds
Epoch - 12, step #000000/000234	Loss: 2.303339
Epoch - 12, step #000100/000234	Loss: 2.301337
Epoch - 12, step #000200/000234	Loss: 2.301981
E[12], train Loss: 2.302288, training Acc: 0.111, val loss: 2.302, val Acc: 0.113	 Time: 1.830 seconds
E[12], train Loss: 2.302288, training Acc: 0.111, val loss: 2.302, val Acc: 0.113	 Time: 1.833 seconds
E[12], train Loss: 2.302288, training Acc: 0.111, val loss: 2.302, val Acc: 0.113	 Time: 1.833 seconds
E[12], train Loss: 2.302288, training Acc: 0.111, val loss: 2.302, val Acc: 0.113	 Time: 1.833 seconds
E[12], train Loss: 2.302288, training Acc: 0.111, val loss: 2.302, val Acc: 0.113	 Time: 1.834 seconds
E[12], train Loss: 2.302288, training Acc: 0.111, val loss: 2.302, val Acc: 0.113	 Time: 1.833 seconds
E[12], train Loss: 2.302288, training Acc: 0.111, val loss: 2.302, val Acc: 0.113	 Time: 1.837 seconds
E[12], train Loss: 2.302288, training Acc: 0.111, val loss: 2.302, val Acc: 0.113	 Time: 1.836 seconds
Epoch - 13, step #000000/000234	Loss: 2.302606
Epoch - 13, step #000100/000234	Loss: 2.299939
Epoch - 13, step #000200/000234	Loss: 2.302994
E[13], train Loss: 2.302247, training Acc: 0.111, val loss: 2.303, val Acc: 0.113	 Time: 1.860 seconds
E[13], train Loss: 2.302247, training Acc: 0.111, val loss: 2.303, val Acc: 0.113	 Time: 1.863 seconds
E[13], train Loss: 2.302247, training Acc: 0.111, val loss: 2.303, val Acc: 0.113	 Time: 1.863 seconds
E[13], train Loss: 2.302247, training Acc: 0.111, val loss: 2.303, val Acc: 0.113	 Time: 1.860 seconds
E[13], train Loss: 2.302247, training Acc: 0.111, val loss: 2.303, val Acc: 0.113	 Time: 1.861 seconds
E[13], train Loss: 2.302247, training Acc: 0.111, val loss: 2.303, val Acc: 0.113	 Time: 1.862 seconds
E[13], train Loss: 2.302247, training Acc: 0.111, val loss: 2.303, val Acc: 0.113	 Time: 1.863 seconds
E[13], train Loss: 2.302247, training Acc: 0.111, val loss: 2.303, val Acc: 0.113	 Time: 1.865 seconds
Epoch - 14, step #000000/000234	Loss: 2.301358
Epoch - 14, step #000100/000234	Loss: 2.301804
Epoch - 14, step #000200/000234	Loss: 2.304621
E[14], train Loss: 2.302156, training Acc: 0.110, val loss: 2.302, val Acc: 0.113	 Time: 2.243 seconds
E[14], train Loss: 2.302156, training Acc: 0.110, val loss: 2.302, val Acc: 0.113	 Time: 2.243 seconds
E[14], train Loss: 2.302156, training Acc: 0.110, val loss: 2.302, val Acc: 0.113	 Time: 2.242 seconds
E[14], train Loss: 2.302156, training Acc: 0.110, val loss: 2.302, val Acc: 0.113	 Time: 2.238 seconds
E[14], train Loss: 2.302156, training Acc: 0.110, val loss: 2.302, val Acc: 0.113	 Time: 2.246 seconds
E[14], train Loss: 2.302156, training Acc: 0.110, val loss: 2.302, val Acc: 0.113	 Time: 2.244 seconds
E[14], train Loss: 2.302156, training Acc: 0.110, val loss: 2.302, val Acc: 0.113	 Time: 2.244 seconds
E[14], train Loss: 2.302156, training Acc: 0.110, val loss: 2.302, val Acc: 0.113	 Time: 2.242 seconds
Epoch - 15, step #000000/000234	Loss: 2.300126
Epoch - 15, step #000100/000234	Loss: 2.303293
Epoch - 15, step #000200/000234	Loss: 2.302944
E[15], train Loss: 2.302010, training Acc: 0.111, val loss: 2.302, val Acc: 0.113	 Time: 1.946 seconds
E[15], train Loss: 2.302010, training Acc: 0.111, val loss: 2.302, val Acc: 0.113	 Time: 1.951 seconds
E[15], train Loss: 2.302010, training Acc: 0.111, val loss: 2.302, val Acc: 0.113	 Time: 1.950 seconds
E[15], train Loss: 2.302010, training Acc: 0.111, val loss: 2.302, val Acc: 0.113	 Time: 1.948 seconds
E[15], train Loss: 2.302010, training Acc: 0.111, val loss: 2.302, val Acc: 0.113	 Time: 1.946 seconds
E[15], train Loss: 2.302010, training Acc: 0.111, val loss: 2.302, val Acc: 0.113	 Time: 1.951 seconds
Total training time: 48.139211654663086 seconds
E[15], train Loss: 2.302010, training Acc: 0.111, val loss: 2.302, val Acc: 0.113	 Time: 1.952 seconds
E[15], train Loss: 2.302010, training Acc: 0.111, val loss: 2.302, val Acc: 0.113	 Time: 1.949 seconds
Total training time: 48.157005071640015 seconds
Total training time: 48.100271224975586 seconds
Total training time: 48.1486713886261 seconds
Total training time: 48.203784227371216 seconds
Total training time: 48.137892723083496 seconds
Total training time: 48.101069927215576 seconds
Total training time: 48.22726559638977 seconds

```