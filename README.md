After upgrading to Fedora 32 and 5.6.6 kernel, the Nvidia driver 390.132 stopped working.

# Building the Nvidia driver 390.132 with patch

The patch was downloaded from [here](https://gitlab.com/snippets/1943873) and aplied over a [Nvidia driver 390.132 patched for kernel 5.5](https://nvidia.if-not-true-then-false.com/NVIDIA-Linux-x86_64-390.132-kernel-5.5-patched.run).

Run the following command:

`./NVIDIA-Linux-x86_64-390.132-kernel-5.5-patched.run --apply-patch kernel-5.6.patch`

This will create another archived executable with the name ending in **_custom.run**. Running this executable should successfully build and install the nvidia driver.

The final file can be downloaded from [here](https://drive.google.com/file/d/1gICEe8mMJ-P-tQypBeVgGuaPX_7GX7D9/view?usp=sharing).
