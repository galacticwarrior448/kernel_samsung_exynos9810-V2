# KernelSU for Exynos 9810
## Build from source

From a pre existing aosp source environment :-

```
cd kernel/samsung
git clone https://github.com/galacticwarrior448/kernel_samsung_exynos9810-V2 exynos9810
cd exynos9810
git clone https://github.com/galacticwarrior448/kernel_samsung_exynos9810-V2/ -b KernelSU KernelSU
ln -sf ../KernelSU/kernel drivers/kernelsu
cd ../../../
make bootimage -j$(nproc --all)
```
