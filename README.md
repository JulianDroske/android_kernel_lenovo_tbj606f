# Kernel for Lenovo Tab P11 (TB-J606F)

This is a bootable kernel for Lenovo TB-J606F, adapted from
[Lenovo Opensource Portal](https://support.lenovo.com/us/en/solutions/ht511330-lenovo-open-source-portal)
.

For current status, see [STATUS.md](./STATUS.md).


## Testing Environment

- Device
	- Name: Lenovo Tab P11
	- Model: TB-J606F
	- Bootloader
		- Product: bengal
	- Vendor Info
		- Version: Android 10
		- Board: bengal
		- Platform: bengal
		- Name: m11_prc_wifi
	- Device Tree/compatible
		- qcom,bengalp-idp
		- qcom,bengalp
		- qcom,idp
- Compiler
	- `Compiler: Android (5484270 based on r353983c) clang version 9.0.3 (https://android.googlesource.com/toolchain/clang 745b335211bb9eadfa6aa6301f84715cee4b37c5) (https://android.googlesource.com/toolchain/llvm 60cf23e54e46c807513f7a36d0a7b777920b5881) (based on LLVM 9.0.3svn)`
	- Provided by Lenovo Opensource Portal

The whole ufs flash has been rewritten with other unbrick stock ROMs (source lost),
so some of the information above may differ from any stock devices.


## Additional Notes

There's [another kernel source](https://github.com/adazem009/kernel_lenovo_tbj606)
that should work
([source](https://github.com/lenovo/gplcc/issues/1#issuecomment-2285915620)),
however it failed to boot on my device.

This kernel is not intended to run on all TB-J606* devices, neither should mainline (for now).
Current goal is to support both AOSP and Linux Mobile (libhybris) operating systems,
while being ready for daily use.
