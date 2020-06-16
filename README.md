
1. It is important to note that this work was conducted using the source code of CycleGAN (Unpaired Image-to-Image Translation using Cycle-Consistent Adversarial Networks).
2. The code of CycleGAN was shared by Jun-yan Zhu, et al. （http://people.csail.mit.edu/junyanz/）
3. More details about this code can be found at https://github.com/junyanz/CycleGAN.

=======================
1. train a model
python train.py --dataroot ./datasets/real_lrct2hrct_9to5 --name real_lrct2hrct_9to5_cyclegan --model  cycle_gan  --load_size 256  --crop_size 256 --batch_size 1  --niter 25  --niter_decay 25  --input_nc  1   --output_nc 1  --gpu_ids 0

2. test the model
python test.py --dataroot datasets/real_lrct2hrct_9to5 --name real_lrct2hrct_9to5_cyclegan --model test --no_dropout --input_nc  1   --output_nc 1   --load_size 256  --crop_size 256  --num_test  1  --gpu_ids 0


