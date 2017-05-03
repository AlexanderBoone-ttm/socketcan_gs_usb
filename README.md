# Fixed gs_usb driver for recent kernels

This module includes fixes for recent (>4.9) kernels where the existing gs_usb driver attempted to use stack-allocated buffers for USB communication, which caused the driver to fail.

A patch containing these fixes has been accepted to the Linux kernel.

## Build
<code>
  make
</code>

## Install (as root)

<code>
  rmmod gs_usb

  insmod ./gs_usb.ko
</code>
